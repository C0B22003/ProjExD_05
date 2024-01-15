# ゲーム のタイトル
**Banging Splash**

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
プレイヤーは画面下部に配置されています。  
プレイヤーは左右に移動し、スペースキーを押すことで弾を発射できます。  
敵は画面上部からランダムに出現し、左右に移動します。  
敵はプレイヤーに向かって弾を打ってきます。  
当たるとゲームオーバーになります。  
プレイヤーが弾を当てると、新しい敵がランダムな位置に再出現します。  
プレイヤーが敵に弾を当てるとスコアが上がります。  
スコアが上がると同時にパワーポイントも上がります。  
パワーポイントに応じてアビリティを使うことができます。  
ゲームの目標は、できるだけ多くの敵を倒してスコアを稼ぐことです。  
20ポイントをとるとゲームクリア画面になります。  

## ゲームの実装
###共通基本機能
* YouTubeより拝借したインベーダーゲームコードを基にしている。  
→　https://www.youtube.com/watch?v=fAJ_BjLd3Ro

## 操作方法
**左矢印キー**: プレイヤーを左に移動  
**右矢印キー**: プレイヤーを右に移動  
**スペースキー**: 弾を発射  
**左シフトキー**: パワーを消費してバリアを生成  
**右シフトキー**: パワーを消費して散弾モード  

## ゲームの要素
* **プレイヤー（playerImg）** : 左右に移動できる宇宙船。
* **敵（enemyImg）** : 画面上部から左右に移動するエイリアン。
* **弾（bulletImg）**: プレイヤーと敵が発射する弾。
* **得点 (score)**: 敵宇宙船を倒すごとに、得点が加算されます。得点は画面左上に表示されます。20点取るとクリア画面に移る。  
* **パワー (power)**: 敵宇宙船を倒すごとに、得点が加算されます。得点は画面左上に表示されます。最大値は、10です。
   
***アビリティ***    
* **バリア**：パワーが5以上の時左シフトキーを押すとパワーを消費して、弾をはじくバリアを生成する。
* **散弾**：パワーが1以上の状態で打つとパワーをすべて消費して、パワー分の弾を打ちます。

## 担当追加機能
* **中西**  
敵の動きをランダム性（速度）のある横移動にする。
* **金子**  
出るビームをあるポイント量を消費することによって出る散弾ビーム機能の追加。
* **浅岡**  
敵を倒すと溜まるゲージの生成。クリア画面。
* **南部**  
プレイヤーに敵が放出した弾に当たったらゲームオーバーになる機能。
* **宮崎**  
敵が弾を一定の間隔で弾を放出する機能。

### メモ
