# **Deploy my VUI**

## **information**
- [about](https://thkkvui.github.io/about)
- [twitter (https://twitter.com/thkkvui)](https://twitter.com/thkkvui)


## **categories**
- 音声AIの選択
- 音声AIのtraining
- 音声AIのテスト
- イベントプログラムの構築
- 音声AIとイベントプログラムのリンク



## **Main Theme 「条件付きイベント処理に特化した音声AIの活用法」について**

「条件付きイベント処理に特化した音声AIの活用法」というテーマは、私が音声AIの使用中に感じた "発声の窮屈さ" が原点となっている。ホームデバイスでもスマートフォンでも実際に試すとお分かり頂けると思うが、「声を出すのは気が引ける」「声を出すと迷惑になる」「騒々しい場所で声が通らない」「プライベートな内容だから声に出したくない」などの場面では、機能の利便性に関係なく音声操作を躊躇することがある。この声の難点とも言うべき心理が、私にはデバイス使用以前の問題に思えてならなかった。

例えば、「音楽を再生して」「レシピを検索して」「メッセージを送信して」などの音声処理は、「離れた場所からまたは手が離せない状況から」「少ない発声回数で」「何時でも安定して」という利点が融合すると手動操作に勝る価値を生む。しかし、通勤・オフィス・家などの日常時間では上記のような "発声の窮屈さ" が常に存在するため、あるタイミングで「便利だけど、今はいいや、自分でやるから」という負の価値が生まれる。そこからはユーザーの行動によるが、長年培ってきた手動操作の利便性が再認識された場合、音声AIを使用する意欲は次第に消えてしまう。

普段使いを目指すはずのテクノロジーも、その状況1つで使用が躊躇されるようでは良いUXが得られるはずがない。何か別の道筋を立て、人間心理と効用のバランスを図る必要があるはずだ。この取り組みでは、その糸口を掴みたいと考えている。


では、具体的にどのような方法が良いか。ここでは電車の経路検索を例に考えてみたい。

①　今日は「18時に子供の迎え」がある。出先での仕事終了後に経路検索したが、電車の遅延により18時には間に合わないことが判明した。迎え先に遅刻の連絡を入れ、子供には可哀想だが待ってもらうことにした。

②　今日は「18時に子供の迎え」があると、家を出る前に音声AIへ伝えておいた。出先での仕事中、音声AIから「電車が遅延しています。到着に遅れる可能性があります。」と通知が来た。添付されていた迂回経路に乗車するため仕事を早く切り上げたお陰で、何とか遅刻せず迎えに到着することができた。

　①は通常の経路検索、②は音声AIを使った仮想の応用例を示している。②の音声AIには、電車の遅延情報と現在の位置情報から迎えの到着に遅れることを検知した場合、ユーザーに注意喚起する機能が搭載されている。②の例では遅刻可能性への言及のみだが、「お迎え先に連絡しますか？」「他に頼める方へ連絡しますか？」としてもよい。

　この場合、音声AIはハンズフリー操作の媒体ではなく、ユーザーのイベントを事前に"学習"する頭脳として機能することが重要なポイントである。学習のタイミングは②では出発前としたが、実際は "発声の窮屈さ" を極力感じないタイミングをユーザーが自由に選択すればよい。そして、「子供の迎えに遅れる」というイベントが発生しそうな場合にだけプログラムが起動し、イベントの通知、経路検索、代替手段の提示によりユーザーの手間を省いている。

　音声AIの利便性は通常の日常でこそ発揮されるべきなのだが、ハンズフリー操作を主眼に置くことは（少なくとも私には）適当ではない。それならば、音声AIを "ユーザー学習" の頭脳に見立て、手動対応が難しい少し複雑なイベント処理に活用する方法なら、心理と効用のバランスを図ることができないか？・・・というのが、このアイデアである。


　"ユーザー学習" という分野も今やテクノロジーの範疇であるが、その分析プロセスには文字、数字、画像などの情報が選好されやすいと考えている。なぜなら、それらと音声データではAIによる解読精度や実務上の取り扱いについて、現状では明確な差があるからだ。日常イベントの有無だけを確認したいなら、既存のカレンダーやリマインダー（つまり、文字や数字などのテキストデータ）の読み取りでも十分である。

　しかし今回の場合は、音声データを選好したい明確な理由がある。情報不足による利便性の低下を回避するためだ。音声AIへの呼び掛けは言い換えれば依頼と同様であり、依頼の実行にはより詳細なユーザーの意向が必要となる。つまり、既存のカレンダーやリマインダーのような自分専用、もしくは共有されても困らない程度の情報量では、音声AIが正しく機能しない可能性がある。

「今日は18時に子供の迎えがあるから、遅刻しそうな場合は早めに教えてくれる？」
「今日は18時に子供の迎えがあるんだけど、30分前には最寄駅に着きたいから、遅刻しそうな場合は早めに教えてくれる？

　また、↑↑のようなイベント（今日、18時、子供の迎え）、条件（遅刻、30分前に最寄駅、早めに）、アクション（教えてくれる？）などの内容を数秒で伝達できることは音声inputの強みであり、この手軽さや速さは手動inputでは到底叶わない。ユーザーは誰かにお願いするように音声AIを使うだけで、情報は音声AIの中に格納され、"もしもの時" のイベント処理に使用されるという構図だ。

　音声AIと音声データ。その学問的な奥深さや利便性追求の余地から考えると、誰もその究極形に到達していないことは明らかであり、私の興味を惹く1つの理由になっている。一連の想定を具体化することは、私にとって既存の活用法では得られない音声AIの効用を見出す第一歩となる。先ずは音声AIに日常の "見張り役" としての地位を確立させ、手動でやること、音声でやることの棲み分けを明確にしていきたいと考えている。


## **recent posts**
- [2022-04-26]
- [2022-04-22](https://github.com/thkkvui/thkkvui.github.io/2022/04/22/first_post.html) 初投稿


## **GitHub Pages**
- This page was generated by GitHub Pages.
  - [GitHub Pages (https://pages.github.com)](https://pages.github.com)
- The theme of this page is "Cayman theme".
  - [Cayman theme (https://github.com/pages-themes/cayman)](https://github.com/pages-themes/cayman)
