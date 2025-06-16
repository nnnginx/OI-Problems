# AT_future_contest_2019_final_b ビジュアライザ

## 题目描述

[problemUrl]: https://atcoder.jp/contests/future-contest-2019-final/tasks/future_contest_2019_final_b

## 输入格式

无

## 输出格式

无

## 说明/提示

### テストケース生成

乱数シードを指定し、ローカル実行用にテストケースを生成する機能を用意しました。

- 本機能はchrome上での動作を想定しています。他の環境で正常に動作する保証はなく、特にIEでは動作しないことを確認しています。
- 本機能は当コンテスト上でのテストケースとの同一性を保証するものではありません。特に乱数生成の仕様に差異があることが考えられますので、予めご了承ください。

Seed=

<a download="testCase.txt" id="download" target="_blank"> </a> 

### ビジュアライザー

入力ファイルと出力ファイルから、点数の計算および結果を可視化するビジュアライザを用意しました。

- 本ビジュアライザはchrome上での動作を想定しています。他の環境で正常に動作する保証はなく、特にIEでは動作しないことを確認しています。
- 本ビジュアライザから解答の提出はできません。 AtCoder A問題「モンスターテイマー」上より解答を提出して下さい。
- 本ビジュアライザ上で計算された点数は、当コンテスト上での点数を保証するものではありません。本ビジュアライザを使用することによるあらゆる損害は保障しかねますので、予めご了承ください。

 入力ファイル：

 

   
 出力ファイル：

 

   
  
  ▶ 再生速度: 遅速 

    turn 

 

  

 

 

 たかはしくん は なかまに なりたそうに こちらをみている！ 

 

  Score

0

 

おかね

0

 

スキル

 

  

 ※表示するモンスターのビジュアライズは、あくまでイメージです。スコアには影響しません。

 
  const MAX_LEVEL = 10;
  const APPANAGE = 1000;
  const COST_TRAINING = 10000;
  var inputFlg = false;
  var loadedFlg = false;
  var T = 1000;
  var N = 10;
  var M = 30000;
  var rendTurn = 0;

  var tasks = [];

  var outputData = [];
  var order = [];

  var golds = [];
  var skills = [];
  var trainings = [];
  var done = []
  var mosterType = []
  var invalidQuests = []
  var doneQuests = []

  class Task{
	constructor(inputStr){
		this.start = Number(inputStr[0]);
		this.end = Number(inputStr[1]);
		this.gold = Number(inputStr[2]);
		this.takes = [...Array(N)].map(() => 0);
		for(var i=0; i &lt; N; i++){
			this.takes[i] = Number(inputStr[3 + i]);
		}
		this.done = false;
	}
	output(){
		ret = start + "-" + end + " \\" + gold + " \[" + takes[0];
		for(var i; i &lt; N; i++){
			ret += +","+takes[i];
		}
		ret += "\]"
		return ret;
	}
  }

  class Order{
	constructor(inputStr){
	  this.type = Number(inputStr[0]);
	  if(this.type == 1 || this.type == 2){
	    this.param = Number(inputStr[1]);
	  }
	}
	output(){
		ret = this.type;
		if(type == 1 || type == 2){
		  ret += "-" + this.param;
		}
		return ret;
	}
  }
  // テストケース生成
  $ ("#createTestCase").click(function\ ()\ {
\ let\ seed\ = $('#testCaseSeed').val();
      if (!isFinite(seed) || Number(seed) &lt; 0 || !seed){
          seed = 0;
          $ ('#testCaseSeed').val(seed);
\ }
\ console.log("seed="+seed);
\ const\ random\ =\ new\ Random(seed);
\ records\ =\ "1000\ 10\ 30000\r\n";
\ var\ quests\ =\ [];
\ var\ questType\ =\ [0,1,2];
\ var\ L\ =\ 0;
\ for\ (var\ i\ =\ 0;\ i\ <\ 30000;\ i++)\ {
\ switch(questType[random.nextInt(0,\ 2)]){
\ case\ 0:
\ L\ =\ random.nextInt(2,\ 10);
\ break;
\ case\ 1:
\ L\ =\ random.nextInt(11,\ 100);
\ break;
\ case\ 2:
\ L\ =\ random.nextInt(101,\ 1000);
\ break;
\ default:
\ console.log("Error!");
\ return;
\ }
\ var\ A\ =\ random.nextInt(1,\ Math.max(1,1000\ -\ L));
\ var\ B\ =\ A\ +\ L\ -\ 1;
\ var\ takes\ =\ [...Array(10)].map(()\ =>\ 0);
\ takes[0]\ =\ random.nextInt(1,\ 10);
\ for(var\ j\ =\ 1;\ j\ <\ 10;\ j++){
\ takes[j]\ =\ random.nextInt(0,\ takes[j-1]);
\ }
\ //\ シャッフル
\ for(var\ j\ =\ 10\ -\ 1;\ j\ >\ 0;\ j--){
\ var\ r\ =\ Math.floor(random.nextDouble()\ *\ (j\ +\ 1));
\ var\ tmp\ =\ takes[j];
\ takes[j]\ =\ takes[r];
\ takes[r]\ =\ tmp;
\ }
\ var\ sum\ =\ takes.reduce((a,x)\ =>\ a+=x,0);
\ var\ C\ =\ Math.floor(sum\ *\ 1.3\ *\ random.nextInt(1,2000\ ));

\ records\ +=\ A\ +\ "\ "\ +\ B\ +\ "\ "\ +\ C;
\ for(var\ j\ =\ 0;\ j\ <\ 10;\ j++){
\ records\ +=\ "\ "\ +\ takes[j];
\ }
\ records\ +=\ "\r\n";
\ }
\ var\ blob\ =\ new\ Blob([records],\ {
\ "type":\ "text/plain"
\ });
\ window.URL\ =\ window.webkitURL\ ||\ window.URL; $("#download").attr("href", window.URL.createObjectURL(blob));
      document.getElementById('download').innerText = "Input_" + seed;
      let fileName = "testCase_" + seed + ".txt";
      $ ('#download').attr('download',\ fileName);
\ });

