# GL.iNetトラベルルーターを使い始めます

モデム:

GL-MT300N, GL-MT300N-V2 

GL-AR150, GL-AR150-PoE, GL-AR150-Ext-2, GL-AR150-Ext-PoE-2

GL-AR300M, GL-AR300M-Ext, GL-AR300M16, GL-AR300M16-Ext, GL-AR300M-Lite

![router](https://static.gl-inet.com/docs/jp/3/setup/mini_router/first-time_setup/構造.jpg)

*注意：**GL-AR300M-Lite** のEthernetポートは1基のみです。*

---

## 1.電源を入れます

Micro USB電源ケーブルを電源ポートに接続します。
標準の5V/1A電源アダプタを使用していることを確認してください。サポートされていない電源の使用は故障の原因となる場合があります。

![Power on](https://static.gl-inet.com/docs/jp/3/setup/mini_router/first-time_setup/power.jpg)

## 2.接続 

ルーターにはEthernet又はWi-Fiで接続することができます。

*注意：この手順では、デバイスをルーターのローカルエリアネットワーク（LAN）に接続します。あなたは現在インターネットにアクセスすることはできません。インターネットに接続するには、以下の設定手順を完了して、[ネットワーク](internet.md)に従ってインターネット接続を設定してください。



### LANで接続
ルーターのLANポートにEthernetケーブルであなたのデバイスを接続します。

![connect via lan](https://static.gl-inet.com/docs/en/3/setup/mini_router/first-time_setup/connect.jpg)

*注意：**GL-AR300M-Lite**のEthernetポートは1基のみで、デフォルトではWANポートとして使用されます。ルーターを初めて設定する際はWi-Fiで接続することになります。Wi-Fiで接続した後に[「インターネット」](internet.md)からWANポートをLANポートに変更することで、Ethernetケーブルでデバイスを接続できるようになります。*



### WiFiで接続
デバイスでルーターのSSIDを探し、デフォルトパスワード ***goodlife*** を入力します。

*注意：SSIDはルーター底面のラベルに以下の形式で印刷されています：*

- **GL-AR150-XXX**

- **GL-AR300M-XXX**

- **GL-AR300M-XXX-NOR**




## 3.Web管理パネルをアクセスします

Webブラウザ(Firefox/Chrome推奨)を開いて、[http://192.168.8.1](http://192.168.8.1) にアクセスします。



### 1）言語設定
管理パネルで表示する言語を選択します。現在は**日本語**、**English**、**简体中文**、**繁體中文**、**Deutsch**、**Français**、**Español**がサポートされています。

![initial setup](https://static.gl-inet.com/docs/jp/3/setup/mini_router/first-time_setup/言語設定.png)

*Note: ブラウザが常にLuCI（http://192.168.8.1/cgi-bin/luci)にリダイレクトされる場合は、[http://192.168.8.1/index.html](http://192.168.8.1/index.html)にアクセスしてください*

  

### 2）管理者パスワード設定
管理パネルを開く際のパスワードは標準で設定されていないため、5文字以上のパスワードを設定する必要があります。

![password](https://static.gl-inet.com/docs/jp/3/setup/mini_router/first-time_setup/パスワード設定.png)

*注意：このパスワードは管理パネルまたは組み込みLinuxシステムのためのものです。Wi-Fiのパスワードは変更されません。*



### 3）管理パネル
初期設定が完了するとルーターの管理パネルが開きます。ルーターの状態を確認したり、設定を変更することができます。

![admin panel](https://static.gl-inet.com/docs/jp/3/setup/mini_router/first-time_setup/管理者パネル.png)
