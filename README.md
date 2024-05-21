# Git Lesson

## リモートリポジトリとローカルリポジトリとはそれぞれ何でしょうか？

- リモートリポジトリはGitHub等のサービスによりネット上に配置され、複数人で共有するためのものです。
- ローカルリポジトリは自分のPC等のローカル環境に配置され、開発者一人ひとりが使用するためのものです。

## プッシュとマージの違いは何でしょうか？

- ローカルからリモートに変更内容を反映させるか、ローカル同士で変更履歴を反映させるかの違いです。
  - プッシュはローカルリポジトリからリモートリポジトリに変更内容を反映させること。
  - マージはローカルリポジトリ内のブランチの変更履歴を別のブランチに反映させること。

## コミットとプッシュの違い

- ローカルリポジトリ内で完結するかどうかです。
  - コミットはローカルリポジトリ内で変更履歴を残すこと。
  - プッシュはローカルリポジトリ内の変更履歴をリモートリポジトリに反映させること。

## コミットのメッセージはどのように書いてあげるのが最適でしょうか？

- 変更点を分かりやすく書くのが最適です。

## ローカルでマージするフローと、プルリクエストでマージするフローの違いは何でしょうか？

- マージされるローカルブランチに、変更内容を反映するタイミングが変わります。
  - ローカルでマージする場合、先にローカルに変更内容の反映を行った後、プッシュ等を行い、リモートに反映します。
  - プルリクエストでマージする場合、先にリモートに変更内容の反映を行った後、プルを行い、ローカルに反映します。

## コンフリクトを起こしてしまった場合、どう対処すべきですか？

- 下記記載の3通りの方法のうち、いずれかの方法で対処します。対処後、コンフリクト解決で行った作業内容をコミットします。
  1. 先にマージされた変更内容を取り込む。
  2. 後にマージしようとしている変更内容を取り込む。
  3. エディタを使用し、両方の変更内容を取り込んだ処理で上書きすることにより、どちらの変更内容も取り込む。