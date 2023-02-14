# OmochiDAOへの参加方法

## ウォレットの準備 
まず、デスクトップ端末にBraveをインストールしてください。

[https://brave.com/download](https://brave.com/download)

次に、こちらのヘルプページの手順でBrave Walletを作成してください。

[https://support.brave.com/hc/en-us/articles/4413909784205](https://support.brave.com/hc/en-us/articles/4413909784205)

【勉強会参加者の方へ】ウォレットを作成したら、ウォレットアドレスをBrave Talkのチャット欄に投稿してください。ハンズオンで必要となるトークン(mch)をお送りします。ちなみにテストネットなので資産価値はゼロです。ご安心ください。
![wallet1](img/wallet_01.png)

## Brave Walletの設定(Mumbaiネットワークの追加)
Omochi DAOは<span style="color: #ff0000;">Polygon</span>の<span style="color: #ff0000;">テストネット</span>である<span style="color: #ff0000;">Mumbai</span>を使用するため、設定の確認が必要です。

Braveのアドレスバーに

brave://settings/wallet/networks

と入力し、設定画面を表示させます。「<span style="color: #ff0000;">Ethereumネットワーク</span>」の右の［追加］を押下してください。
![setting](img/setting_02.png)

「ネットワークを検索」で "mumbai" と入力し、表示された項目を選択します。
![setting](img/setting_03.png)

必要な設定が自動入力されますので、画面を下にスクロールし、［送信］を押下します。
![setting](img/setting_04.png)

## Brave Walletの設定(MCHトークンの表示設定)
勉強会で使用するOMOCHI(MCH)トークンは、この勉強会でしか使用されないため、ウォレットに表示させるための設定が必要です。

Braveのアドレスバーに

brave://wallet/crypto/portfolio/add-asset

と入力し、「カスタムアセットを追加」をクリックします。

![setting](img/setting_06.png)

それぞれの項目は以下の通り設定します。

■ネットワークを選択  
Mumbai

■トークン名  
OMOCHI

■トークンアドレス  
0xC279D3E2A1E7A585F0Cb42A593327cEd909FdA86

■トークンシンボル  
MCH

小数点桁数  
18

![setting](img/setting_07.png)

［追加］ボタンを押下すると、OMOCHIトークンが表示されます！

![setting](img/setting_08.png)

## Brave Walletの設定(ロックされるまでの時間)

そのほか、

brave://settings/wallet

で、ウォレットがロックされるまでの時間を30分程度に設定することを推奨します。

![setting](img/setting_05.png)

## <span style="color: #ff0000;">ガス代</span>で使用する<span style="color: #ff0000;">maticトークン</span>の取得
[https://faucet.polygon.technology/](https://faucet.polygon.technology/)にアクセスし、ウォレットアドレスを入力して［Submit］を押下してください。
![setting](img/gas_01.png)

確認画面が表示されたら［Confirm］を押下します。
![setting](img/gas_02.png)

この画面が表示されたら作業は完了です。
![setting](img/gas_03.png)

1,2分経つと、ウォレットにmaticが送金されたことが確認できます。おそらく0.2maticが振り込まれたと思います。ちなみに、何度もmaticをもらおうとするとサイトでエラーになるのでご注意ください。
![setting](img/gas_04.png)

## Aragonにアクセス

[https://client.aragon.org/](https://client.aragon.org/)にアクセスします。
まず、ネットワーク設定をMumbaiにセットします。
![ara1](img/aragon_01.png)
![ara2](img/aragon_02.png)

次にウォレット接続を行います。

![ara3](img/aragon_03.png)
![ara4](img/aragon_04.png)
![wallet2](img/wallet_02.png)

それではDAOに入りましょう！

![ara5](img/aragon_05.png)
![ara6](img/aragon_06.png)
![ara7](img/aragon_07.png)

"Loading App" の表示がなかなか消えないときは、Brave Shieldsを一度無効にしてみてください。画面が表示されたら有効に戻して問題ありません。
![ara8](img/aragon_08.png)