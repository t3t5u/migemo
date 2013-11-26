J/Migemo

  Migemoとは、通常日本語を入力する時に使う変換プログラム(IM)を通さずに
  日本語の検索を行う技術で、J/MigemoはそれをJavaで実装したものです。
  Migemo自体の詳細については本家Migemoのページ http://0xcc.net/migemo/
  を参照してください。

動作条件
  JRE1.4以上

  Migemoには専用の辞書が必要です。
  このパッケージには辞書は含まれていないので、本家Migemoのページから
  migemo-0.XX.tar.gzをダウンロード・解凍し、migemo-0.XXの下のmigemo-dictを
  辞書として使用してください。

コンパイル
  srcディレクトリに移動して
  	javac org\monazilla\migemo\Migemo.java (Windows)
  	javac org/monazilla/migemo/Migemo.java (UNIX系)
  Sample.javaはJ/Migemoの使用例です。

ドキュメント
  javadocで生成してください。
  	javadoc src\org\monazilla\migemo\Migemo.java (Windows)
  	javadoc src/org/monazilla/migemo/Migemo.java (UNIX系)

入力文字列の分割について
  大文字アルファベットの前で入力を分割しそれぞれ独立に検索文字列を生成した後
  それらを結合したものを返します。
  "Q"も他の大文字アルファベット同様境界となりますが、
  "Q"自体は検索文字列には反映されず続く部分は辞書を参照しません。

問い合わせ
  J/Migemoの動作上の問題に関する問い合わせは2chソフトウェア板の
  V2Cスレッドにお願いします。

ライセンス
  同梱のLICENSE.txtを参照してください。（MIT/X）


                                    n|a <http://v2c.s50.xrea.com/jmigemo/>
