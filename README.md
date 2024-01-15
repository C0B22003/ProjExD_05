# ゲーム のタイトル
Banging Splash

## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
プレイヤーは画面下部に配置されています。  
プレイヤーは左右に移動し、スペースキーを押すことで弾を発射できます。  
敵は画面上部からランダムに出現し、左右に移動します。  
プレイヤーが弾を当てると、新しい敵がランダムな位置に再出現します。  
敵に弾を当てるとスコアが上がります。  
スコアが上がると同時にパワーポイントも上がります。  
パワーポイントに応じてアビリティを使うことができます。  
ゲームの目標は、できるだけ多くの敵を倒してスコアを稼ぐことです。  
20ポイントをとるとゲームクリア画面になります。  

## ゲームの実装
###共通基本機能
* YouTubeより拝借したインベーダーゲームコードを基にしている。  
https://www.youtube.com/watch?v=fAJ_BjLd3Ro  

***操作方法***:
左矢印キー: プレイヤーを左に移動
右矢印キー: プレイヤーを右に移動
スペースキー: 弾を発射
左シフトキー: スコアを消費してバリアを生成
右シフトキー: スコアを消費して散弾銃モード

### 担当追加機能
* ほげほげ
* ふがふが
* ぴよぴよ
### ToDo
- [ ] ほげほげ機能
- [ ] ふがふが関数内の変数名の統一
### メモ
* クラス内の変数は，すべて，「get_変数名」という名前のメソッドを介してアクセスするように設計してある
* すべてのクラスに関係する関数は，クラスの外で定義してある












# Banging Splash

# ゲーム のタイトル
Banging Splash


## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要

プレイヤーは画面下部に配置されています。プレイヤーは左右に移動し、スペースキーを押すことで弾を発射できます。
敵は画面上部からランダムに出現し、左右に移動します。プレイヤーが弾を当てると、新しい敵がランダムな位置に再出現します。
ゲームの目標は、できるだけ多くの敵を倒してスコアを稼ぐことです。

###　共通基本機能
* 自機キャラを操り、敵機を打ち倒すシューティングゲーム。
* YouTubeより拝借したインベーダーゲームコードを基にしている。

### メモ
* プレイヤーは画面下部に配置されています。プレイヤーは左右に移動し、スペースキーを押すことで弾を発射できます。
敵は画面上部からランダムに出現し、左右に移動します。プレイヤーが弾を当てると、新しい敵がランダムな位置に再出現します。
ゲームの目標は、できるだけ多くの敵を倒してスコアを稼ぐことです。主人公キャラクターが敵を倒すシューティングゲーム

## ゲームの実装

***操作方法***:
左矢印キー: プレイヤーを左に移動
右矢印キー: プレイヤーを右に移動
スペースキー: 弾を発射
左シフトキー: スコアを消費してバリアを生成
右シフトキー: スコアを消費して散弾銃モード

***要素***:4


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

バリア（shield）: プレイヤーが生成するバリア



得点:
敵宇宙船を倒すごとに、得点が加算されます。得点は画面左上に表示されます。

注意点:
敵宇宙船が放つ弾がプレイヤーに当たると、ゲームが終了します。

コードの構造:

***得点***:
敵宇宙船を倒すごとに、得点が加算されます。得点は画面左上に表示されます。

***注意点***:
敵宇宙船が放つ弾がプレイヤーに当たると、ゲームが終了します。

***コードの構造***:

得点:
敵宇宙船を倒すごとに、得点が加算されます。得点は画面左上に表示されます。

注意点:
敵宇宙船が放つ弾がプレイヤーに当たると、ゲームが終了します。

コードの構造:


Pygameライブラリを使用してウィンドウを作成し、ゲームのメインループを実装しています。
イベントハンドリングを使用して、キーボードの入力に応じてプレイヤーの動きや弾の発射を制御しています。
isCollision 関数は、弾と敵の衝突を検出しています。
スコアは画面左上に表示され、敵を倒すと増加します。


クリア条件:
敵が放つ弾に当たらずプレイヤーは敵を打ち落とし最高点を目指す

参考サイト:
https://www.youtube.com/watch?v=fAJ_BjLd3Ro
### 共通基本機能
* 主人公キャラクターに関するクラス
方向キーで左右に移動
スペースキーで弾の放出
* 敵に関するクラス
ランダムのスピードで左右に移動一定の時間ごとに弾の放出

### 担当追加機能
* 中西
敵の動きをランダム性（速度）のある横移動にする
### ToDo
- [ ] 敵横移動機能
- [ ] 散弾機能
- [ ] バリア機能
- [ ] ゲージ機能
- [ ] 敵の攻撃機能

