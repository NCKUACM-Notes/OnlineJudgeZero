# ZOJ-a134 - Fibonaccimal Base

有名的費氏數列是以 $0$ 和 $1$ 開始，然後把最後的兩個數字相加以得到下一項。例如數列的第三項為 $1$ ($1 = 1 + 0$)，第四項為 $2$ ($2 = 1 + 1$)，第五項為 $3$ ($3 = 2 + 1$)，等等。
 
| $i$ | $0$ | $1$ | $2$ | $3$ | $4$ | $5$ | $6$ | $7$ | $8$ | $9$ |
|---|---|---|---|---|---|---|---|---|---|---|
| $\mathrm{Fib}(i)$ | $0$ | $1$ | $1$ | $2$ | $3$ | $5$ | $8$ | $13$ | $21$ | $34$ |

**表 1 - 費氏數列的前幾項**

這個數列很重要且出現在我們生活及大自然的許多事物上。其中，你知道所有的正整數都可以用費氏數列中的不重覆的數字集合的和來代表嗎？例如：$13$ 可以是集合 ${ 13 }$, ${ 5, 8 }$ 或 ${ 2, 3, 8 }$ 的和，而 $17$ 則可用 ${ 1, 3, 13 }$ 或 ${ 1, 3, 5, 8 }$ 來表示。即然每個數都有這個特性 (你要自己證證看嗎？) 這個數列可以用作表示數字的「底」。但如前所示，有些數字有多種表示法，這該怎麼辦呢？簡單，因為費氏數列中任兩個連續項的和就是下一項，所以只要加上一個限制：不得使用連續的項，那麼每個數字都有一個唯一的表示法。

有了這個認知後我們可以建立一個很酷的方式來表示任意正整數。我們一連串的 $0$ 與 $1$ 來表示。例如：$17 = 1 + 3 + 13$ (記住不可以使用費氏數列中連續的項)，以 $0$ 來表示沒有用到的項，以 $1$ 來表示有用到的項，由右至左排列。因此 $17 = 100101$. 詳情參閱表 2。在這個表示法中，最左邊的那一位數一定是 $1$，不可以是 $0$。根據我們的限制，這種表示法中不可以出現相鄰的 $1$。我們這種表示法為「費氏進位」並以下列方式表示 $17 = 100101$ (fib). 
 
| 17 = | 1 | 0 | 0 | 1 | 0 | 1 |
|---|---|---|---|---|---|---|
| 13 + 3 + 1 = | 13 | 8 | 5 | 3 | 2 | 1 |

**表 2 - $17$ 的費氏進位表示法之說明**

給你一組十進位的數字，你的任務是將它們以費氏進位輸出。

> * 題目來源：**UVA-948**
> * 記憶體限制：512 MB
> * 公開測資點#0 (100%): 1.0s , < 1M

---
## Input

輸入的第一行含有一個數字 $N$，代表以下有幾個數字 ($1 \le N \le 500$)。接下來有 $N$ 行，每行有一個小於 $100,000,000$ 的正整數。數字不一定按順序出現。

---
## Output

對於 $N$ 個整數中的每一個整數要用下列格式輸出一行，`DEC_BASE = FIB_BASE (fib)`。`DEC_BASE` 原始的十進位數字而 `FIB_BASE` 則是它的費氏進位表示法。詳情參閱範例輸出。

---
## Sample Input

```
10
1
2
3
4
5
6
7
8
9
10
```

---
## Sample Output

```
1 = 1 (fib)
2 = 10 (fib)
3 = 100 (fib)
4 = 101 (fib)
5 = 1000 (fib)
6 = 1001 (fib)
7 = 1010 (fib)
8 = 10000 (fib)
9 = 10001 (fib)
10 = 10010 (fib)
```