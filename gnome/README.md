# ノームソート

## 計算量
|  | 計算時間 |
|:---:|:---:|
| 最悪計算時間 | O(n^2) |
| 最良計算時間 | O(n) |
| 平均計算時間 | O(n^2) |
| 最悪空間計算量 | O(1) auxiliary |

## アルゴリズム
挿入ソートに似ているが、要素の移動は挿入ではなくバブルソートのような一連の交換で行う。
非常に単純であり、入れ子のループも必要としない。時間計算量は O(n2) だが、実際にソートしてみると挿入ソートと同程度の性能を発揮する。

安定ソートである。