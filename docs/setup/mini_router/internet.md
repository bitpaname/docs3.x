# ネットワーク

インターネットへの接続方法は**有線接続**、**無線中継**、**3G/4Gモデム**、**テザリング**の4つから選択できます。

![connection method](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/モード.jpg)



インターネットへの接続を行うには、管理パネル左の`「ネットワーク」`をクリックします。

![internet](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/ネットワーク.png)

  

---

## 1. 有線接続

モデムまたはメインのルーターを介してルーターをインターネットに接続します。

EthernetケーブルをルーターのWANポートに接続する前に、`LANポートとして使用` をクリックして、WANポートをLANポートに変更することができます。ルーターを無線中継に利用する際に、もう一つのLANポートを利用できるようになります。

![cable](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/ケーブル.png)



EthernetケーブルをルーターのWANポートに接続します。接続情報が`有線`セクションに表示されます。デフォルトのプロトコルはDHCPで、`修正`をクリックしてプロトコルを変更できます。

![cable](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/ケーブルセクション.png)



### DHCP

DHCPはデフォルトで一般的なプロトコルです。手動で設定する必要はありません。

![dhcp](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/デフォルトプロトコル.png)



### Static

インターネットサービスプロバイダ(ISP)が固定のIPアドレスを提供しているか、IPアドレス/ゲートウェイ/サブネットマスクなどの情報を手動で設定したい場合には`Static`を選択します。

`Static`を選択すると現在の設定内容が自動で入力されます。設定内容を入力し、`応用する`をクリックしてください。

![static](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/せいたい.png)



### PPPoE

PPPoEは多くのインターネットサービスプロバイダ(ISP)で要求されます。
一般に、ISPからはインターネットへの接続に必要なモデムとユーザー名・パスワードが提供されます。

`PPPoE`を選択し、ユーザー名とパスワードを入力して`応用する`をクリックします。

![PPPoE](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/PPPoE.png)



---

## 2. 無線中継

`無線中継`はルーターをホテルや喫茶店のフリーWi-Fiのような他の無線ネットワークに接続することです。

ルーターはデフォルトでWISP(Wireless Internet Service Provider)モードを使用します。このモードではサブネットを作成し、ファイアウォールとして公衆ネットワークからあなたを保護します。

`中継`セクションで、`スキャン`をクリックして近くの無線ネットワークを検索します。

![repeater scan](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/中継.png)



ドロップダウンリストからSSIDを選択し、パスワードを入力します。**ネットワークを保存**を有効にすると、現在選択しているネットワークの情報が保存されます。最後に、`添加する`をクリックします。


![connect wifi](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/中継スキャン.png)



---

## 3. USB 3G/4Gモデム

USB 3G/4Gモデムを使ってインターネットに接続することができます。SIMカードをUSBモデムに挿入し、USBモデムをルーターのUSBポートに接続します。USBモデムが検出されると`3G/4G無線ネットモジュール`セクションが有効になり、USBモデムを設定できるようになります。

一部のモデムはホストレスモードで動作することに注意してください。これは、3G/4Gモデムモードではなく、テザリングを通じて設定されます。

一般に、あなたは以下の3つの基本パラメータで3G/4Gモデムを設定します。`応用する` をクリックして続きます。

- **デバイス**：モデムがQMIをサポートする場合は、**/dev/cdc-wdm0**を選択してください。 そうでなければ **/dev/ttyUSB**を選択する必要があります。**/dev/ttyUSB**には0から3までがあり、モデムの仕様に合ったものを選択する必要があります。最初に**ttyUSB0**を試してください。
- **サービス**：SIMカードのサービスタイプを示します。
- **APN**：SIMカードを提供している事業者に確認してください。

![modem](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/3G4G.png)

高度な設定：

- **ナンバー**：通常、この欄はデフォルト値であり手動での設定は必要ありません。この情報を有している場合に限り入力してください。
- **PINコード、ユーザー名、パスワード**：ロックされていないSIMカードではこれらの値は必要ありません。SIMカードがロックされている場合は事業者に問い合わせてください。

![modem](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/3G4Gセット.png)



IPアドレスが表示されていれば接続は完了しています。

![modem connect](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/modem2.jpg)

![modem connected](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/modem3.jpg)



### 動作確認済みのモデム

以下はテストにより動作が確認されているモデムの一覧です。

| 型番                                  | 3G/4G | テスト済み | テスト実施者       | コメント* |
| -------------------------------------- | ----- | ------ | --------------- | --------- |
| Quectel EC20-E, EC20-A, EC20-C         | 4G    | はい    | GL.iNet         |           |
| Quectel EC25-E, EC25-A, EC25-V, EC25-C | 4G    | はい    | GL.iNet         |           |
| Quectel UC20-E                         | 3G    | はい    | GL.iNet         |           |
| ZTE ME909s-821                         | 4G    | はい    | GL.iNet         |           |
| Huawei E1550                           | 3G    | はい    | GL.iNet         |           |
| Huawei E3276                          | 4G    | はい    | GL.iNet         |           |
| TP-Link MA260                          | 3G    | はい    | GL.iNet         |           |
| ZTE M823                               | 4G    | はい    | Arnas Risqianto |           |
| ZTE MF190                              | 3G    | はい    | Arnas Risqianto |           |
| Huawei E3372                           | 4G    | はい    | anonymous       |           |
| Pantech UML290VW (Verizon)             | 4G    | はい    | GL.iNet/steven  | QMI       |
| Pantech UML295 (Verizon)               | 4G    | はい    | GL.iNet/steven  | ホストレス |
| Novatel USB551L (Verizon)              | 4G    | はい    | GL.iNet/steven  | QMI       |
| Verizon U620L (Verizon)                | 4G    | はい   |                 | ホストレス |
|                                        |       |        |                 |           |

*QMI: このモデムはQMIモードをサポートしています。**デバイス**リストで **/dev/cdc-wdm0** を選択してください。

*ホストレスモード: このモデムはテザリングモードをサポートしています。「3G/4Gモデム」ではなく、「テザリング」を使って設定してください。

 対応するモデムについては[http://ofmodemsandmen.com/supported.html](http://ofmodemsandmen.com/supported.html)も参考にしてください。



---

## 4.テザリング

「テザリング」は、スマートフォンからルーターにUSBケーブルでネットワークを共有することです。ホストレスモードをサポートするモデムも「テザリング」で利用します。

ホストレスモデムでテザリングを行う場合は、モデムをルーターのUSBポートに接続します。

スマートフォンでテザリングを行う場合は、スマートフォンをUSBケーブルでルーターのUSBポートに接続し、スマートフォンで**信頼する**を選択します。

デバイスを接続すると`テザリング`セクションが更新され、接続したデバイスがリストに表示されます。デバイスの名は**eth2**、**usb0**のように**eth**または**usb**で始まります。 お使いのデバイスを選択して`接続`をクリックしてください。

![tethering](https://static.gl-inet.com/docs/jp/3/setup/mini_router/internet/テザリング.png)



### EasyTether

一部の通信事業者は、テザリングを使用できないようにデータの共有を禁止しています。 しかし、あなたはEasytetheringを試すことができます。

*注意： EasyTetherは無料のサービスではなく、私たちは彼らと提携していません。*
