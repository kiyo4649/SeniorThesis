# ドメイン依存のデータセットを使用した識別子命名支援システム
　　　　　

卒業研究の一環として、識別子を命名支援するシステムを開発しました。



//////////////// システム先のリンク　////////////////

https://kiyo4649.github.io/SeniorThesis/

//////////////// システムの説明　////////////////

　このシステムは、ゲーム、画像処理、卒研実験用プロジェクトの3つのドメインに依存されたデータセットを用いて、より精度の高い命名支援を行う

そして、本実験ではこのシステムを用いて、ドメインに依存されたデータセットを使用すれば、命名支援システムの精度が高くなるかを確認する

　以下に、このシステムの要素の説明をする

データセットのドメイン

　ゲーム：ゲーム開発で使われている識別子のデータセットを対象とする

　画像処理：画像処理プログラムで使われている識別子のデータセットを対象とする

　卒研実験用：実験の問題で使われている識別子のプロジェクトを対象とする

 
データセットの言語

　Java：Javaで書かれたプロジェクトのデータセットを対象とする

　Python：Pythonで書かれたプロジェクトのデータセットを対象とする
 
出力する識別子

　変数：取得した識別子から変数を出力する

　関数：取得した識別子から関数を出力する

 
 また、このシステムには、名前探索機能と相関パス機能がある。
 名前探索機能は、以下の「出力する方法」に対応する識別子と、データセット内での識別子の出現回数を出力する。

  　head-key：入力されたキーワードから始まる識別子を出力する

  　include-key：入力されたキーワードを含む識別子を出力する

  　parfect-key：入力されたキーワードに一致する識別子を出力する

 出現回数が多い順に出力されるので、上位に表示されている識別子ほど、より使われていて精度が高いといえる。

 相関パス機能は、以下の「出力する方法」に対応する識別子と、データセット内での識別子の出現回数を出力する。

  　head-key：入力されたキーワードから始まる識別子と相関関係にある識別子を出力する

  　include-key：入力されたキーワードを含む識別子と相関関係にある識別子を出力する

  　parfect-key：入力されたキーワードに一致する識別子と相関関係にある識別子を出力する

　ここでいう相関関係の詳細として、

　　変数の場合、キーワードとなる 変数 と同じ構文中に含まれている 変数 が出力される

　　関数の場合、キーワードとなる 変数 を含んでいる 関数 が出力される

 これも出現回数が多い順に出力されるので、上位に表示されている識別子ほど、より使われていて精度が高いといえる。

 
　つまり、以下の選択をしていた場合、Javaで書かれたゲーム開発で使われている変数から、入力されたキーワード 'a' から始まる変数を出力することになる。

　　データセットのドメイン：ゲーム

　　データセットの言語：Java

　　出力する識別子：変数

　　機能：名前探索機能：head-key

  　入力されたキーワード：a


   
//////////////// 実験でのシステムの使い方　////////////////


　問題1では、Pythonで書かれたプログラムに対し、引継開発を行う。
 よって、データセットの言語を "Python" に設定する必要がある。
 
　また、問題2では、Javaで書かれたプログラムに対し、引継開発を行う。
 よって、データセットの言語を "Java" に設定する必要がある。

　　　　　
　　　　　
 　












