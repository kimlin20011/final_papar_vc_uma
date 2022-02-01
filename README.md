# final_papar_vc_uma

## note

- 雙欄論文中，設定圖片一欄

```
figure旁邊+ *

\begin{figure*}[htbp] %浮動式圖形
```

- 解決應用文獻排序問題，依照出現順序排序

```
\usepackage[numbers, sort]{natbib}
```

- 表格下方加入敘述

```
\usepackage{threeparttable}
```

```
\begin{table}[]
\begin{threeparttable} %添加此处
      \begin{tabular}{cccc}
        \hline
           & B1  &B2   & B3\\ \hline
        A1 & 0.1 & 0.2 & 0.3\\
        A2 & ... & ..  & .\\
        A3 & ..  & .   & .\\ \hline
      \end{tabular}
      \begin{tablenotes} %添加此处
		\item here are tablenotes. %添加此处
     \end{tablenotes} %添加此处
\end{threeparttable} %添加此处
\end{table}
```

- 剛剛設置好的環境無法顯示 圖片
  - 在`documentclass`後面加`dvipdfmx`才能新增 pdf 圖片
  - `\documentclass[conference, dvipdfmx]{IEEEtran}`
