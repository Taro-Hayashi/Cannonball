# Cannonball カーソルパッド ビルドガイド（[English](https://github.com/Taro-Hayashi/Cannonball/blob/main/README_EN.md)）
- [キット内容](#キット内容)
- [準備](#準備)
- [はんだ付け](#はんだ付け)
- [組み立て](#組み立て)
- [カスタマイズ](#カスタマイズ)
- [その他](#その他)

## キット内容
![](img/IMG_1757.jpeg) 
||部品名|数| |
|-|-|-|-|
|1|メインボード|1||
|2|ボトムプレート|1||
|3|ミドルプレート1|1||
|4|ミドルプレート2|1||
|5|保護プレート|1||
|6|ネジ（短）|4|3mm|
|7|ネジ（中）|2|5mm|
|8|ネジ（長）|6|6mm|
|9|スペーサー（短）|6|3mm|
|10|スペーサー（中）|2|4mm|
|11|ダイオード|13|1N4148|
|12|リセットスイッチ|1||
|13|ロータリーエンコーダ（ダイヤル）|1|EC11互換品|
|14|ノブ|1||
|15|ロータリーエンコーダ（ホイール）|2|EVQWGD001|
|16|ゴム足|6||
|17|Pro Micro|1||
|18|レバースイッチ|2|メインボードに取り付け済み。|

### キット以外に必要なもの
|部品名|数||
|-|-|-|
|キースイッチ|9|[Kailh choc V1](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)、もしくは[Kailh Choc V2](https://shop.yushakobo.jp/collections/all-switches/products/kailh-choc-v2)|
|キーキャップ|9|V1は[専用キーキャップ](https://shop.yushakobo.jp/collections/keycaps/For-Choc-v1)、V2は[CherryMX互換](https://shop.yushakobo.jp/collections/keycaps/cherry-mx-%E4%BA%92%E6%8F%9B-%E3%82%AD%E3%83%BC%E3%82%AD%E3%83%A3%E3%83%83%E3%83%97)です。|
|Micro USB ケーブル|1||

### オプション
|部品名|数||
|-|-|-|
|[SK6812MINI-E](https://shop.yushakobo.jp/products/sk6812mini-e-10)|9|バックライト|
|[WS2812B](https://shop.yushakobo.jp/products/a0800ws-01-10)|3|アンダーグロー|
|[色違いアクリルプレート](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890230296807)|||
|[コンスルー 12ピン、高さ2.5mm](https://shop.yushakobo.jp/products/31?_pos=1&_sid=ca92edae3&_ss=r&variant=37665714405537)|2|[使い方](conthrough.md)|

### 必要な工具
|工具名|
|-|
|はんだごて|
|こて先クリーナー（こて台）|
|鉛入りはんだ|
|精密ドライバー|
|ニッパー等ダイオードの足を切れるもの|
|エポシキ接着剤|
|Microsoft Edge、もしくはGoogle Chrome||

### あると便利な工具
|工具名|
|-|
|耐熱シリコンマット|
|温度調節可能なはんだごて|
|斜めに切ったタイプのこて先|
|フラックス|
|フラックスリムーバー、IPA|
|ピンセット|
|マスキングテープ|
|耐熱絶縁テープ（カプトンテープ）|
|テスター|
|はんだ吸い取り線|
|はんだ吸い取り器|



## 準備
Pro MicroはMicro-USB端子がもげやすいのでエポシキ接着剤で補強します。  
![](img/IMG_1011.jpeg)  
両サイドと手前側のはんだ付けされてるところに少し厚めに塗ります。端子の中に入り込まないように気を付けます。
![](img/IMG_1020.jpeg)  
乾燥させている間にはんだ付けを進めましょう。  

  
## はんだ付け
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  
[![](http://img.youtube.com/vi/JFQg_ObITYE/0.jpg)](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)  

### LEDのはんだ付け

LEDを取り付ける場合はメインボードに最初にはんだ付けします。
 - [LEDの取り付け方](led.md)  

### ダイオード、リセットスイッチのはんだ付け

D1からD13まで取り付けます。  
足を曲げて裏から差し込みます。  
![](img/IMG_1795.jpeg)  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  

表で更に足を曲げて抜けないようにします。  
![](img/IMG_1798.jpeg) 
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。  

はんだ付けをして足を切ります。  
![](img/IMG_1800.jpg)  

リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/IMG_1805.jpeg) 

フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/IMG_1821.jpeg) 

### キースイッチのはんだ付け

表から差し込み裏ではんだ付けします。  
![](img/IMG_5007.jpg)  
ここの二つのスイッチはPro Microと接触する可能性があるので、足を切ってからはんだ付けします。　　
![](img/IMG_5008.jpg)  
choc V1スイッチの場合、足が一か所干渉するので短くカットしてください。　　
![](img/IMG_5009.jpg)  
全てのスイッチをはんだ付けします。

### Pro Microのはんだ付け
隠れてしまうダイオードD3,D4の方向が合っているか、キースイッチの足がはんだ付けされているかを再度確認してください。  
Pro Microに付属しているピンヘッダの、短い側を基板に差し込みます。  
![](img/IMG_5010.jpg)  
Pro Microを乗せます。TX0, RAW, USBの位置をシルク印刷と合わせましょう。  
カプトンテープを持っている人は、ここで基板とPro Microが重なる部分を絶縁しておくと安心です。　　
![](img/IMG_5011.jpg)  
足をニッパーで切ったらはんだ付けします。  
![](img/IMG_5013.jpg)  
![](img/IMG_5014.jpg)  
基板側をはんだ付けします。  
![](img/IMG_5017.jpg)  


### 動作テスト
ロータリーエンコーダーを取り付ける前にPro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

テストファームウェアを選んでFLASHします。
![](img/remap02.jpg)  
![](img/remap03.jpg)  

キットのリセットスイッチを押すとArduino Microが現れるので、クリックして接続します。
![](img/remap04.jpg) 

書き込みが完了したらウィンドウを閉じて大丈夫です。
![](img/remap05.jpg) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。  

Remapを使ってファームウェアの更新ができない場合は、QMK Toolboxをお試しください。  
- [QMK Toolboxを使ったファームウェア更新方法](firmware.md)

### ロータリーエンコーダーのはんだ付け
表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/IMG_5019.jpg)  

ツメを穴に引っかけてからピンを穴に差し込みます。
ピンを曲げてしまわないように注意してください。
![](img/IMG_5021.jpg)  

差し込めたらはんだ付けします。
![](img/IMG_5024.jpg)  

表からダイヤル型のロータリーエンコーダーを取り付けて裏からはんだ付けします。
![](img/IMG_5022.jpg)
ピンが曲がらないように気を付けましょう。  
![](img/IMG_5025.jpg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/IMG_5026.jpg)  

お疲れ様でした。再び動作を確認して問題がなければはんだ付けは終了です。

## 組み立て
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。割れやすいので気をつけましょう。  

青丸のネジ穴を通してスペーサー（短）とスペーサー（中）を繋ぎます。  
![](img/IMG_5027.jpg)  
図のようにキースイッチがついてる側に少し長い方のスペーサーがあるようにしてください。  
![](img/IMG_5029.jpg)  

メインボード裏面のネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/IMG_5031.jpg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/IMG_5032.jpg)  
![](img/IMG_5037.jpg)  
ゴム足も取り付けました。

表に保護プレートをネジ（中）で取り付けましょう。
![](img/IMG_5038.jpg)  

マイナスドライバーでノブを取りつけたらキーキャップを取り付けて完成です。  
![](img/IMG_5043.jpg)  

先ほどと同様の手順で本番用のファームウェアに更新しましょう。  
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

![](img/remap06.jpg)  

## カスタマイズ
このキットはレイヤー機能を使っています。  
![](img/layout.jpg)  
[Keyboard Layout Editor で見る](http://www.keyboard-layout-editor.com/#/gists/2fe2023fd6a9318985b9c40c264c6cef)  

使わないキーを削除したり使用頻度の高いキーを押しやすい位置に変更してみましょう。  

ChromeかEdgeでRemapにアクセスしてください。  
- Remap https://remap-keys.app/

![](img/remap1.png)  
左を選んで進んでいくとアドレスバーからメッセージが出てキーボードを選択できます。  

ドラッグアンドドロップでキーマップの変更が終わったら右上のflashボタンを押すと反映されます。  
![](img/remap3.png)  

### 置く向きに合わせる
レイアウトオプションから方向を変えることができます。  
![](img/c.jpg)  

### レイアウトの保存と復元
⇔アイコンで作ったレイアウトを保存することができます。  
いくつかサンプルをご用意しました。自分のレイアウトを公開することもできるので是非お試しください。
![](img/re.jpg)  

## その他
### Bluetooth接続
- [BLE Micro Pro使用例](ble.md)

### ぱいとん様のゆっくり実況動画  
ユーザーの方が組み立ての手順をとてもわかりやすく動画にしてくださいました。   
ご購入の前に雰囲気を掴んだり、ビルドガイドと一緒に見ながら作業するとわかりやすいと思いますのでぜひご覧ください。  
[![](http://img.youtube.com/vi/m9hnfXNCipo/0.jpg)](https://www.youtube.com/watch?v=m9hnfXNCipo)  

### ファームウェアのフォルダ  
https://github.com/Taro-Hayashi/qmk_firmware/tree/tarohayashi/keyboards/tarohayashi/cannonball

### VIA用JSONファイル
- [cannonball.json](https://github.com/Taro-Hayashi/Cannonball/releases/download/15.20/cannonball.json)  

### プレートのデザインデータ  
[cannonball_plates.zip](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.31/cannonball_plates.zip)  
発注先のルールに沿ってデータを修正してください。  

### 謝辞
foostan様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/foostan/kbd/  
https://github.com/foostan/kbd/blob/master/LICENSE  

plut0nium様のフットプリントを流用、改変して使わせていただきました。  
https://github.com/plut0nium/0xLib  
https://github.com/plut0nium/0xLib/blob/master/LICENSE.txt  

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />この キット は <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">クリエイティブ・コモンズ 表示 - 継承 4.0 国際 ライセンス</a>の下に提供されています。

### 販売サイト
- 遊舎工房: https://shop.yushakobo.jp/collections/keyboard/products/2797   
- BOOTH: https://tarohayashi.booth.pm/items/3172502
