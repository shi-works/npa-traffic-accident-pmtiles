# traffic-accident-pmtiles
## データについて
- 本データは、警察庁が公開している、[交通事故統計情報のオープンデータ（2019年、2020年、2021年）の本票](https://www.npa.go.jp/publications/statistics/koutsuu/opendata/index_opendata.html)を[tippecanoe](https://github.com/felt/tippecanoe)で[PMTiles形式](https://github.com/protomaps/PMTiles)に変換したデータになります。
- オープンソースソフトウェアで構築

## データ配布
- `https://pmtiles-data.s3.ap-northeast-1.amazonaws.com/traffic-accident/honhyo_2019-2021_convert_v2.pmtiles`(171.5MB)

## ベクトルタイル設計情報
- 本票そのものを可能な限り生かしたデータです。
- tippecanoeによるデータの間引き（自動）を行っています。

### ズームレベル範囲
- 0-14

### 属性
- 本票の属性はそのまま生かしています。
- ただし、値については、コード表をもとに読みやすい形式に変換しています。
- 変換プログラム（Python）は、本リポジトリ内の「converter.zip」を参照してください。

## PMTiles Viewer
- PMTilesはPMTiles Viewerで閲覧することができます。
- https://protomaps.github.io/PMTiles/

## ライセンス
本データセットは[CC-BY-4.0](https://github.com/shi-works/traffic-accident-pmtiles/blob/main/LICENSE)で提供されます。使用の際には本レポジトリへのリンクを提示してください。
また、本データセットは交通事故統計情報のオープンデータ（2019年、2020年、2021年）の本票を加工して作成したものです。本データセットの使用・加工にあたっては、[警察庁Webサイトの利用規約](https://www.npa.go.jp/rules/index.html)を確認し、権利者の権利を侵害しないように留意してください。