### メモ
Banging Splashゲームは、プレイヤーが左右に移動可能な宇宙船で画面上部から出現する敵宇宙船を撃破し、
得点を稼ぐシンプルな2Dゲームです。プレイヤーは左右矢印キーで移動し、スペースキーで弾を発射します。
敵を倒すと得点が加算され、敵が画面下部に到達するとゲーム終了。
***クリア条件***:
敵が放つ弾に当たらずプレイヤーは敵を打ち落とし最高点を目指す

***参考サイト***:

クリア条件:
敵が放つ弾に当たらずプレイヤーは敵を打ち落とし最高点を目指す

参考サイト:

https://www.youtube.com/watch?v=fAJ_BjLd3Ro

###共通基本機能

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

敵が弾を一定の間隔で弾を放出する機能を追加。
enemybulletについて→座標とステータスを定義した。
fire_enemy_bulletで座標を更新する形にした。
isCollision、isPlayerHitで当たり判定に関する事を定義した。
背景を追加。

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

- [ ] 敵の攻撃機能

### メモ
Banging Splashゲームは、プレイヤーが左右に移動可能な宇宙船で画面上部から出現する敵宇宙船を撃破し、
得点を稼ぐシンプルな2Dゲームです。プレイヤーは左右矢印キーで移動し、スペースキーで弾を発射します。
敵を倒すと得点が加算され、敵が画面下部に到達するとゲーム終了。
効果音やシンプルなグラフィックを使用し、改善点としてアニメーションやレベルごとの難易度変更が挙げられます。
PythonとPygameが必要な動作環境です。


* 中西
敵の動きをランダム性（速度）のある横移動にする
* 金子
出るビームをあるポイント量を消費することによって出る散弾ビーム機能の追加
* アサオカ（担当コマンド）
敵を倒すと溜まるゲージの生成（マックス10）
ゲージの元となる図形を描画して敵に充てるたびにゲージが少しずつ増えていく仕組みにした。
* 南部
プレイヤーに敵が放出した弾に当たったらゲームオーバーになる機能
* 宮崎
敵が弾を一定の間隔で弾を放出する機能
* 伊藤
ゲージをある量使用して発生させるバリア生成機能
### ToDo

-  ゲージ機能（担当機能）
- 1.敵に当たるとゲージ増加
- 2.スキルを使うとゲージ減少



### メモ
シールドの状態や描画は、shield_state変数で管理されています。shield_stateが 'ready' のときはシールドが非アクティブで、'active' のときはシールドがアクティブです。

キー入力（'S'キー）によってシールドをアクティブにする処理があります。具体的には、キーが押されたとき（pygame.KEYDOWN イベント）、'S'キーが押された場合、shield_stateを 'active' に設定し、shieldXおよびshieldYをプレイヤーの位置に設定しています。

シールドがアクティブの場合、draw_shield関数が呼び出されて、シールドが描画されます。この関数は指定された位置 (x + 33, y) に半径 shield_radius の円を描画します。

敵がプレイヤーのシールドに当たったかどうかの判定は、isCollision関数で行われています。この関数は、円と円の衝突判定を行います。具体的には、isCollision(enemyX, enemyY, playerX, playerY, shield_radius, 32)のように呼び出されています。もしシールドがアクティブでかつ敵との衝突が検出されれば、shield_stateを 'ready' に設定し、新しい敵の位置をランダムに設定しています。

これにより、プレイヤーが 'S' キーを押すことでシールドをアクティブにし、敵の攻撃を防ぐことができるようになります。

今日は、ほかの人のゲージ生成と敵の弾が放出されて当たるコードをマージしていない
とりあえずシールドを生成して敵が自分に当たったら無効化されるコードの作成をした


# ゲーム のタイトル
Banging Splash
## 実行環境の必要条件
* python >= 3.10
* pygame >= 2.1

## ゲームの概要
主人公キャラクター豪華豚（ゴウカトン ）をマウス操作により丸焼きにするゲームで，・・・

## ゲームの実装
###共通基本機能
* 主人公キャラクターに関するクラス
### 担当追加機能
* ほげほげ
* ふがふが
* ぴよぴよ
### ToDo
- [ ] ほげほげ機能
- [ ] ふがふが関数内の変数名の統一
### メモ
* クラス内の変数は，すべて，「get_変数名」という名前のメソッドを介してアクセスするように設計してある
* すべてのクラスに関係する関数は，クラスの外で定義してある