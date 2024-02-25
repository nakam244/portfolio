# 自己紹介
**中村 大智(なかむら だいち)**  
名古屋工学院専門学校 ゲーム総合学科  
卒業予定 2025年3月  

C#と設計を中心に勉強しています。  
ツール開発が好きです。  

作品のプロジェクトファイル、ビルドファイルは別途添付しているGoogleDriveをご覧ください。

## 使用できる言語/ツール  
一番自信のあるC#を基準に考えています。

| 言語/ツール  | 習熟度 |
|-----------|--------|
| C#        | ★★★★★☆ |
| Unity     | ★★★★★☆ |
| C++       | ★★★☆☆☆ |
| DirectX   | ★★☆☆☆☆ |
| HLSL/GLSL | ★★★☆☆☆ |

# 目次
- [2Dゲーム](#2d)
    - [クックストライク](#クックストライク)
    - [スライムラッシュ](#スライムラッシュ)
    - [パピルスのだいぼうけん](#パピルスのだいぼうけん)
- [3Dゲーム](#3d)
    - [Impact!](#impact)
    - [アマツバメ](#アマツバメ)
- [エディタ拡張/その他](#エディタ拡張その他)

# 2D
## クックストライク
<iframe width="560" height="315" src="https://www.youtube.com/embed/CG_xRZioAYI?si=-OQR1SQbavKKfZyj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

23年8月頃に行われた「プロトスプリントリーグ」(ゲームジャム)で制作した作品です。  
全5チームの作品の中から優秀賞に選ばれました。  

チーム人数 5人  
制作期間 3日  

主な担当箇所  
設計, ゲーム進行制御, お客さん関連(移動、生成, 注文/レシピUI), スコア, 評判(星)  

[unityroom](https://unityroom.com/games/cook-strike)で遊ぶことができます。  

## パピルスのだいぼうけん
<iframe width="560" height="315" src="https://www.youtube.com/embed/Axn6NJHxkwI?si=4YG3XoPowgJ5g_7t" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> 

ゴムを使ったワイヤーアクションです。ゴムを引っ張ってゴムパッチン！したり、ゴムの反動で勢いよくキックしたりして、敵を倒しながら進んでいきます。

チーム人数 6人  
制作期間 3か月  

主な担当箇所  
設計, ゲーム進行制御, プレイヤー制御, 収集アイテム, [エディター](#ステートマシン)  

## スライムラッシュ
<iframe width="560" height="315" src="https://www.youtube.com/embed/0nTE3o13VbQ?si=dIgHULWg1kaEJ1P0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>  

チーム人数 5人  
制作期間 2か月  

主な担当箇所  
設計, ゲーム進行制御, ダンジョン生成, カメラ制御, アイテム,  サウンド, ダメージ, ゲーム中UI全般, 武器選択画面

# 3D
## Impact!
<iframe width="560" height="315" src="https://www.youtube.com/embed/5e127fNT6hk?si=pbRNUQkbs_f3l5Dt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

全国専門学校ゲームコンペティションに向けて制作した作品です。
ファイナリストに選ばれました。

個人製作  
制作期間 2週間  

## アマツバメ
<iframe width="560" height="315" src="https://www.youtube.com/embed/cyGH6isQOco?si=ej6P3KKHTXOzrlKr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

チーム人数 6人  
制作期間 2ヵ月半  

主な担当箇所  
設計, ゲーム進行制御, レール制御, カメラ制御, [エディター](#コースエディタ)  

# エディタ拡張/その他
## ステージエディタ
シーンビュー上にグリッドを表示して、その上にオブジェクトを配置できるエディタです。
インスペクタから配置したいオブジェクトを選択して、ワンボタンで配置できます。

## ステートマシン  
特定のクラスを継承して「Action」と「Transition」を実装すると、エディタ上で使用できるようになります。  
複数のActionやTransitionを組み合わせてステートを作成することができます。  
エディタ上で任意のステートの参照を指定することができ、遷移先の指定に使うことができます。

## コースエディタ
レールシューターのステージを作るために制作したエディタです。Timelineを拡張しています。  
Splineを使って作ったレール上を、どの時間でどこまで移動するのかを設定したり、カメラの向きや回転、イージングを設定したりできるようにしました。  
また、敵の出現タイミングもTimelineから設定できるようにしています。