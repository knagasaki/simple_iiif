このプログラムとサンプルデータは、「簡単にIIIF対応公開をする」ためのデモンストレーションです。あくまでも可能性を示すためのもので、これ自体はプロダクトといえるものではありません。それを前提の上で、ご利用ください。

このプログラムで生成されるデータは概ね以下のような要件を想定しています。

1. 静的なファイルを公開するWebサーバが利用可能
2. IIIF 画像API用の画像サーバを動かせる（仮想）マシンがない
3. Pythonで何かをしろと言われたら一応モジュールをインストールしてコマンドを打つくらいのことはできる

特に、IIIF対応画像サーバを運用可能なところは、このプログラムを使ってはいけません。あくまでも、画像サーバをどうしても動かせないところのためのものです。

使い方は：

1. mk_mani.pyに書かれているモジュールを一通りインストール
2. metadata.tsvの項目にあわせてデータ入力（Google Spreadsheetで入力してからタブ区切りテキストでダウンロードするのがおすすめです）
3. mk_mani.pyと同じディレクトリ（フォルダ）に、JPGの画像ファイルが入ったフォルダを置く。
4. mk_mani.py を実行する。（metadata.tsvのファイル名は決め打ちになっている）
5. 各画像フォルダの中にmanifest.htmlとview.htmlとサムネイル画像（thum.jpg）ができていることと、mk_mani.pyと同じ階層にindex.htmlが出来ていることを確認。
6. 各画像フォルダとindex.htmlをサーバにアップロード

「簡単にデジタルアーカイブを作れるシステム」を作っておられるみなさまは、ちょっとスクリプトが雑で恐縮ですが、ぜひ参考にして、IIIF対応デジタルアーカイブを増やすことにご協力してください。部分的にまるっとコピペして使っていただいても問題ありません。