\ class\ Random\ {
\ constructor(seed\ =\ 88675123)\ {
\ this.x\ =\ 123456789;
\ this.y\ =\ 362436069;
\ this.z\ =\ 521288629;
\ this.w\ =\ seed;
\ }

\ //\ XorShift
\ next()\ {
\ let\ t;

\ t\ =\ this.x\ ^\ (this.x\ <\ <\ 11);
\ this.x\ =\ this.y;\ this.y\ =\ this.z;\ this.z\ =\ this.w;
\ return\ this.w\ =\ (this.w\ ^\ (this.w\ >>>\ 19))\ ^\ (t\ ^\ (t\ >>>\ 8));
\ }
\ nextInt(min,\ max)\ {
\ const\ r\ =\ Math.abs(this.next());
\ return\ min\ +\ (r\ %\ (max\ +\ 1\ -\ min));
\ }
\ nextDouble()\ {
\ const\ r\ =\ Math.abs(this.next());
\ return\ (r\ %\ (1000000007\ +\ 1))\ /\ 1000000007;
\ }
\ };

\ //\ 入力ファイルの読込
\ var\ handleInputFiles\ =\ function\ (file,\ callback)\ {
\ document.getElementById('inputFile').innerText\ =\ '';
\ document.getElementById('outputFile').innerText\ =\ ''; $('#output').val('');
    inputFlg = false;
    loadedFlg = false;
    document.getElementById('score').innerText = 0;
    var reader = new FileReader();
    reader.readAsText(file[0]);
    reader.onload = function (ev) {
      const inputDatalist = reader.result.split(/\r\n|\r|\n/);
      if(inputDatalist.length &lt; 1){
        console.log("No Text Error!! " + inputDatalist.length);
        document.getElementById('inputFile').innerText = 'error!';
        $ ('#input').val('');
\ return;
\ }
\ var\ firstLine\ =\ inputDatalist[0].split("\ ");
\ if(firstLine.length\ !=\ 3){
\ console.log("First\ Line\ Error!!\ "\ +\ inputDatalist.length);
\ document.getElementById('inputFile').innerText\ =\ 'error!'; $('#input').val('');
        return;
      }
      for(var i = 0; i &lt; 3; i++){
        if(Number.isNaN(Number(firstLine[i]))){
          console.log("First Line Error!! " + inputDatalist.length);
          document.getElementById('inputFile').innerText = 'error!';
          $ ('#input').val('');
\ return;
\ }
\ }
\ T\ =\ Number(firstLine[0]);
\ N\ =\ Number(firstLine[1]);
\ M\ =\ Number(firstLine[2]);

\ tasks\ =\ [...Array(M)].map(()\ =>\ null);

\ if(inputDatalist.length\ <\ M){
\ console.log("T\ Error!!\ "\ +\ inputDatalist.length);
\ document.getElementById('inputFile').innerText\ =\ 'error!\ short\ line!'; $('#input').val('');
        return;
      }
      for (var i = 0; i &lt; M; i++) {
		line = inputDatalist[i+1].split(" ");
        if(line.length &lt; 3 + N){
          console.log("M error!! " + (i+1) + " " +inputDatalist[i].length);
          console.log(inputDatalist[i]);
          document.getElementById('inputFile').innerText = 'error! invalid task!';
          $ ('#input').val('');
\ return;
\ }
\ for\ (var\ j\ =\ 0;\ j\ <\ 3\ +\ N;\ j++)\ {
\ if(Number.isNaN(Number(line[j]))){
\ document.getElementById('inputFile').innerText\ =\ 'error!\ not\ number!';
\ console.log("type\ error!!\ Line="\ +\ i); $('#input').val('');
            return;
          }
          if(Number(line[j]) &lt; 0){
              document.getElementById('inputFile').innerText = 'error! negative value!';
              console.log("negative value error!! Line=" + i);
              $ ('#input').val('');
\ return;
\ }
\ if(j\ <\ 3){
\ continue;
\ }
\ if(Number(line[j])\ >\ MAX_LEVEL){
\ document.getElementById('inputFile').innerText\ =\ 'error!\ over\ level\ 10!';
\ console.log("over\ level\ error!!\ Line="\ +\ i); $('#input').val('');
              return;
          }
        }
        tasks[i] = new Task(line);
      }
      document.getElementById('inputFile').innerText = 'OK!';
      console.log("input OK!");
      inputFlg = true;
      setTimeout(function() {
        callback(-1);
      }, 50);
    };
  }

  function clearInFilePath() {
    $ ('#input').val('');
\ }
\ function\ clearOutFilePath()\ { $('#output').val('');
  }
  // 出力ファイルの読込
  function handleOutputFiles(file, callback) {
    document.getElementById('outputFile').innerText = '';
    if (!inputFlg) {
        document.getElementById('outputFile').innerText = 'input first!';
        $ ('#output').val('');
\ return;
\ }
\ loadedFlg\ =\ false;
\ outputData\ =\ [];
\ document.getElementById('score').innerText\ =\ 0;
\ var\ reader\ =\ new\ FileReader();
\ reader.readAsText(file[0]);
\ reader.onload\ =\ function\ (ev)\ {
\ const\ outputDatalist\ =\ reader.result.split(/\r\n|\r|\n/);
\ if(outputDatalist.length\ <\ T){
\ console.log("output\ filr\ error!");
\ document.getElementById('outputFile').innerText\ =\ 'error!\ short\ line!'; $('#output').val('');
        return;
      }
      order = [...Array(T)].map(() => null);
      for (var i = 0; i &lt; T; i++) {
        line = outputDatalist[i].split(" ");
        if(Number.isNaN(Number(line[0]))){
          console.log("output filr error! Line=" + i);
          console.log(row);
          document.getElementById('outputFile').innerText = 'error! not number!';
          $ ('#output').val('');
\ return;
\ }
\ switch(Number(line[0])){
\ case\ 1:
\ if(line.lengh\ <\ 2){
\ console.log("output\ filr\ error!\ Line="\ +\ i);
\ document.getElementById('outputFile').innerText\ =\ 'error!\ needs\ second\ param!'; $('#output').val('');
            return;
          }
          if(Number.isNaN(Number(line[1]))){
            console.log("output filr error! Line=" + i);
            console.log(row);
            document.getElementById('outputFile').innerText = 'error! not number!';
            $ ('#output').val('');
\ return;
\ }
\ if(Number(line[1])\ >\ MAX_LEVEL\ ||\ Number(line[1])\ <\ 1){
\ console.log("output\ filr\ error!\ Line="\ +\ i);
\ document.getElementById('outputFile').innerText\ =\ 'error!\ invalid\ skill\ no!'; $('#output').val('');
            return;
          }
          order[i] = new Order(line);
          break;
        case 2:
          if(line.lengh &lt; 2){
            console.log("output filr error! Line=" + i);
            document.getElementById('outputFile').innerText = 'error! needs second param!';
            $ ('#output').val('');
\ return;
\ }
\ if(Number.isNaN(Number(line[1]))){
\ console.log("output\ filr\ error!\ Line="\ +\ i);
\ console.log(row);
\ document.getElementById('outputFile').innerText\ =\ 'error!\ not\ number!'; $('#output').val('');
            return;
          }
          if(Number(line[1]) > M || Number(line[1]) &lt; 1){
            console.log("output filr error! Line=" + i);
            document.getElementById('outputFile').innerText = 'error! invalid task no!';
            $ ('#output').val('');
\ return;
\ }
\ order[i]\ =\ new\ Order(line);
\ break;
\ case\ 3:
\ order[i]\ =\ new\ Order(line);
\ break;
\ default:
\ document.getElementById('outputFile').innerText\ =\ 'error!\ not\ 1\ or\ 2\ or\ 3!';
\ console.log("output\ filr\ error!\ Line="\ +\ i);
\ console.log("error!!"); $('#output').val('');
          return;
        }
      }
      document.getElementById('outputFile').innerText = 'OK!';
      console.log("output OK!");
      loadedFlg = true;
      setTimeout(function() {
        simulate();
        callback(T+1);
      }, 50);
    };
  }

  function simulate() {
    if(!inputFlg || ! loadedFlg){
      return;
    }
    // init
    done = [...Array(M)].map(() => false);
    skills = [...Array(T+1)].map(() => [...Array(N)].map(() => 0));
    trainings = [...Array(T+1)].map(() => [...Array(N)].map(() => 0));
    golds = [...Array(T+1)].map(() =>  0);
    golds[0] = 1000;
    mosterType = [...Array(T+1)].map(() =>  "m1");
    invalidQuests = [...Array(T+1)].map(() => false);
    doneQuests = [...Array(T+1)].map(() => false);
    for (var i = 0; i &lt; T; i++) {
      // copy
      for(var j = 0; j &lt; N; j++) {
        skills[i+1][j] = skills[i][j];
        trainings[i+1][j] = trainings[i][j];
      }
      mosterType[i+1] = mosterType[i];

      var nowGold = golds[i];
      var nowOrder = order[i];
      switch(nowOrder.type){
        case 1:
          var skillNo = nowOrder.param-1;
          if(skills[i][skillNo] >= MAX_LEVEL){
            break;
          }
          var nextLevel = skills[i][skillNo] + 1;
          if(nowGold &lt; Math.pow(2,nextLevel) * COST_TRAINING){
            break;
          }
          nowGold -= Math.pow(2,nextLevel) * COST_TRAINING;
          trainings[i+1][skillNo]++;
          if(trainings[i+1][skillNo] >= nextLevel){
            trainings[i+1][skillNo]=0;
            skills[i+1][skillNo]++;

            var sum = 0;
            for(var j = 0; j &lt; N; j++) {
              sum += skills[i+1][j];
            }
            switch(sum){
              case 10:
                mosterType[i+1] = "m2-a"
                for(var j = 0; j &lt; N; j++) {
                  if(skills[i+1][j]>1){
                    mosterType[i+1] = "m2-b"
                    break;
                  }
                }
                break;
              case 20:
                mosterType[i+1] = "m3-a"
                for(var j = 0; j &lt; N; j++) {
                  if(skills[i+1][j]>2){
                    mosterType[i+1] = "m3-b"
                    break;
                  }
                }
                break;
              case 30:
                mosterType[i+1] = "m4-a"
                for(var j = 0; j &lt; N; j++) {
                  if(skills[i+1][j]>3){
                    mosterType[i+1] = "m4-b"
                    break;
                  }
                }
                break;
              case 50:
                mosterType[i+1] = "m5-a"
                for(var j = 0; j &lt; N; j++) {
                  if(skills[i+1][j]>5){
                    mosterType[i+1] = "m5-b"
                    break;
                  }
                }
                break;
              case 70:
                mosterType[i+1] = "m6-a"
                for(var j = 0; j &lt; N; j++) {
                  if(skills[i+1][j]>7){
                    mosterType[i+1] = "m6-b"
                    break;
                  }
                }
                break;
              case 90:
                mosterType[i+1] = "m7-a"
                for(var j = 0; j &lt; N; j++) {
                  if(skills[i+1][j]>9){
                    mosterType[i+1] = "m7-b"
                    break;
                  }
                }
                break;
              case 100:
                mosterType[i+1] = "m8"
                break;
              default:
                break;
            }
          }
          break;
        case 2:
          var task = tasks[nowOrder.param-1];
          if(task.start > i+1 || task.end &lt; i+1){
            invalidQuests[i] = true;
            break;
          }
          if(done[nowOrder.param-1]){
            doneQuests[i] = true;
            break;
          }

          money = task.gold;
          money *= (1 + 9 * (i+1 - task.start) / (task.end - task.start));
          skillLack = 0;
          for (var j = 0; j &lt; N; j++){
            skillLack += Math.max(0, task.takes[j] - skills[i][j]);
          }
          if (skillLack == 0){
            money *= 10;
          } else {
            money *= Math.pow(0.5, skillLack);
            money += 1e-9;
          }
          nowGold += Math.floor(money);
          done[nowOrder.param-1] = true;
          break;
        case 3:
        	nowGold += APPANAGE;
            break;
        default:
          document.getElementById('outputFile').innerText = 'error! not 1 or 2 or 3!';
          console.log("output filr error! Line=" + i);
          console.log("error!!");
          $ ('#output').val('');
\ return;
\ }
\ golds[i\ +\ 1]\ =\ nowGold;
\ var\ str\ =\ i\ +\ "\ "\ +\ nowGold\ +\ "\ \[";
\ for(var\ j\ =\ 0;\ j\ <\ N;\ j++){
\ str\ +=\ skills[i+1][j]\ +\ ",";
\ }
\ str\ +=\ "\]";
\ //console.log(str);
\ }
\ document.getElementById('score').innerText\ =\ golds[T];
\ }

