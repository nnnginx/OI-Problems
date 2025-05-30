## Description

<div><p>You are given a <a href="https://assets.codeforces.com/rounds/1356/training_data1.json">training dataset</a>, in which each entry is a features vector (an array of 2 real numbers) and a label 0 or 1 indicating the class to which this vector belongs.</p><p>Your goal is to use this dataset to train a quantum classification model that will accurately classify a validation dataset - a different dataset generated using the same data distribution as the training one. The error rate of classifying the validation dataset using your model (the percentage of incorrectly classified samples) should be less than 5 </p><ul> <li> The quantum classification library that will use your model to classify the data is documented <a href="https://docs.microsoft.com/quantum/libraries/machine-learning/">here</a>. </li><li> <a href="https://github.com/microsoft/MLADS2020-QuantumClassification">This tutorial</a> has an end-to-end example of training a model using this library as a Python notebook. </li><li> You can find examples of training a model and using it for classification <a href="https://github.com/microsoft/Quantum/tree/master/samples/machine-learning/">here</a>. </li></ul></div><div class="input-specification"><p>Your code will not be given any inputs. Instead, you should use the <a href="https://assets.codeforces.com/rounds/1356/training_data1.json">provided dataset file</a> to train your model.</p><p>The training dataset is represented as a JSON file and consists of two arrays, "Features" and "Labels". Each array has exactly 200 elements. Each element of the "Features" array is an array with 2 elements, each of them a floating-point number between -1 and 1. Each element of the "Labels" array is the label of the class to which the corresponding element of the "Features" array belongs, 0 or 1.</p></div><div class="output-specification"><p>Your code should return the description of the model you'd like to use in the following format:</p><ul> <li> The model is described using a tuple <span class="tex-font-style-tt">(ControlledRotation[], (Double[], Double))</span>. </li><li> The first element of the tuple describes circuit geometry of the model as an array of controlled rotation gates. </li><li> The second element of the tuple describes numeric parameters of the model and is a tuple of an array of rotation angles used by the gates and the bias used to decide the class of the model. </li></ul><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.MachineLearning;

    operation Solve () : (ControlledRotation[], (Double[], Double)) {
        // your code here
    }
}</pre><p>Please refer to the documentation and examples for details on each parameter.</p></div>

## Input

<p>Your code will not be given any inputs. Instead, you should use the <a href="https://assets.codeforces.com/rounds/1356/training_data1.json">provided dataset file</a> to train your model.</p><p>The training dataset is represented as a JSON file and consists of two arrays, "Features" and "Labels". Each array has exactly 200 elements. Each element of the "Features" array is an array with 2 elements, each of them a floating-point number between -1 and 1. Each element of the "Labels" array is the label of the class to which the corresponding element of the "Features" array belongs, 0 or 1.</p>

## Output

<p>Your code should return the description of the model you'd like to use in the following format:</p><ul> <li> The model is described using a tuple <span class="tex-font-style-tt">(ControlledRotation[], (Double[], Double))</span>. </li><li> The first element of the tuple describes circuit geometry of the model as an array of controlled rotation gates. </li><li> The second element of the tuple describes numeric parameters of the model and is a tuple of an array of rotation angles used by the gates and the bias used to decide the class of the model. </li></ul><p>Your code should have the following signature:</p><pre class="verbatim">namespace Solution {
    open Microsoft.Quantum.MachineLearning;

    operation Solve () : (ControlledRotation[], (Double[], Double)) {
        // your code here
    }
}</pre><p>Please refer to the documentation and examples for details on each parameter.</p>

## Note

<p>Note that majority of the data analysis is going to happen "offline" before you submit the solution. The solution has to contain only the description of the trained model, not the training code itself - if you attempt to train the model "online" in your submitted code during the evaluation process, it will very likely time out.</p><p>Training your model offline is likely to involve:</p><ul> <li> Defining the circuit structure that your model will use. </li><li> Generating several parameter seed vectors - the values from which training the model will start. </li><li> Selecting appropriate hyperparameters of the training process (learning rate, batch size, tolerance, maximal number of iterations etc.) </li><li> Training a number of classification models (one per each seed vector and hyperparameter combination) </li><li> Selecting the best trained model and submitting it. </li></ul>
