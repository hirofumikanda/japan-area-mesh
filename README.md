# japan-area-mesh

日本全国の地域メッシュ（1次メッシュ、2次メッシュ、3次メッシュ）をベクタータイル形式で公開しています。  
地理空間データの可視化や解析、教育用資料などにご活用いただけます。

## 🔷 概要

本リポジトリには、以下のメッシュ区画のpbfファイル及びMBTiles形式のベクタータイルが含まれています。

| メッシュ種別 | ズームレベル | レイヤ名 | 内容                             |
|--------------|------------------------|----------------------------------|----------------------------------|
| 1次メッシュ  | 5-12  | first_mesh / first_mesh_labels | 約80km四方のメッシュポリゴン     |
| 2次メッシュ  | 9-12  | second_mesh / second_mesh_labels | 約10km四方のメッシュポリゴン     |
| 3次メッシュ  | 12  | third_mesh / third_mesh_labels | 約1km四方のメッシュポリゴン |

## 📦 ファイル構成

```

.
├── tiles/           # vector tileを展開したディレクトリ
├　　├── style.json   # style.jsonのサンプル
├── mesh.mbtiles     # 1〜3次メッシュを含むベクタータイル（MVT）
└── ...

````

## 🌐 タイルの利用方法

MapLibre GL JSなどのライブラリを使って、tiles/style.jsonを読み込むことができます。

## 📘 メッシュ仕様

* 標準地域メッシュ：
  [https://www.esrij.com/gis-guide/gis-other/mesh/](https://www.esrij.com/gis-guide/gis-other/mesh/)
* メッシュコードの仕様に基づき独自にGeoJSONを生成

## 🪪 ライセンス

MIT License に基づき、自由にご利用いただけます。
