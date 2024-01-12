# 令和6年能登半島地震 被災状況マップ
令和6年能登半島地震に関連して被災状況の把握を目的に公開されたデータをMapLibre GL JSで表示するデモサイトです。

## Public Website
https://shi-works.github.io/noto-hanto-earthquake-2024-gsi-ortho-map-on-maplibre-gl-js/

https://github.com/shi-works/noto-hanto-earthquake-2024-gsi-ortho-map-on-maplibre-gl-js/assets/71203808/c5c9be77-e79e-4c31-abba-f9abc0362def

## Data Source
### 国土地理院
- 被災前の空中写真：全国（能登半島：2010年4月～5月撮影）
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#seamlessphoto
- 被災後の空中写真（正射画像）：珠洲地区、輪島東地区、輪島中地区、20240102撮影
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#t20240102noto_suzu_0102do
- 被災後の空中写真（正射画像）：珠洲地区、輪島中地区、穴水地区、七尾地区、20240105撮影
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#t20240102_noto_suzu_0105do
- 被災後の空中写真（正射画像）：輪島中地区、穴水地区、輪島西地区、20240111撮影
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#t20240102noto_wazimanaka_0111do
- 斜面崩壊・堆積分布データ（2024年1月9日更新）
    - 出典：https://www.gsi.go.jp/BOUSAI/20240101_noto_earthquake.html#2
    - 概要：国土地理院が1月2日及び1月5日に撮影した空中写真（正射画像）・（珠洲地区、輪島東地区、輪島中地区、穴水地区、七尾地区）から、令和6年能登半島地震によって生じたと考えられる斜面崩壊地及び土砂堆積箇所の範囲について判読（一部は再度判読）したものです。
    - ※1 道路や河川上の土砂は、一部撤去されている可能性があります。
    - ※2 穴水地区及び七尾地区は、1月5日に撮影した空中写真（正射画像）のみを用いて判読しています。
    - ※3 珠洲地区及び輪島中地区は、1月2日及び1月5日に撮影した空中写真（正射画像）を用いて、再度判読しています。

- 空中写真判読による津波浸水域（推定）データ（2024年1月12日更新）
    - 出典：https://www.gsi.go.jp/BOUSAI/20240101_noto_earthquake.html#7
    - 概要：国土地理院が1月2日及び1月5日に撮影した空中写真（珠洲地区、輪島東地区、穴水地区、七尾地区、輪島西地区）から、令和6年能登半島地震によって生じたと考えられる津波到達範囲（堤外地を含む）を判読（一部を再判読）して作成したものです。津波到達範囲（堤外地を含む）の面積は、おおむね2.8平方キロメートルです。
    - ※ 海岸線は空中写真（正射画像）に合わせて取得しており、地形図と整合していない箇所があります。

- 上記の公開データのライセンス：[国土地理院コンテンツ利用規約](https://www.gsi.go.jp/kikakuchousei/kikakuchousei40182.html)に従い、出典明示により、転載も含め使用可

### 東京大学渡邉英徳研究室
- 被災後のSAR画像：20240106撮影
    - 出典：https://github.com/wtnv-lab/20240102_Noto_Earthquake_SAR_Umbra/
    - 概要：[Umbra Open Data Program](https://umbra.space/open-data)にて公開されている[Noto Peninsula Earthquake](http://umbra-open-data-catalog.s3-website.us-west-2.amazonaws.com/?prefix=sar-data/tasks/ad%20hoc/Noto%20Peninsula%20Earthquake/)を、東京大学渡邉英徳研究室にてXYZタイルに変換したものです。

- 上記の公開データのライセンス：[Umbra Open Data Program](https://umbra.space/open-data)、[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

### 日本地理学会災害対応委員会
- 海岸地形変化の検討結果（1月8日公開）
    - 出典：https://ajg-disaster.blogspot.com/
    - 概要：http://disaster.ajg.or.jp/files/202401_Noto004.pdf

- 上記の公開データのライセンス：令和6年能登半島地震変動地形調査グループ（日本地理学会）、[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

### 背景地図及び地形データ
- 国土地理院 最適化ベクトルタイル
    - 出典：https://github.com/gsi-cyberjapan/optimal_bvmap
- 国土地理院 地理院タイル（陰影起伏図）
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#hillshademap
- 産業技術総合研究所 シームレス標高タイル（統合DEM）
    - 出典：https://tiles.gsj.jp/tiles/elev/tiles.html
- 森林総合研究所 CS立体図(能登(石川県))
    - 出典：https://www2.ffpri.go.jp/soilmap/data-src.html

### 人口分布データ
- 令和2年簡易100mメッシュ人口データ（石川県、富山県）（FlatGeobuf形式）
    - 出典：https://github.com/shi-works/noto-hanto-earthquake-2024-100m-mesh-pop-data
        - 原初データ出典：[地域分析に有用なデータの提供, 地域・交通データ研究所代表（東京大学空間情報科学研究センター客員研究員）西澤明](https://gtfs-gis.jp/teikyo/index.html)
    - 概要：地域・交通データ研究所にて公開されている令和2年簡易100mメッシュ人口データをFlatGeobuf形式に変換したデータです。
    - ライセンス：[西澤明](https://gtfs-gis.jp/teikyo/index.html)、[@shi-works](https://twitter.com/shi__works)、[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)

### 孤立集落人数データ（1月10日時点）
- 孤立集落人数データ（石川県）（GeoJSON形式）
    - 出典：https://x.com/GISPHN/status/1745321675393298538?s=20
        - 原初データ出典：[石川県災害対策本部員会議資料](https://www.pref.ishikawa.lg.jp/saigai/202401jishin-taisakuhonbu.html#honbu)
    - 概要：堀池様（[@GISPHN](https://twitter.com/GISPHN)）が石川県災害対策本部員会議資料の孤立集落の区域と人数をGeoJSON形式で作成したデータです。
    - 作成方法：https://g-cham.carrd.co/#news10
