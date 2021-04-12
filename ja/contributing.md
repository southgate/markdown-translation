差出人: https://github.com/facebook/chef-cookbooks/edit/master/CONTRIBUTING.md

# フェイスブックのシェフクックブックに貢献

## テスト マークダウン

~~ここでは~~、gitHub風味のマークダウンテストをいくつか@southgate。

:その後: | :ok_hand: | :眉をひそめ: |
---------|----------|----------|
巨大なおめでとうございます  | おめでとう数を減 | おめでとうございます

- [ ] タスク 1
- [ ] タスク 2
- [ ] タスク 3

## 当社の開発プロセス
このリポジトリは内部リポジトリから同期されます。私たちは絶対にプルを受け入れます
を要求し、適切にマージを処理します。

シェフの正しさのテストにはFoodcritic、ルビースタイルにはルボコップを使用しています
糸くず。ルールセットは、内部と外部の両方で同期され、確実に
すべての人に一貫したコード品質とスタイルを提供します。

## 共同作成者ライセンス契約 ("CLA")
プルリクエストを受け入れるには、CLAを提出する必要があります。必要なのは
これを一度行って、Facebookのオープンソースプロジェクトで作業します。

ここでCLAを完了してください: <https://code.facebook.com/cla>

## 前提条件
まず、貢献に興味を持っていただきありがとうございます、私たちはプルリクエストを歓迎します!

このレポにプルリクエストを送信する前に、このレポを忘れないようにしてください。
属性駆動型 API は他のコミュニティとは非常に異なるモデルです。
料理。そのモデルを構築するために、料理本が必要とする特定の方法があります
書き込まれます。

を必ずお読み下りすることを強くお勧めします。 [README.md](README.md)
[Philosphy.md](https://github.com/facebook/chef-utils/blob/master/Philosophy.md).
また、Runlist の順序を使用する環境をセットアップすることをお勧めします。
(コアクックブックが最初に、その後の他のすべて)。

最後に、3 段階のアプローチに従ってください。

 * `attributes/` ファイルは API をセットアップし、他のクックブックの属性には触れません。
 * `recipes/` ファイルセットアップリソース (テンプレートやサービスなど)
   API (読み取り: 他のクックブックの属性を設定する)
 * 属性は( `runtime`別名)でのみ消費されます`converge time`。
   たとえば`templates`、 、 `ruby_blocks` 、 、 `whyrun_safe_ruby_blocks`、
   `providers`.

## 問題
GitHub の問題を使用して、パブリックバグを追跡します。あなたの説明が
問題を再現するための十分な指示があります。

フェイスブックは [バウンティプログラム](https://www.facebook.com/whitehat/) 金庫用を持っている
セキュリティバグの開示。そのような場合は、プロセスを経てください
そのページに概説され、公開問題を提出しないでください。

## プル要求の送信

修正または機能をお持ちですか?すごい！プルリクエストを送信する際に、お客様に推奨
適用可能なシェフランの出力を含めます。

新しい API (属性) の場合は、適切な API に記載されていることを確認してください。
料理本の読み取り。

私たちは、同じ品質とスタイルの基準にすべての貢献を保持します。
既存のコード。


### 新しいクックブック

私たちは、ベースを管理する「コア」料理本に焦点を当てて、このレポを維持したいと思います
OS。このような料理本を投稿したい場合は、最初から
重複する努力を避けるために最初に問題を提出する(私たちはできる問題を持っているかもしれません
オープンソースを試みるか、他の人が1つを書いているかもしれません)に取り組む前に。

そのカテゴリに該当しない料理本を投稿したい場合(例えば.
デスクトップの事やその他のサービスを管理する)、その後、PRを参照してください。
あなたがそれを維持したいと思うレポで、私たちはそれを見直して追加させて喜んで行います
私たちの中であなたのレポへのポインタ
[UNIVERSE.md](https://github.com/facebook/chef-cookbooks/blob/master/UNIVERSE.md)
ファイルを表示します。

 私たちは、 `fb_` フィットする料理本を示すために接頭辞を使用します
このモデルとこのレポから来ているが、他の場所で料理本を出版すること自由に感じる
このモデルを平均化し、他の接頭辞を使用します。

## ライセンス
このリポジトリに貢献することで、あなたの貢献は
Apache 2.0 ライセンスの下でライセンスされています。