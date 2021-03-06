# ZOJ-d221 - Add All

是的，題目名稱就是你要做的任務：把一些數加起來。但是這對你來說一定是太簡單了，所以讓我們加一些東西在裡面。
做加法要付出的代價 (cost) 定義為這 $2$ 個數的總和，所以要加 $1$ 和 $10$ 所需付出的代價為 $11$ 。假如你想要加 $1$，$2$ 和 $3$，那麼有以下幾種方法：

| 1 + 2 = 3, cost = 3<br>3 + 3 = 6, cost = 6<br>Total = 9 | 1 + 3 = 4, cost = 4<br>2 + 4 = 6, cost = 6<br>Total = 10 | 2 + 3 = 5, cost = 5<br>1 + 5 = 6, cost = 6<br>Total = 11 |
|---|---|---|

我希望你已經瞭解你的任務，就是把 $N$ 個數加起來使得付出的代價最少。

> * 題目來源：**UVA-10954**
> * 記憶體限制：512 MB
> * 公開測資點#0 (100%): 10.0s , < 1M

---
## Input

輸入含有多組測試資料。每組測試資料開始有一個正整數 $N$ ($2 \le N \le 5,000$)，接下來有 $N$ 個正整數 (均小於 $100,000$)。當 $N = 0$ 時代表輸入結束。請參考 Sample Input。

---
## Output

對每一組測試資料輸出一列，相加這 $N$ 個數付出的代價最少是多少。這個代價一定可以用 `INT64` 或是 `long long int` 存取。

---
## Sample Input

```
3
1 2 3
4
1 2 3 4
0
```

---
## Sample Output

```
9
19
```