# レビュー

## PRの略語

`Q` : 質問されている。その質問の背景も添えると優しいが単に知りたいなら端的に

`MUST` : 必ず直す。理由も添える

`IMO` : In my opinionの略。マストではないのでマージしてもokだが、コメントには答えること

`Nit` : nitpick。細かい指摘。typoや書き方、スタイル、変数名など。MUSTではないのでapproveできるが、修正した方が学習になると思います

## コミットメッセージ

[ref](https://twitter.com/terrace_tech/status/1332491058744233984?s=20)

## お作法

[参照](https://zenn.dev/keitakn/articles/github-code-review-reviewee)

ここに書いてあるとおり、できるだけ軽減していただけるようお願いします(これは普通に現場でのお作法に近い)

- 個別説明が必要な箇所はコメントをつける
- 修正内容のコミットIDをリンクで伝える
- レビュアーに重点的にチェックして欲しい点
- その他の情報
↑該当リンク内のやつ
↓追加で欲しいやつ
- 問題へのリンク
- codesandboxのリンク(できたらして欲しい)

## PRの出し方

[【もりけん塾】GitHubでコードレビューを受けるときのお作法まとめ](https://happy-making.com/github-review/)

[実際の出しているページ](https://github.com/haru-programming/JavaScript-lessons/pull/6)

このように

```txt
Issue No.6. // 問題番号
-> Resolve the DOM created by Promise in 3 secontxt

CodeSandBox // codesandboxへのリンク
:Latest Commit adb3fd4 // 最新のコミットメッセージ。codeSandboxがそれを反映していることを確認してください。そのためのものです

// 実装していて困っていることやちょっとうまくいってないこと、疑問など
Concerns and areas to focus on
After creating an instance with new Promise, is it hard to see the Arrow function overlapping?
I have a feeling there is a better way to write this, but I couldn't get to it.
```


## レビュー方法

レビューをする側

- 塾生なら誰でも良いです
- 気になったこと疑問、なんでも書いてみてください

レビューを受ける際にして欲しいこと

1. 何かgithubのプルリクリンクかcodeSandboxのリンクを投稿してください
2. 恐らく誰か別の方が見てくれます
3. 指摘頂いたり学んだら(Twitter上でメンション付きで感謝とか、フィードバック)あげてください(レビュワーはあなたのために時間を割いてくれています)
4. 指摘をもらってしばらく放置、何週間後に出してくるは極力やめたいです。わからない場合は聞く。

※PR内のコメントに関して補足や間違ってそうな指摘には気づいたら自分が横から入りますね。自信がない場合は github内のコメントのリンク をここに貼ってください


課題に関して
- 1問終わったら次の1問に進むようにしてください。
理由は連続した例えば1問目、2問目としてPRを出してしまうと1問目で修正をもらってしまうと2問目でも同じ修正をしなくてはならないケースが多いからです。まずは1問目のLGTMを目指してください
