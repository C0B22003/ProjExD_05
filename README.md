# ゲーム のタイトル
Banging Splash
## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
プレイヤーは画面下部に配置されています。プレイヤーは左右に移動し、スペースキーを押すことで弾を発射できます。
敵は画面上部からランダムに出現し、左右に移動します。プレイヤーが弾を当てると、新しい敵がランダムな位置に再出現します。
ゲームの目標は、できるだけ多くの敵を倒してスコアを稼ぐことです。主人公キャラクターが敵を倒すシューティングゲーム

## ゲームの実装
操作方法:
左矢印キー: プレイヤーを左に移動
右矢印キー: プレイヤーを右に移動
スペースキー: 弾を発射
左シフトキー: スコアを消費してバリアを生成
右シフトキー: スコアを消費して散弾銃モード

要素:4
プレイヤー（playerImg）: 左右に移動できる宇宙船。
敵（enemyImg）: 画面上部から左右に移動する敵宇宙船。
弾（bulletImg）: プレイヤーと敵が発射する弾。
バリア（shield）: プレイヤーが生成するバリア###共通基本機能
* 主人公キャラクターに関するクラス

### 担当追加機能
* 中西
敵の動きをランダム性（速度）のある横移動にする
* 金子
出るビームをあるポイント量を消費することによって出る散弾ビーム機能の追加
* 浅岡
敵を倒すと溜まるゲージの生成（マックス10）
* 南部
プレイヤーに敵が放出した弾に当たったらゲームオーバーになる機能
* 宮崎
敵が弾を一定の間隔で弾を放出する機能
* 伊藤
ゲージをある量使用して発生させるバリア生成機能
### ToDo
- [ ] 敵横移動機能
- [ ] 散弾機能
- [ ] バリア機能
- [ ] ゲージ機能
- [ ] 敵の攻撃機能- [ ]
### メモ
* クラス内の変数は，すべて，「get_変数名」という名前のメソッドを介してアクセスするように設計してある
* すべてのクラスに関係する関数は，クラスの外で定義してある
* Keybordをインポートした
Banging Splashゲームは、プレイヤーが左右に移動可能な宇宙船で画面上部から出現する敵宇宙船を撃破し、
得点を稼ぐシンプルな2Dゲームです。プレイヤーは左右矢印キーで移動し、スペースキーで弾を発射します。
敵を倒すと得点が加算され、敵が画面下部に到達するとゲーム終了。
効果音やシンプルなグラフィックを使用し、改善点としてアニメーションやレベルごとの難易度変更が挙げられます。
PythonとPygameが必要な動作環境です。