# 警察庁 交通事故統計情報のオープンデータ（PMTiles形式）
- 本データは、警察庁が公開している、[交通事故統計情報のオープンデータ（2019年、2020年、2021年、2022年）の本票](https://www.npa.go.jp/publications/statistics/koutsuu/opendata/index_opendata.html)を[feltのtippecanoe](https://github.com/felt/tippecanoe)で[PMTiles形式](https://github.com/protomaps/PMTiles)に変換したデータになります。
- オープンソースソフトウェアで構築

## デモサイト
- https://shi-works.github.io/npa-traffic-accident-map-on-maplibre-gl-js/#15/35.92275/139.48775

## データの加工方法
- 2019-2021年
  - https://github.com/shi-works/npa-traffic-accident-data-converter
- 2022年
  - https://github.com/shi-works/npa-traffic-accident-data-2022-converter

## データ配布
- PMTiles形式
  - 2019-2021年
    - `https://xs489works.xsrv.jp/pmtiles-data/traffic-accident/honhyo_2019-2021_convert_v2.pmtiles`(206.3MB)
  - 2019-2022年
    - `https://xs489works.xsrv.jp/pmtiles-data/traffic-accident/honhyo_2019-2022_convert.pmtiles`(280.8MB)
- GeoParquet形式
  - 2019-2021年
    - `https://xs489works.xsrv.jp/pmtiles-data/traffic-accident/honhyo_2019-2021_convert_v2.parquet`(65.8MB)
  - 2019-2022年
    - `https://xs489works.xsrv.jp/pmtiles-data/traffic-accident/honhyo_2019-2022_convert.parquet`(94.2MB)

## ベクトルタイル設計情報
- 本票そのものを可能な限り生かしたデータです。
- tippecanoeによるデータの間引き（自動）を行っています。

### ズームレベル範囲
- 0-14

### 属性
- 本票の属性はそのまま生かしています。
- ただし、値については、コード表をもとに読みやすい形式に変換しています。
- 変換プログラム（Python）は、下記のリポジトリを参照してください。
  - 2019-2021年 https://github.com/shi-works/traffic-accident-data-converter
  - 2022年 https://github.com/shi-works/traffic-accident-data-2022-converter

## PMTiles Viewer
- PMTilesはPMTiles Viewerで閲覧することができます。
  - https://protomaps.github.io/PMTiles/?url=https://xs489works.xsrv.jp/pmtiles-data/traffic-accident/honhyo_2019-2022_convert.pmtiles#map=8.64/35.6674/139.8287

## ライセンス
本データセットは[CC-BY-4.0](https://github.com/shi-works/traffic-accident-pmtiles/blob/main/LICENSE)で提供されます。使用の際には本リポジトリへのリンクを提示してください。

また、本データセットは交通事故統計情報のオープンデータ（2019年、2020年、2021年、2022年）の本票を加工して作成したものです。本データセットの使用・加工にあたっては、[警察庁Webサイトの利用規約](https://www.npa.go.jp/rules/index.html)を必ずご確認ください。

## 免責事項
利用者が当該データを用いて行う一切の行為について何ら責任を負うものではありません。
