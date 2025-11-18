# ekidata.rb

## 概要

[駅データ.jp](https://ekidata.jp)様が配布されている日本の鉄道駅情報CSVデータを基に生成されたJSONおよびXML形式のAPIを提供します。

## API仕様

提供されるAPIは、以前駅データ.jp様が提供されていた[APIサービス]([https://ekidata.jp/api/])の仕様に準拠しています。

駅データ.jp 様より配布されているCSVデータを元にRubyスクリプトを使用してJSONおよびXMLファイルに変換しています。
これらの生成ファイルはGitHub Pagesを用いて公開しているため、無料でAPIサービスを提供できます。

## API更新手順

1. master ブランチから作業用ブランチを切る。
2. 駅データ.jp 様より配布されている最新のCSVデータを data フォルダに配置する。
3. 作業用ブランチを master ブランチにマージする。
4. master ブランチの内容を release ブランチにマージする。
5. GitHub Actionsがトリガーされ、CSVデータがJSON/XMLファイルに変換され、gh-pages ブランチにプッシュされる。

## 利用方法

以下のAPI仕様書をご確認ください。

https://dreamkyast0.github.io/ekidata.rb/

## ライセンス

本APIの利用にあたっては、データ提供元である駅データ.jp様の[利用規約](https://ekidata.jp/agreement.php)を参照してください。
