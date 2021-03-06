thkkvuiのGithub Pagesへようこそ。

This is thkkvui Github Pages.

## **information**
- [about](https://thkkvui.github.io/about)
- [News](https://thkkvui.github.io/news)
- [twitter (https://twitter.com/thkkvui)](https://twitter.com/thkkvui)


## **project categories**
- [音声AIの選択](https://thkkvui.github.io/select)
- [音声AIのトレーニング](https://thkkvui.github.io/training)
- [音声AIのテスト](https://thkkvui.github.io/validation)
- [イベントプログラムの構築](https://thkkvui.github.io/event)
- [音声AIとイベントプログラムのリンク](https://thkkvui.github.io/linker)


## **recent posts**
1. [2022-04-22](https://thkkvui.github.io/2022/04/22/first-post.html) 初投稿
2. []
3. []
4. []
5. []
6. []
7. []
8. []
9. []
10. []

&emsp;

## **Main Theme**
## **「条件付きイベント処理に特化した音声AIの活用法」について**

&emsp;

　音声AIの使用には、"発声の窮屈さ" という副作用が伴う。「声を出すのは気が引ける」「声を出すと迷惑になる」「騒々しい場所で声が通らない」「プライベートな内容だから声に出したくない」という人間心理は、日常シーンにおける音声AIの浸透を阻む原因の一つではないだろうか。

　音声AIは、「離れた場所から、または手が離せない状況から」「少ない発声回数で」「ユーザーの好きなタイミングで」何かを操作できる、という複数利点の相乗効果が期待されている。しかし、先の人間心理が邪魔するとユーザーは音声AIの使用に敢えて拘らず、使い慣れた手動操作を選択する。「やっぱ手で操作した方が、早いし楽だな」と再認識したユーザー意識を再び音声AIに回帰させることは、個人的な経験を見る限り意外と難しい。

　普段使いを目指すはずのテクノロジーも、状況1つでその使用が躊躇されてしまう現実が存在する。音声AIの使用を良いUXへと繋げていくためには、ハンズフリー操作とは異なる利点を作り出す必要があるはずだ。

&emsp;

### **音声AIを "頭脳" に見立てる**

　以下の例を見てもらいたい。

①　今日は「18時に子供の迎え」がある。出先での仕事終了後に経路検索したが、電車の遅延により18時には間に合わないことが判明した。迎え先に遅刻の連絡を入れ、子供には可哀想だが待ってもらうことにした。

②　今日は「18時に子供の迎え」があると、家を出る前に音声AIへ伝えておいた。出先での仕事中、音声AIから「電車が遅延しています。到着に遅れる可能性があります。」と通知が来た。添付されていた迂回経路に乗車するため仕事を早く切り上げたお陰で、何とか遅刻せず迎えに到着することができた。

　①は通常の経路検索、②は音声AIを使った仮想の応用例を示している。②の音声AIには、電車の遅延情報と現在の位置情報から迎えの到着に遅れることを検知した場合、ユーザーに注意喚起する機能が搭載されている。②の例では遅刻可能性への言及のみだが、「お迎え先に連絡しますか？」「他に頼める方へ連絡しますか？」としてもよい。

　この例のポイントは、音声AIがハンズフリー操作の媒体ではなく、ユーザーのイベントを学習して処理する "頭脳" として機能する点にある。学習のタイミングは②では出発前としたが、実際は "発声の窮屈さ" を極力感じないタイミングをユーザーが自由に選択すればよい。そして、「子供の迎えに遅れる」というイベントが発生しそうな場合にだけプログラムが起動し、イベントの通知、経路検索、代替手段の提示によりユーザーの手間を省く。

　このように、音声AIの利便性を「手動対応が面倒で少し複雑なイベント処理に活用する」という別の道筋で捉える。そうすれば、人間心理と効用のバランスを図ることができないだろうか。これが、このプロジェクトの目的である。

&emsp;

### **AIとユーザーデータ**

　音声AIによるユーザー学習という分野は、特段目新しいものではない。ただ、ユーザー学習は文字、数字、画像などのデータが選好されやすく、音声はメインの分析対象とは言い難いだろう。AIによる解読精度、データ分析プロセス、プライバシーの保護など、実務上の取り扱いが少し異質な音声データにわざわざ手を伸ばさなくても、各種アプリやブラウザから取得できる従来のユーザー情報で十分と考える開発者は多いはずだ。

　しかし、このプロジェクトでは音声AIから効用の高いUXを引き出すという目的があるため、音声データに拘ったユーザー学習を前提とする。つまり、「手軽かつ迅速に情報をinputできる」「ユーザーが要約した言葉への理解力がある」という音声AIの既知の強みを生かしながら、学習とイベント処理を実現する追加機能を実装していくことになる。

- 「今日は18時に子供の迎えがあるから、遅刻しそうな場合は早めに教えてくれる？」
- 「今日は18時に子供の迎えがあるんだけど、30分前には最寄駅に着きたいから、遅刻しそうな場合は早めに教えてくれる？」

　これらは、前段②で想定した音声AIへのinput例である。ユーザーからinputされた内容を、イベント（今日、18時、子供の迎え）、条件（遅刻、30分前に最寄駅、早めに）、アクション（教えてくれる？）に細分化し、"もしもの時"のイベント処理に活用する。この一連の想定を具体化する・・・と言っても、そう簡単なものではなさそうだ。

&emsp;

　音声AIは長い歴史を持つテクノロジーであるが、その学問的な奥深さや利便性追求の余地から考えると、誰もその究極形に到達していないことは明らかであり、私の興味を惹く1つの理由になっている。このプロジェクトを通じて、僅かでもその成長に貢献できれば嬉しい限りである。

&emsp;

## **License**
-

&emsp;

## **GitHub Pages**
- This page was generated by [GitHub Pages (https://pages.github.com)](https://pages.github.com).
- This page's theme is [Cayman theme (https://github.com/pages-themes/cayman)](https://github.com/pages-themes/cayman).
