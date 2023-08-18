%%%%%%%%%%%%%%%%%%%%%%%%%%%
% 非必要的實用套件
% // 可自行增加所需套件 //
%%%%%%%%%%%%%%%%%%%%%%%%%%%
% \usepackage[style=alphabetic, sorting=ynt]{biblatex} % for cite bib
% \usepackage{amsmath} % 各式 AMS 數學功能
% \usepackage{amssymb} % 各式 AMS 數學符號
% \usepackage{mathrsfs} % 草寫體數學符號，在數學模式裡用 \mathscr{E} 得草寫 E.
% \usepackage{subfig} % 圖表中圖表(圖組、表組)
% \usepackage[export]{adjustbox} 修改 TeX boxes 的大小、對齊方式
% \usepackage{longtable} % 跨頁面表
% \usepackage{multicol} % 配置多欄文件
% \usepackage{blindtext} % 假文字 Lipsum
% \usepackage{algorithm} % hyperref 必須放在 algorithm 前面(衝突)
% \usepackage{algpseudocode}
% \usepackage{enumerate}
%%%%%%%%%%%%%%%%%%
%%    table     %%
%%%%%%%%%%%%%%%%%%
% \usepackage{booktabs} % 學術論文三線表 \toprule、\midrule、\bottomrule
% \usepackage{diagbox} % 角線拆分單元格，添加內容到兩個部分
% \usepackage{multirow} % 表中創建跨多行的單元格
% \usepackage{tabularx} % tabular 的擴展
% \usepackage{rotating} % table rotation
% \usepackage{threeparttable} % table note
%%%%%%%%%%%%%%%%%%
%%  創建圖形元素  %%
%%%%%%%%%%%%%%%%%%
% \usepackage{pgfplots} % built on top of TikZ
% \pgfplotsset{compat=1.17}
% \usepackage{pgf}
% \usepackage{tikz} % built on top of PGF
    % \usetikzlibrary{arrows,shapes} % 為 TikZ 加載其他庫
% \usepackage{flowchart} % built on top of TikZ
%%%%%%%%%%%%%%%%%%
%%  程式列表套件  %%
%%%%%%%%%%%%%%%%%%
% \usepackage{listings}
% \lstset{
%     breaklines=true, % 過長的程式行可斷行
%     extendedchars=false, % 中文處理不需要 extendedchars
%     texcl=true, % 中文註解需要有 TeX 處理過的 comment line, 所以設成 true
%     comment=[l]\%\%, % 以雙「百分號」做為程式中文註解的起頭標記，配合 MATLAB
%     basicstyle=\small, % 小號字體, 約 10 pt 大小
%     commentstyle=\upshape, % 預設是斜體字，會影響註解裏的英文，改用正體
%     language=Octave % 會將一些 octave 指令以粗體顯示
% }