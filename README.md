# Cannonball カーソルパッド ビルドガイド（[English](https://github.com/Taro-Hayashi/Cannonball/blob/main/README_EN.md)）
- [キット内容](#キット内容)
- [準備](#準備)
- [はんだ付け](#はんだ付け)
- [組み立て](#組み立て)
- [キーのカスタマイズ](#キーのカスタマイズ)
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

### キット以外に必要なもの
|部品名|数||
|-|-|-|
|キースイッチ|9|[Kailh choc V1](https://shop.yushakobo.jp/collections/all-switches/products/pg1350)、もしくは[Kailh Choc V2](https://shop.yushakobo.jp/collections/all-switches/products/kailh-choc-v2)|
|キーキャップ|9|V1は[専用キーキャップ](https://shop.yushakobo.jp/collections/keycaps/For-Choc-v1)、V2は[CherryMX互換](https://shop.yushakobo.jp/collections/keycaps/cherry-mx-%E4%BA%92%E6%8F%9B-%E3%82%AD%E3%83%BC%E3%82%AD%E3%83%A3%E3%83%83%E3%83%97)です。|
|Micro USB ケーブル|1||

### オプション

#### LEDを光らせる場合
|部品名|数||
|-|-|-|
|[SK6812MINI-E](https://shop.yushakobo.jp/products/sk6812mini-e-10)|9|バックライト|
|[WS2812B](https://shop.yushakobo.jp/products/a0800ws-01-10)|3|アンダーグロー|

#### USB Type-Cに変更する場合
|部品名|数||
|-|-|-|
|Type-C版Pro Micro|1|[DailyCraftKeyboard](https://shop.dailycraft.jp/products/promicro_typec)、 [Talpkeyboard](https://talpkeyboard.net/items/62e24e6f8a0bd07fe2d38137)、[遊舎工房](https://shop.yushakobo.jp/products/sk6812mini-e-10)|
|3.5mmコンスルー|2|[DailyCraftKeyboard](https://shop.dailycraft.jp/products/conthrough_12_35)[Talpkeyboard](https://talpkeyboard.net/items/6229e8c130344b271f290c3c)、[マルツ電子](https://www.marutsu.co.jp/pc/i/2349912/)、|

使用方法はこちら
- [コンスルーの使用方法とPro Micro互換品の対応表](promicro.md)  

#### 色違いのアクリルプレート
- [キーボードアクリルプレート（遊舎工房）](https://shop.yushakobo.jp/collections/services/products/keyboard_acrylic_plate?variant=43890230296807)
- [プレートのデザインデータ](https://github.com/Taro-Hayashi/Cannonball/releases/download/14.31/cannonball_plates.zip)  


### 必要な工具
|工具名|
|-|
|はんだごて|
|はんだ|
|精密ドライバー|
|ニッパー等ダイオードの足を切れるもの|
|エポシキ接着剤|

## 準備
Pro MicroはMicro-USB端子をエポシキ接着剤で補強します。  
![](img/IMG_1011.jpeg)  
両サイドと手前側のはんだ付けされてるところに少し厚めに塗ります。端子の中に入り込まないように気を付けます。
![](img/IMG_1020.jpeg)  
乾燥させている間にはんだ付けを進めましょう。  

  
## はんだ付け
はんだ付けのやり方は動画で見るとわかりやすいです。  
パーツは思ったより壊れないので落ち着いて作業すると失敗しにくいです。  
 - ホームセンターのDCMさんの解説動画(58秒～)  
[![](http://img.youtube.com/vi/JFQg_ObITYE/0.jpg)](https://www.youtube.com/watch?v=JFQg_ObITYE&t=58s)  

### LEDのはんだ付け（オプション）

LEDを取り付ける場合はメインボードに最初にはんだ付けします。
 - [LEDの取り付け方](led.md)  

### ダイオード、リセットスイッチのはんだ付け

D1からD13までダイオードを取り付けます。  
足を曲げて裏から差し込みます。  

![](img/IMG_1794.jpg)  
ダイオードには向きがあります。三角形の先の棒と黒線を合わせましょう。  

表で更に足を曲げて抜けないようにします。  
![](img/IMG_1798.jpeg) 
ダイオードと並行に曲げるとあとでキースイッチに干渉しにくいです。  

はんだ付けをして足を切ります。  
![](img/IMG_1800.jpeg)  

リセットスイッチを裏から差し込み表ではんだ付けします。  
![](img/IMG_1805.jpeg) 

フラックスクリーナーを使う人はここで表面を綺麗にしておきましょう。  
![](img/IMG_1821.jpeg) 

### ピンヘッダーのはんだ付け（Pro Microはまだはんだ付けしません）
Pro Microの取り付け場所にピンヘッダーの短い側を差し込みます。
![](img/IMG_1833.jpeg)  
位置決めのためにPro Mioroを乗せますが、はんだ付けはせず表にします。
![](img/IMG_1834.jpg) 
![](img/IMG_1842.jpeg)  
メインボードにピンヘッダーをはんだ付けします。
![](img/IMG_1849.jpeg)  
Pro Microをいったん外します。

### キースイッチのはんだ付け

ここの二つのキースイッチは足がPro Microと干渉するので短く切ります。
![](img/IMG_1852.jpeg)  
差し込んだ状態で短く切りましょう。
![](img/IMG_1859.jpeg)  
Choc V2の場合は3本の足を、Choc V1では2本の足と固定用ピンの一つを短くします。
![](img/IMG_1145.jpg)  
![](img/IMG_1148.jpg)  
全てのスイッチをはんだ付けします。　　
![](img/IMG_1860.jpeg)  



### Pro Microのはんだ付け
隠れてしまうダイオードD3,D4の方向が合っているか、キースイッチの足がはんだ付けされているかを再度確認してください。  
足をニッパーで切ったらはんだ付けします。
![](img/IMG_1874.jpeg)  
![](img/IMG_1878.jpeg)  


### 動作テスト
ロータリーエンコーダーを取り付ける前にPro Microに動作ソフト（ファームウェア）を書き込んで動作確認をしましょう。  
キットとPCをUSBケーブルでつないでください。   

下のwebサイトにアクセスしてください。
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

テストファームウェアを選んでFLASHします。
![](img/remap02.jpg)  
![](img/remap03.jpg)  

キットのリセットスイッチを押すとArduino Microが現れるので、クリックして接続します（初回のみリセットスイッチを2回押す必要があることがあります）。
![](img/remap04.jpg) 

書き込みが完了したらウィンドウを閉じて大丈夫です。
![](img/remap05.jpg) 

アドレスバーやテキストエディタを使ってすべてのスイッチが反応することを確かめてください。  

Remapを使ってファームウェアの更新ができない場合は、QMK Toolboxをお試しください。  
- [QMK Toolboxを使ったファームウェア更新方法](firmware.md)

### ロータリーエンコーダーのはんだ付け
表からホイール型のロータリーエンコーダーを取り付けます。  
ピンの位置を確認してツメを穴に差し込みます。  
![](img/IMG_1887.jpeg)  

ツメを穴に引っかけてからピンを穴に差し込みます。
ピンを曲げてしまわないように注意してください。
![](img/IMG_1895.jpeg)   

差し込めたらはんだ付けします。
![](img/IMG_1901.jpeg)   

表からダイヤル型のロータリーエンコーダーを取り付けて裏からはんだ付けします。
![](img/IMG_1904.jpeg)  
クリップの部分ははんだ付けしなくても構いません。  
![](img/IMG_1905.jpeg)  

お疲れ様でした。再び動作を確認して問題がなければはんだ付けは終了です。

## 組み立て
USBケーブルを抜いてプレートを組付けます。  
アクリルからは保護フィルムを剥がしてください。  

メインボードのネジ穴にスペーサー（短）をネジ（短）で取り付けてミドルプレート1（透明）を嵌めます。
![](img/IMG_1928.jpeg)   
ここの2箇所は表側はネジではなくスペーサー（中）で止めます。
![](img/IMG_1923.jpeg)  

ミドルプレート2とバックプレートをネジ（長）で止めます。
![](img/IMG_1937.jpeg)  
ゴム足も取り付けました。
![](img/IMG_1940.jpeg)  

表に保護プレートをネジ（中）で取り付けましょう。
![](img/IMG_1948.jpeg)  

キーキャップとノブをつけて完成です。  
![](img/IMG_1951.jpeg)  

先ほどと同様の手順で本番用のファームウェアに更新しましょう。  
- https://remap-keys.app/catalog/OkZxVBzfCSGxdg48cNL2/firmware

![](img/remap06.jpg)  

## キーのカスタマイズ
標準では次のようなキー設定になっています。  
![](img/keymap.png)  

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
- [cannonball.json](https://github.com/Taro-Hayashi/Cannonball/releases/download/0.20.7/cannonball.json)  

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
