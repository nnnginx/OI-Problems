## 籾朕嘘尚
仝認梧です々��厘頁認梧��、仝袗です々��厘頁袗��、仝ルビィです々��厘頁其曳��、仝3繁栽わせて、We are CYaRon�� よろしくね�　坑�眉繁壓匯軟��厘断頁CYaRon�ゞ犇獪現姪僑。�


CYaRon!議眉繁壓僥楼阻園殻岻朔��畳協窟苧匯嶽徭失議園殻囂冱��慢断各葎CYaRon!囂。



(ltt: 苧苧頁厘逸慢断窟苧議。)

辛頁��咀葎代紅得霞字宸扮昨融隼卯阻��ltt短嗤扮寂壅逸CYaRon!議眉了弌純純亟CYaRon!囂議盾瞥匂阻。


噐頁ltt祥竃阻宸劔匯祇籾��隼朔吉彭嗤繁住阻AC殻會祥裕恠公弌純純断。


## 籾朕宙峰
參和頁匯倖灸侏議CYaRon! 囂殻會。


```cpp
{ vars
    chika:int
    you:int
    ruby:array[int, 1..2]
    i:int
}
# 參貧延楚潮範峙譲葎0
# 延楚兆峪辛頁哂猟忖銚。

# yosoro囂鞘辛參補竃匯倖方忖��昧朔効匯倖腎鯉。
:yosoro 2
# 補竃2才匯倖腎鯉(參和音壅戻欺腎鯉)。

# set囂鞘辛參葎延楚験峙。
# 塰麻憲峪屶隔紗受催軸辛。
:set chika, 1
:set you, 2
:yosoro chika + you
# 貧匯訳囂鞘繍補竃3

# 參和議登僅囂鞘譲聞喘參和議鯉塀��
# 荷恬憲��燕器塀��燕器塀
# 箭泌eq, a, 1軸C囂冱嶄 a==1
# 侭嗤荷恬憲淫凄: lt: < gt: > le: <= ge: >= eq: == neq: !=

# 晩云栖議CYaRon眉繁短隈屎鳩仇窟竃if宸倖咄��咀緩慢断祥個撹阻ihu。
{ ihu eq, chika, 1
    :set you, 3
    :yosoro 1
}
# 補竃1
# 參貧頁ihu囂鞘��涙俶屶隔else。

# hor囂鞘揖尖��
# for i=1 to you泌和
{ hor i, 1, you
    :yosoro i
}
# 補竃1 2 3

# 泌和頁while才方怏議聞喘圭隈。
:set i, 1
{ while le, i, 2
    :yosoro i
    :set ruby[i], i+1
    :yosoro ruby[i]
    :set i, i+1
}
# 補竃1 2 2 3

# 方怏音氏竃�崘玉廝�軸峪氏嗤a[i]、a[i+2]遇音氏嗤窃貌噐a[i+b[i]]宸劔議。

# CYaRon囂議恷朔匯佩��匯協頁匯倖算佩。
 
```

低議販暦頁亟匯倖CYaRon!囂議盾瞥匂��糞�嵎簇�CYaRon!囂議殻會��盾瞥岻峇佩朔補竃峇佩潤惚。


## 補秘鯉塀
補秘猟周畠何葎CYaRon!囂殻會��恷朔匯佩隠屬頁倖腎佩。

萩侃尖補秘議扮昨��匯岷響欺EOF葎峭。


## 補竃鯉塀
乎CYaRon!囂殻會議峇佩潤惚。

醤悶貧��頁乎CYaRon!囂殻會侭嗤:yosoro囂鞘議補竃。


```input1
{ vars
    a:int
    b:int
}

:set a, 1
:set b, 2
:yosoro a+b

```

```output1
3
```

## 戻幣
斤方象恂竃參和隠屬��

1. 補秘方象匯協頁栽隈議CYaRon!囂殻會��音淫根廣瞥��旗鷹、抹序欠鯉 ��膨倖腎鯉��嚥貧峰劔箭�猴�。**徽音隠屬矯催、塰麻憲念中議腎鯉方楚才嗤涙匯協�猴�**。

2. 延楚兆壓10倖忖憲參和��叙淫根弌亟哂猟��方怏恷寄寄弌葎1000��延楚恷謹50倖��侭嗤燕器塀議塰麻潤惚��淫凄延楚議峙匯協壓int袈律坪。 �┻�方怏辛嬬頁窃貌噐[2001..3000]議��和炎辛嬬袈律葎0欺1叮��

3. 侭嗤峺綜弌亟。

4. 乎殻會匯協嬬校壓栽尖議扮寂、坪贋�渣督旄莞侏蟇蓮�

5. hor囂鞘峇佩狛殻嶄��儉桟延楚、兜兵峙、潤崩峙音氏瓜儉桟嶄議旗鷹個延。

6. **乎殻會恷謹500佩**

![](https://cdn.luogu.com.cn/upload/pic/4595.png)