\ function\ wrongAnswer(str,\ t)\ {
\ console.log("simulate\ error!!\ turn="+\ t\ +\ "\ "\ +\ str);
\ outputData\ =\ [];
\ _isRunning\ =\ false;
\ start.innerText\ =\ '▶';
\ render(t);
\ document.getElementById('slider1o').value\ =\ t;
\ document.getElementById('outputFile').innerText\ =\ 'error!';
\ document.getElementById('score').innerText\ =\ 'WA';
\ }

\ var\ render\ =\ function(rendTurn)\ {
\ this.rendTurn\ =\ rendTurn;
\ if(!inputFlg){
\ return;
\ }
\ if(rendTurn\ <\ 0){
\ document.getElementById('money').innerText\ =\ 0;
\ return;
\ }

\ if(!loadedFlg){
\ return;
\ }

\ if(rendTurn\ >=\ T){
\ document.getElementById('money').innerText\ =\ golds[T];
\ document.getElementById('message-area').innerHTML\ =
\ "あなた\ は"+golds[T]\ +\ "\ 円を"+"てにいれた！";
\ for(var\ i\ =\ 0;i\ <\ N;i++){
\ myChart.chart.data.datasets[0].data[i]\ =\ skills[T][i];
\ }
\ myChart.chart.update();
\ document.getElementById("monster").className\ =\ mosterType[T];
\ return;
\ }
\ document.getElementById('money').innerText\ =\ golds[rendTurn];
\ for(var\ i=0;i\ T\ +\ 2){
\ _isRunning\ =\ false;
\ start.innerText\ =\ '▶';
\ cancelAnimationFrame(_animationID);
\ output.value\ =\ 0;
\ return;
\ }
\ _animationID\ =\ requestAnimationFrame(autoUpdate);
\ frame++;
\ if(frame\ %\ (50\ -\ Number(animeSpeed.value))\ !==\ 0)\ {\ return;\ }
\ render(Number(output.value));
\ output.value\ =\ tmp;
\ value\ =\ tmp;
\ set_value();
\ }

