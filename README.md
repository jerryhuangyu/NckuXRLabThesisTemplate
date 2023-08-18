# NCKU XRLab Thesis Template

適用於成功大學土木工程研究所碩士論文使用的模板，需要的同學可以直接 fork 後做使用。

> 2023/08/14 已通過上傳系統！

## Usage

### Basic

以下是使用本模板的一些基本步驟：

1. 下載本模板。
2. 上傳至 https://overleaf.com。
3. thesis-param 資料夾: 撰寫論文基本資料、目錄名稱。
4. contents 資料夾: 撰寫論文內容
5. images 資料夾: 論文使用圖檔放置處

### Syntax

#### 標題

```latex=
% Latex
\section{研究動機}
\subsection{自動化施作瓶頸}
\subsubsection{\Ssd{1}解析需求} % 小標不納入TOC
```

```latex=
% Results
1.1 研究動機
1.1.2 自動化施作瓶頸
(1) 解析需求
```

#### 圖片引用

```latex=
缺工問題（圖\ref{fig:example_tag}）。

\begin{figure}[H]
  \centering
  \includegraphics[width=10cm]{images/example.png}
  \caption{近四年營建工程業人力需求淨增減人數}
  \label{fig:example_tag}
\end{figure}
```

#### 表格引用

> 表格請使用 latex table generator 產生 (https://www.tablesgenerator.com/)

```latex=
之間的差異如表 \ref{tab:compare-agv-amr} 所示。

\begin{table}[H]
  \centering
  \caption{AGV 和 AMR 間的差異比較}
  \label{tab:compare-agv-amr}
  \begin{tabular}{lll}
  \hline
  \rowcolor[HTML]{C0C0C0} 
  項目\hspace{1.5cm} & Automated Guided Vehicle & Autonomous Mobile Robot \\ \hline
  導航方式 & 固定路線 & 自主導航 \\
  預置設施 & 需要安裝 & 無需安裝 \\
  適用場景 & 固定環境 & 動態環境 \\ \hline
  任務性質 & 專注單一 & 多樣靈活 \\
  任務適應性 & 缺乏調整彈性 & 具可擴展性 \\
  導入速度 & 較長佈署時間 & 快速導入 \\ \hline
  \end{tabular}
\end{table}
```

#### 無序列表

```latex=
\begin{itemize}
  \item 建物名稱：成功大學某教學大樓
  \item 建物規模：鋼筋混凝土建築結構，地下兩層、地上七層
  \item 案例驗證空間：2F 指定區域
\end{itemize}
```

## Folder tree

主要檔案: `main.tex` (透過呼叫其他 .tex 來組成)

* `main.tex`
* contents/
  * body/
    * (各章節內容)
  * enAbstract/
    * (英文摘要)
  * `ackn.tex`: 致謝
  * `zhAbstract.tex`: 中文摘要
* images/
  * (論文使用圖檔放置處)
* ncku-style/
  * (論文風格)
* thesis-param/
  * `Date.sty`: 畢業日期
  * `DepartmentInfomation.sty`: 學校學系基本資料
  * `TableOfContent.sty`: 目錄的章節名稱
  * `Title.sty`: 論文中英標題
  * `Writer.sty`: 第一作者、第二作者