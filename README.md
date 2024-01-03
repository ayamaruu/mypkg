[![test](https://github.com/ayamaruu/src/actions/workflows/test.yml/badge.svg)](https://github.com/ayamaruu/src/actions/workflows/test.yml)

以下のコードはros2のツールとして使用できるものを提示しています。
## 導入方法
1.下記のリンクからサイトにとぶ
```
https://github.com/ayamaruu/src
```
2.ROS2のワークスペース上で以下のコードを実行する
```
colcon build
source ~/.bashrc
```
これらのプログラムを使用し、それぞれをファイルに保存し、ターミナルで以下の操作を行うことによって使用可能になる
```
chmod +x ファイル名
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
[INFO] [Listener]: Listen: 1
[INFO] [Listener]: Listen: 2
```
Ctrl Cを押せばプログラムは終了します。

## 備考
* このソフトウェアパッケージは、3条項BSDライセンスの下、再頒布および使用が許可されます.
* このパッケージのコードは下記のスライド(CC-BY-SA 4.0 by Ryuichi Ueda)のものを,本人の許可を得て自身の著作としたものです.
     * [ryuichiueda/my_slides robosys_2022](http://githb.com/ryuichiueda/my_slides/tree/master/robosys_2022)
* © 2023 Ayaka Murakoshi
