# ZOJ-c013 - Triangle Wave

在這個問題中，根據所給的振幅 (Amplitude) 及頻率 (Frequency)，你的程式要產生這樣的波。

> * 題目來源：**UVA-488**
> * 記憶體限制：512 MB
> * 公開測資點#0 (100%): 1.0s , < 1K

---
## Input

輸入的第一列有一個整數 $n$，代表有幾組測試資料。接下來每組測試資料有 $2$ 列，各有 $1$ 個正整數（A、F），$A$ 代表振幅（$A \le 9$），$F$ 代表頻率。 第一列以及各組測試資料間皆有一空白行。請參考 Sample Input。

---
## Output

每組測試資料請輸出 $F$ 個波，每個波振幅的水平高度為 $A$。波本身是以其「高度」的內容所組成。每個波之間以一空白行分隔開來。 測試資料間也以一空白行分開。 請參考 Sample Output。

---
## Sample Input

```
2

3
2
5
3
```

---
## Sample Output

```
1
22
333
22
1

1
22
333
22
1

1
22
333
4444
55555
4444
333
22
1

1
22
333
4444
55555
4444
333
22
1

1
22
333
4444
55555
4444
333
22
1
```