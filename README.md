# noto-hanto-earthquake-2024-gsi-ortho-map-on-maplibre-gl-js
令和6年能登半島地震に関連して被災状況の把握を目的に公開されたデータをMapLibre GL JSで表示するデモサイトです。

## Public Website
https://shi-works.github.io/noto-hanto-earthquake-2024-gsi-ortho-map-on-maplibre-gl-js/

## Data Source
### 国土地理院
- 被災前の空中写真：全国（能登半島：2010年4月～5月撮影）
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#seamlessphoto
- 被災後の空中写真（正射画像）：珠洲地区、輪島東地区、輪島中地区、20240102撮影
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#t20240102noto_suzu_0102do
- 被災後の空中写真（正射画像）：珠洲地区、輪島中地区、穴水地区、七尾地区、20240105撮影
    - 出典：https://maps.gsi.go.jp/development/ichiran.html#t20240102_noto_suzu_0105do
- 斜面崩壊・堆積分布データ（2024年1月6日更新分）
    - 出典：https://www.gsi.go.jp/BOUSAI/20240101_noto_earthquake.html#2
    - 概要：国土地理院が1月2日及び1月5日に撮影した空中写真（正射画像）・（珠洲地区、輪島東地区、輪島中地区、穴水地区）から、令和6年能登半島地震によって生じたと考えられる斜面崩壊地及び土砂堆積箇所の範囲について判読（一部は再度判読）したものです。
    - ※1 道路や河川上の土砂は、一部撤去されている可能性があります。
    - ※2 穴水地区は、1月5日に撮影した空中写真（正射画像）のみを用いて判読しています。
    - ※3 珠洲地区及び輪島中地区は、1月2日及び1月5日に撮影した空中写真（正射画像）を用いて、再度判読しています。

- 空中写真判読による津波浸水域（推定）データ
    - 出典：https://www.gsi.go.jp/BOUSAI/20240101_noto_earthquake.html#7
    - 概要：`国土地理院が1月2日に撮影した空中写真（正射画像）・（珠洲地区、輪島東地区）から、令和6年能登半島地震によって生じたと考えられる津波浸水域を判読して作成したもの`であり、`海岸線は空中写真（正射画像）に合わせて取得しており、地形図と整合していない箇所があります`とのこと。

- 上記の公開データのライセンス：[国土地理院コンテンツ利用規約](https://www.gsi.go.jp/kikakuchousei/kikakuchousei40182.html)に従い、出典明示により、転載も含め使用可

### 日本地理学会災害対応委員会
- 海岸地形変化の検討結果（1月5日公開）
    - 出典：https://ajg-disaster.blogspot.com/
        - 原初データ出典：[国土地理院空中写真（正射画像）](https://www.gsi.go.jp/BOUSAI/20240101_noto_earthquake.html)

- 上記の公開データのライセンス：令和6年能登半島地震変動地形調査グループ（日本地理学会）、[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.ja)
