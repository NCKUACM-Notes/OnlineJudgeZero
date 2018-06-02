# ZOJ-d396 - Prime Ring Problem

有一個環 (ring) 是由 $n$ 個圈圈所組成的 (在這裡 $n$ 一定是個偶數)，我們想要把 $1$ 到 $n$ 的自然數各放到一個圈圈中，使得相鄰 $2$ 個圈圈中的數的和一定是質數。下圖為 $n = 6$ 的情形。

* **注意：**第 $1$ 個圈圈中的數一定是 $1$。

![](https://i.imgur.com/mnfi3sZ.png)

> * 題目來源：**UVA-524**
> * 記憶體限制： 512 MB
> * 公開 測資點#0 (100%): 3.0s , < 1K

---
## Input

每組測試資料只包含一整數 $n$ ($0 < n \le 16$)。

---
## Output

請參考 Sample Output，每一列中的數字即為圈圈中的數字，從 $1$ 開始順時針方向旋轉，數字的順序必須滿足以上敘述的要求。

---
## Sample Input

```
6
8
```

---
## Sample Output

```
Case 1:
1 4 3 2 5 6
1 6 5 2 3 4

Case 2:
1 2 3 8 5 6 7 4
1 2 5 8 3 4 7 6
1 4 7 6 5 8 3 2
1 6 7 4 3 8 5 2
```