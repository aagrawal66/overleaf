# overleaf

\documentclass[10  pt, english]{article}
\usepackage[english]{babel}
\selectlanguage{english}
\usepackage[utf8]{inputenc}
\usepackage[margin=1in]{geometry}% Change the margins here if you wish.
\setlength{\parindent}{0pt} % This is the set the indent length for new paragraphs, change if you want.
\setlength{\parskip}{5pt} % This sets the distance between paragraphs, which will be used anytime you have a blank line in your LaTeX code.
% \pagenumbering{gobble}% This means the page will not be numbered. You can comment it out if you like page numbers.

%------------------------------------

\usepackage{amsmath,amsthm,amssymb} %common math  
\usepackage{graphicx}
\usepackage{float}  
\usepackage{wasysym} %smiley faces :)-
\usepackage[utf8]{inputenc}
\usepackage[nottoc]{tocbibind}
\bibliographystyle{ieeetr}
\usepackage{listings}
\usepackage{graphicx}
\usepackage{stmaryrd}
\usepackage{bm}
\usepackage{tikz-cd}
\usepackage{fancyhdr}
\usepackage{cancel}
\usepackage{minted} % code coloring
\usepackage{hyperref}
\usepackage{gensymb}
\usepackage{subcaption}
\usepackage{pdfpages}
\usepackage{dirtytalk} %quoting
\usepackage[framed,numbered,autolinebreaks,useliterate]{mcode}

\newcommand{\pr}[1]{\left(#1\right)}
\newcommand{\sq}[1]{\left[#1\right]}
\newcommand{\br}[1]{\left\{#1\right\}}
\newcommand{\ip}[2]{\langle #1, #2 \rangle} %example call:  \innerproduct{v}{w}
\newcommand{\nr}[1]{\left\|{#1}\right\|} % norm command
\newcommand{\abs}[1]{\left|{#1}\right|} % absolute value command
\newcommand{\spt}{\,\,\,} % three spaces command
\newcommand{\qf}[2]{\mathbf{#1}#2\mathbf{#1}} % quadratic form 
\newcommand{\vd}[1]{\dot{\mathbf{#1}}} % vector derivative
\newcommand{\bv}[1]{\mathbf{#1}} % bold vector
\newcommand{\sd}[1]{\dot{\boldsymbol{#1}}} % bold symbol vector derivative
\newcommand{\bs}[1]{\boldsymbol{#1}} % bold sybmol vector 
\newcommand{\qn}[1]{\mathbf{\bar{#1}}} % quaternion 
\newcommand{\qd}[1]{\mathbf{\dot{\bar{#1}}}} % quaternion deriv
\newcommand{\qde}[1]{\delta\mathbf{\bar{#1}}} % quaternion error
\newcommand{\ssc}[1]{\begin{bmatrix} 0 & -#1_z & #1_y \\ #1_z & 0 & -#1_x\\ -#1_y & #1_x & 0 \end{bmatrix}} % cross-product skew symmetric matrix 
\newcommand{\sscu}[1]{\begin{bmatrix} 0 & -#1_3 & #1_2 \\ #1_3 & 0 & -#1_1\\ -#1_2 & #1_1 & 0 \end{bmatrix}} % cross-product skew symmetric matrix, numbers
\newcommand{\sscn}[2]{\begin{bmatrix} 0 & -#1_{#2,z} & #1_{#2,y} \\ #1_{#2,z} & 0 & -#1_{#2,x}\\ -#1_{#2,y} & #1_{#2,x} & 0 \end{bmatrix}} % nominal cross product skew symmetric matrix 
\newcommand{\sscnu}[2]{\begin{bmatrix} 0 & -#1_{#2,3} & #1_{#2,2} \\ #1_{#2,3} & 0 & -#1_{#2,1}\\ -#1_{#2,2} & #1_{#2,1} & 0 \end{bmatrix}} % nominal cross product skew symmetric matrix, numbers
\newcommand{\diat}[1]{\begin{bmatrix} #1_1 & 0 & 0 \\ 0 & #1_2 & 0\\ 0 & 0 & #1_3 \end{bmatrix}} % 3x3 diagonal, inertia matrix
\newcommand{\idiat}[1]{\begin{bmatrix} #1_1^{-1} & 0 & 0 \\ 0 & #1_2^{-1} & 0\\ 0 & 0 & #1_3^{-1} \end{bmatrix}} % inverse 3x3 diag matrix 

\newcommand{\bnv}[2]{\begin{bmatrix}\boldsymbol{#1}_{#2,x} \\ \boldsymbol{#1}_{#2,y}\\ \boldsymbol{#1}_{#2,z}\end{bmatrix}}%nominal vector

\newcommand{\evn}[1]{\begin{bmatrix}\delta{#1}_{1} \\ \delta{#1}_{2}\\ \delta{#1}_{3}\end{bmatrix}}

% \newenvironment{problem}[2][Problem]{\begin{trivlist}
% \item[\hskip \labelsep {\bfseries #1}\hskip \labelsep {\bfseries #2.}]}{\end{trivlist}}

\begin{document}

\thispagestyle{empty}
\begin{center}
\vspace{0.5\baselineskip}
\large{\textbf{Template}} \\
\vspace{0.5\baselineskip}
by \\
\vspace{0.5\baselineskip}
Name \\
% \href{mailto://{}\\
% \href{mailto://{}\\
\vspace{8cm}
\vspace{0.5\baselineskip}
Affiliation  \\ 
\vspace{0.5\baselineskip}
\vspace{8cm}
Location\\
\today
\vspace{0.5\baselineskip}
\end{center}

\pagestyle{fancy}
\fancyhead{} % clear all header fields
\fancyhead[CO]{\textbf{Template}}
\fancyhead[RO]{\text{Template}}
\fancyhead[LO]{Template}
\fancyfoot{} % clear all footer fields
\fancyfoot[CO]{\thepage}

\newpage
\input{d1}
\renewcommand\bibname{References}
\bibliography{references}
\end{document}
