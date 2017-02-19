打席結果データの作成
===

# 概要
ヌルデータ置き場をクロールして、NPBの打席結果データを作る
http://lcom.sakura.ne.jp/NulData/2015/Central/G/f/25_stat.htm

こんな感じ

atbat,date,name,背番,打席番号
四球,2007-04-01,木村拓也,0,1
四球,2007-04-01,木村拓也,0,2
三ゴロ,2007-04-04,木村拓也,0,1
空三振,2007-04-04,木村拓也,0,2

参考: http://tamaobject.hatenablog.com/entry/2017/02/11/010214

# Todo

- [終了] チーム, 年度別の選手名と背番号データの作成
 - URLを作成するため
 - data/year_player_table.csv
- [終了] 年度,選手別の打席結果htmlのダウンロード
 - data/player_gameresult.csv
 - 移籍した場合は? 
  - 同姓同名がいたら詰む
  　- 2007年以降なら問題無し
 - プレーオフは?
 　- データに入っていないから、気にしなくていい
- [レビュー中]打席ごとのデータに整形
 - data/player_atbatresult.csv
 - 対戦相手の列とか必要かな...?
