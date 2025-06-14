---
tags:
  - "#自作PC"
  - "#PC"
  - "#ゲーミング"
  - "#アリエクスプレス"
  - "#PCパーツ"
  - "#leverless-controller"
  - "#diy-electronics"
  - "#arcade-stick"
  - "#gp2040-ce"
---
# 【DIY】4000円から始める「レバーレスアケコン」入門【hitBOX】

この記事では、格ゲー初心者やなるべく低予算でレバーレスを使いたいユーザーに向けて、レバーレスを安価に自作するメリットについて紹介する。

---

レバーレスは従来のアケコンに比べコマンド操作が圧倒的にしやすく、プロゲーマーにも愛用者が多い。機構もシンプルでメンテナンス性に優れるため、ボタンレイアウトやデザインを自分なりにカスタマイズできるのも特徴である。

-   話題のレバーレスを触ってみたい
-   なるべく安く手に入れたい
-   在庫切れでレバーレスがなかなか手に入らない
-   そもそも使いこなせるか不安

上記のような悩みがある方には、ぜひ自作レバーレスをおすすめしたい。必要なのは4,000円と気合いのみ。hitBOXの1/10の価格で実用性も十分な自作レバーレスの魅力について語っていく。

## レバーレスがなかなか手に入らない

「ストリートファイター6」は、大規模な大会が開催され配信者やその視聴者を巻き込んでブームとなっている。ストリーマーやプロの多くがhitBOXをはじめとしたレバーレスコントローラーの使用を公言している事もあり、世界中で品薄が続いているような状況だ。
品薄はもちろん、価格の高さも入手しにくい要因となっている。レバーレスの代表格である「hitBOX」は、定価で約40,000円という強気な価格設定である。