\ //\ スタートボタンクリック
\ start.onclick\ =\ function(evt){
\ if\ (_isRunning)\ {
\ _isRunning\ =\ false;
\ start.innerText\ =\ '▶';
\ cancelAnimationFrame(_animationID);
\ }\ else\ if(loadedFlg){
\ _isRunning\ =\ true;
\ start.innerText\ =\ '■';
\ autoUpdate();
\ }\ else\ {
\ if(inputFlg\ &&\ order.length\ ==\ T+1){ $('#input').val('');
          $ ('#output').val('');
\ if(loadedFlg){
\ _isRunning\ =\ true;
\ start.innerText\ =\ '■';
\ autoUpdate();
\ }
\ }
\ }
\ };

\ //\ 目盛り部分をクリックしたとき
\ slider.onclick\ =\ function(evt){
\ dragging\ =\ true;
\ document.onmousemove(evt);
\ document.onmouseup();
\ };
\ //\ 数値の変更
\ output.onchange\ =\ function(evt){
\ value\ =\ evt.target.value;
\ render(Number(evt.target.value));
\ };
\ //\ ドラッグ開始
\ input.onmousedown\ =\ function(evt){
\ dragging\ =\ true;
\ return\ false;
\ };
\ //\ ドラッグ終了
\ document.onmouseup\ =\ function(evt){
\ if\ (dragging)\ {
\ dragging\ =\ false;
\ output.value\ =\ value;
\ render(value);
\ }
\ };
\ document.onmousemove\ =\ function(evt){
\ if(dragging){
\ //\ ドラッグ途中
\ if(!evt){
\ evt\ =\ window.event;
\ }
\ var\ left\ =\ evt.clientX;
\ var\ rect\ =\ slider.getBoundingClientRect();
\ //\ マウス座標とスライダーの位置関係で値を決める
\ value\ =\ Math.round(left\ -\ rect.left\ -\ width);
\ //\ スライダーからはみ出したとき
\ if\ (value\ <\ 0)\ {
\ value\ =\ 0;
\ }\ else\ if\ (value\ >\ slider.clientWidth)\ {
\ value\ =\ slider.clientWidth;
\ }
\ set_value();
\ return\ false;
\ }
\ };
\ })();
\ //色の設定
\ var\ colorSet\ =\ {
\ 	red:\ 'rgb(255,\ 99,\ 132)',
\ 	orange:\ 'rgb(255,\ 159,\ 64)',
\ 	yellow:\ 'rgb(255,\ 205,\ 86)',
\ 	green:\ 'rgb(75,\ 192,\ 192)',
\ 	blue:\ 'rgb(54,\ 162,\ 235)',
\ 	purple:\ 'rgb(153,\ 102,\ 255)',
\ 	grey:\ 'rgb(201,\ 203,\ 207)'
\ };

