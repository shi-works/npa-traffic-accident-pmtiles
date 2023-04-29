# traffic-accident-pmtiles
## データについて
- 本データは、警察庁が公開している、[交通事故統計情報のオープンデータ（2019年、2020年、2021年）の本票](https://www.npa.go.jp/publications/statistics/koutsuu/opendata/index_opendata.html)を[tippecanoe](https://github.com/felt/tippecanoe)で[PMTiles形式](https://github.com/protomaps/PMTiles)に変換したデータになります。
- オープンソースソフトウェアで構築

## デモサイト
- https://shi-works.github.io/traffic-accident-map/

## データ配布
### PMTiles形式
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/traffic-accident/honhyo_2019-2021_convert_v2.pmtiles`(206.3MB)
### GeoParquet形式
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/traffic-accident/honhyo_2019-2021_convert_v2.parquet`(65.8MB)

## ベクトルタイル設計情報
- 本票そのものを可能な限り生かしたデータです。
- tippecanoeによるデータの間引き（自動）は行っていません。

### ズームレベル範囲
- 0-14

### 属性
- 本票の属性はそのまま生かしています。
- ただし、値については、コード表をもとに読みやすい形式に変換しています。
- 変換プログラム（Python）は、下記のリポジトリを参照してください。
- https://github.com/shi-works/traffic-accident-data-converter

## PMTiles Viewer
- PMTilesはPMTiles Viewerで閲覧することができます。
- https://protomaps.github.io/PMTiles/

## ライセンス
本データセットは[CC-BY-4.0](https://github.com/shi-works/traffic-accident-pmtiles/blob/main/LICENSE)で提供されます。使用の際には本レポジトリへのリンクを提示してください。

また、本データセットは交通事故統計情報のオープンデータ（2019年、2020年、2021年）の本票を加工して作成したものです。本データセットの使用・加工にあたっては、[警察庁Webサイトの利用規約](https://www.npa.go.jp/rules/index.html)を必ずご確認ください。

## 免責事項
利用者が当該データを用いて行う一切の行為について何ら責任を負うものではありません。
