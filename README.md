# 個人用Rubocop設定ファイル

使ってて指摘がうざかったり不要だったりする箇所をカスタマイズしています。

修正箇所一覧
- Rails
  - Rails用に最適化
- require
  - rubocop-performance
    - プロジェクトのパフォーマンス最適化の指摘を受ける
- Metrics/BlockLength
  - 設定やテストなど、指摘を受ける気の無いファイルで無効化
- Metrics/LineLength
  - MAX120字に拡大
  - ヒアドキュメント、URIに関しては例外を認める
  - テストファイルでは無視する
- Metrics/ModuleLength
  - テストファイルでは無視する
- Style/AsciiComments
  - アルファベット以外での(日本語)コメントを許可する
- Style/BlockDelimiters
  - AllowBracesOnProceduralOneLiners
    - ワンラインの場合ブロックは`{}`で書く
  - EnforcedStyle
    - 戻り値にメソッドがチェインしている場合のブロックは`{}`で書く

https://github.com/cookpad/global-style-guides/blob/master/.rubocop.yml