![hitBOX製品画像](https://sheklog.com/wp/wp-content/uploads/2023/07/hitBOX002-1.webp)

もちろん価格に見合うだけの性能・品質を有しているのは確かだが、アマチュアゲーマー、それも初心者が気軽に購入できる値段ではない。
需要の高まりを受けてか、最近では中国製の購入しやすい価格帯の「hitBOX型のレバーレス」も多数登場している。以前より入手しやすい状態にはなってきているものの、安くて使いやすいモデルは軒並み品切れである。

[https://amzn.to/3XCslyX](https://amzn.to/3XCslyX)

さまざまなメディアやプロゲーマーに立て続けに紹介された影響もあり、欲しい人でもなかなか手に入らない状況が続いている。

## レバーレス自作のススメ

レバーレスコントローラーが入手しにくい状況を受け、最近では自作するユーザーが増えている。
実はレバーレスコンの構造は従来のアケコンに比べシンプルなので工作難度は低めである。さらに、自作するための情報が豊富であること、パーツの単価が安いこと、ファームウェア導入が簡単なことも追い風となり、挑戦するメリットは大きい。

自作のメリット
-   **確実に手に入る**
-   **既製品より圧倒的に安価**
-   **ボタンレイアウトも自由自在**
-   **壊れても自力で直せる**
-   **薄型で取り回しやすい**

完成するまでに結構な時間が必要だが、1日もあれば完成するレベルではある。パーツ集めはそれなりに時間が掛かるが、**安さは何にも変え難いメリット**だ。

## 製作に必要なモノと予算

コントローラーとして動作させるには以下の表のパーツが必要となる。点数は少なく単価も安いので、ある程度品質に拘ったとしても10,000円以内には収まるだろう。
ちなみに今回僕がレバーレス製作にかけた金額の内訳は以下の通りである。

| パーツ                        | 金額                               | 備考                                                                                                                                                                                    |
| :------------------------- | :------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Raspberry pi pico          | 750円                             | Aliexpressで購入。時間は掛かるが安い。<br>https://ja.aliexpress.com/item/1005003928558306.html?spm=a2g0o.order_list.order_list_main.92.59c6585athG1RZ&gatewayAdapt=glo2jpn                          |
| Kailh ロープロファイルスイッチ         | 2,310円                           | 35個入。今回は18個使用。Gateron製製ならもう少し安い                                                                                                                                                                         |
| ケース（3Dプリンタ製）               | 0円（フィラメントは1kg 2,500円、消費量は150g程度） | 以下のモデルを使用。<br>https://www.thingiverse.com/thing:5302951<br>製作者様の記事はこちら。より詳細な作成手順について触れられている。<br>https://okayu-moka.hatenablog.com/entry/2022/03/12/181155?utm_source=pocket_saves<br> |
| はんだ（精密機器用）                 | 200円                             |                                                                                                                                                                                       |
| 半田ごて                       | 700円                             | 可能なら3,000〜4,000円位のちゃんとしたモデルがオススメ                                                                                                                                                      |
| エナメル線                      | 500円くらい                          |                                                                                                                                                                                       |
| キーキャップ（3Dプリンタ製）            | 0円                               |                                                                                                                                                                                       |
| ネジ（M3.5 12mmx8、M2.3 6mmx4） | 300円                             |                                                                                                                                                                                       |
| 合計                         | **約4,000円**                          |                                                                                                                                                                                       |

道具を一から揃えたとしてもこの価格である。必要な道具が手元にあるなら更に安く製作できる。また、ハンダやエナメル線などがかなり余るため、キースイッチさえ追加購入すれば、もう1,2台製作することも可能だ。

## なぜ安い？コストを抑えるコツ

安く済んだ要因としては**3Dプリンタの有無がかなり大きい**。外部に依頼すると追加で2,000〜3,000円程度の出費は避けられない（その分品質は良いはずだが）が、一般的なご家庭にある3Dプリンタでプリントすればわずかなフィラメント代と電気代しかかからない。

難しい場合は「DMM.make」などの外部プリントサービスに依頼することを推奨する。
[https://make.dmm.com/public/print/corporation/2_a_ad/?gad=1&gclid=Cj0KCQjwwISlBhD6ARIsAESAmp6AmeQocIwmb4YMo0oMRZRt71ZxlbJnK7sbEIaDN53Ru0WcuEpqtrwaAvlEEALw_wcB](https://make.dmm.com/public/print/corporation/2_a_ad/?gad=1&gclid=Cj0KCQjwwISlBhD6ARIsAESAmp6AmeQocIwmb4YMo0oMRZRt71ZxlbJnK7sbEIaDN53Ru0WcuEpqtrwaAvlEEALw_wcB)

また、「Raspberry pi pico」より安いRP2040互換機に変更することで、500円程度出費を抑えた。
互換機はアリエクで買える下記のモデルがオススメである。USBType-C搭載で、ピン配列も同じ。300円で買えるコスパの高さも魅力だ。[^1]

RP2040コアボードTYPE-C USB-CラズベリーコアボードRP2ラズベリーパイピコmicropython
[https://a.aliexpress.com/_mqiYuco](https://a.aliexpress.com/_mqiYuco)


プリント基板（PCB）を使用しないモデルを選択したのもコストを抑えるため。配線の手間はあるが、動作に影響はない。

キースイッチもGateron製のものに変更すれば、さらに500円程度安く抑えられる。

参考程度に市販のレバーレスと価格を比較してみる。

| 製品名                 | 価格      |
| :--------------------- | :-------- |
| hitBOX                 | 39,600円  |
| PUNKWORSHOP レバーレス | 22,359円〜 |
| Victrix Pro FS-12      | 52,468円  |
| Truboost B1-PC         | 13,000円  |

自作なら不具合が発生しても制作時の道具と余ったパーツで修理も可能でメンテナンス製も高い。そういった意味でも**自作のコスパは圧倒的**と言えそうだ。

## 製作時の最大の障壁について

一見難しそうに感じるが、**作業はとてもシンプル**である。

1.  BOOTボタンを押しながらPCと接続
2.  オープンソースのゲームパッドファームウェアである「GP2040-CE」をインストール
3.  ひたすらハンダ付け

手順1,2で「Raspberry pi pico」がアケコン基板として認識されるので、あとは下記の配線図を見ながら、ボタンと基板をハンダ付けするだけである。
[https://gp2040-ce.info/#/](https://gp2040-ce.info/#/)

このようにハンダ付けのスキルとほんのわずかのPCスキルさえあれば、誰でも簡単に自作できる。半田ごてで火傷しないよう気を付ければ大丈夫だ。
[https://togetter.com/li/1249146](https://togetter.com/li/1249146)

## 多少面倒でも手に入れる価値がある

SF6ならモダン操作もあるし、コントローラーを使うプロだって沢山いる。別にレバーレスなんて必要なくない？という意見は最もだが、レバーレスの魅力はなにも素早い入力操作だけではない。
モダン操作よりできる事も多いし、なにより**格ゲーしてる感が凄い**。コレに尽きる。

![自作レバーレスコントローラー完成品](https://sheklog.com/wp/wp-content/uploads/2023/07/hitBOX003-1-scaled.jpeg)

初心者が最速でランクを上げるならコントローラーとモダン操作がベストだけれど、勝ち負けだけでなく格ゲーならではの操作感や雰囲気を楽しみたいなら、一度レバーレスに触れてみることをオススメしたい。数千円で手に入るのだから。

## まとめ
レバーレスコントローラーに興味はあるけれど、価格や入手困難さで諦めていたあなたへ。自作という選択肢は、その悩みを解決する素晴らしい方法である。

本記事で紹介したように、**数千円の予算と少しの時間、そして「作ってみたい！」という気持ちがあれば、誰でも自分だけのレバーレスアケコンを手に入れることができる**。完成した時の達成感、そして自分の手で作り上げたコントローラーで勝利を掴む喜びは格別である。

もちろん、最初は戸惑うこともあるかもしれない。しかし、情報を集め、一つ一つの工程をクリアしていく過程もまた、DIYの醍醐味である。この記事が、あなたの挑戦を後押しするきっかけになれば、これほど嬉しいことはない。

さあ、あなたもレバーレス自作の世界へ飛び込んでみてはどうだろうか。

---
[^1]: ネジ穴がないので固定には工夫が必要である。プリント基板取り付け台を利用したり、グルーガンで接着するなど、工夫するとよい。[https://eleshop.jp/shop/g/gF29121/](https://eleshop.jp/shop/g/gF29121/)