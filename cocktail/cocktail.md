# カクテルソート（シェーカーソート）

## 計算量
|  | 計算時間 |
|:---:|:---:|
| 最悪計算時間 | O(n^2) |
| 最良計算時間 | O(n) |
| 平均計算時間 | O(n^2) |
| 最悪空間計算量 |  |

## アルゴリズム
バブルソートではスキャンを一方向にしか行わないのに対し、シェーカーソートでは交互に二方向に行う。バブルソートと同じく安定な内部ソート。

バブルソートで1回スキャンを行うと、最後の要素1個がスキャン範囲中最大であることが分かり次回のスキャン範囲を1狭めることができる。さらに、このスキャンの最後で連続してm個の要素の交換が行われていなければ、そのm個についてはソート済みであることが分かるので、次回のスキャン範囲をm狭めることができる。この工夫で、後半が殆ど整列済みのデータに対してバブルソートが高速に行えるようになる。

シェーカーソートはこれに加え、スキャン方向を毎回反転することにより、スキャン範囲を後方からだけではなく前方からも狭めるようにしたものである。挿入ソートのように、殆ど整列済みのデータに対しては高速に行うことができる。