\ //\ 色のRGB変換
\ var\ color\ =\ Chart.helpers.color;

\ /*
\ *\ チャートの初期設定
\ */
\ var\ config\ =\ {
\ 	type:\ 'radar',
\ 	data:\ {
\ 		labels:\ ["No.1",\ "No.2",\ "No.3",\ "No.4",\ "No.5",\ "No.6",\ "No.7",\ "No.8",\ "No.9",\ "No.10"],
\ 		datasets:\ [{
\ 		\ label:\ "レベル",
\ 		\ backgroundColor:\ color(colorSet.blue).alpha(0.5).rgbString(),
\ 		\ borderColor:\ colorSet.blue,
\ 		\ pointBackgroundColor:\ colorSet.blue,
\ 		\ data:\ [0,\ 0,\ 0,\ 0,\ 0,\ 0,\ 0,\ 0,\ 0,\ 0]
\ 		},]
\ 	},
\ 	options:\ {
\ 		chartArea:\ {
\ backgroundColor:\ "#000"
\ },
\ animation:\ {
\ duration:\ 1500,
\ },
\ maintainAspectRatio:\ false,
\ 		showTooltips:\ false,
\ responsive:\ false,
\ 		legend:\ {
\ 		\ display:\ false
\ 		},
\ 		title:\ {
\ 			display:\ false
\ 		},
\ 		scale:\ {
\ 			display:\ true,
\ 			pointLabels:\ {
\ 				fontSize:\ 10,
\ 				fontColor:\ colorSet.yellow
\ 			},
\ 			gridLines:\ {
\ 				display:\ true,
\ 				color:\ colorSet.yellow
\ 			},
\ ticks:\ {
\ display:\ false,
\ fontColor:\ "#FFF",
\ fontSize:\ 8,
\ min:\ 0,
\ max:\ 10
\ }
\ 		}
\ 	}
\ };
\ var\ myChart\ =\ new\ Chart( $("#skill-chart"), config);