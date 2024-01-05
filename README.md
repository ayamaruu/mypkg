[![test](https://github.com/ayamaruu/src/actions/workflows/test.yml/badge.svg)](https://github.com/ayamaruu/src/actions/workflows/test.yml)

* ロボットシステム学用のレポジトリ
* ros2のパッケージ
## 導入方法
1.ターミナルを起動し、自分がコピーしたいディレクトリに移動する
2.ターミナル上で以下のコマンドを入力する
```
git clone git@github.com:ayamaruu/src.git
```
## 必要なソフトウェア
* Python
  * テスト済み: 3.7~3.10
* ros2を実行できる環境

## テスト環境
* Ubuntu 22.04.2 LTS
## 機能
* 1つのプログラムでtalker.pyを起動して、もう1つプログラムを立ち上げて使用する。
* 端末1で以下のコマンドを実行
```
ros2 run mypkg talker
```
* 端末2で以下のコマンドを実行
```
ros2 run mypkg listener
```
すると以下のように表示されます。
```
[INFO] [1704232808.151531925] [listener]: age: 44
```
Ctrl Cを押せばプログラムは終了します。
また、listenerを先に実行し、talkerをあとで実行すると、talkerを実行するまでの間、
```
[INFO] [1704233038.987095365] [listener]: 待機中
```
が表示され続けます。
## 備考
* このソフトウェアパッケージは、3条項BSDライセンスの下、再頒布および使用が許可されます.
* このパッケージのコードは下記のスライド(CC-BY-SA 4.0 by Ryuichi Ueda)のものを,本人の許可を得て自身の著作としたものです.
     * [ryuichiueda/my_slides robosys_2022](http://githb.com/ryuichiueda/my_slides/tree/master/robosys_2022)
* © 2023 Ayaka Murakoshi
