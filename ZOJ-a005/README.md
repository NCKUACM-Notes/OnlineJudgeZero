# ZOJ-a005 - Eva 的回家作業

Eva的家庭作業裏有很多數列填空練習。填空練習的要求是：已知數列的前四項，填出第五項。因為已經知道這些數列只可能是等差或等比數列，她決定寫一個程式來完成這些練習。

> * 記憶體限制： 512 MB
> * 公開 測資點#0 (100%): 1.0s , < 1K
> * 公開 測資點#1 (0%): 1.0s , < 1K
> * 公開 測資點#2 (0%): 1.0s , < 1K
> * 公開 測資點#3 (0%): 1.0s , < 1K
> * 公開 測資點#4 (0%): 1.0s , < 1M
> * 公開 測資點#5 (0%): 1.0s , < 1M
> * 公開 測資點#6 (0%): 1.0s , < 10M
> * 公開 測資點#7 (0%): 1.0s , < 10M
> * 公開 測資點#8 (0%): 1.0s , < 10M
> * 公開 測資點#9 (0%): 1.0s , < 10M
> * 公開 測資點#10 (0%): 1.0s , < 10M
> * 公開 測資點#11 (0%): 1.0s , < 10M
> * 公開 測資點#12 (0%): 1.0s , < 10M

---
## Input

第一行是數列的數目 $t$ ($0 \le t \le 20$)。以下每行均包含四個整數，表示數列的前四項。約定數列的前五項均為不大於 $105$ 的自然數，等比數列的比值也是自然數。

---
## Output

對輸入的每個數列，輸出它的前五項。

---
## Sample Input

```
2
1 2 3 4
1 2 4 8
```

---
## Sample Output

```
1 2 3 4 5
1 2 4 8 16
```