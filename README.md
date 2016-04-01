# Custom beamer theme

This beamer theme is more visually appealing than many of the default themes.

Below is a bare-bones implementation of the theme.

```latex
%!TEX program = xelatex
\documentclass{beamer}

\usepackage{blindtext}
\usepackage{setspace}
\usetheme{custom}
\title{title here}
\subtitle{subtitle here}
\author{Your Name}
\date{whatever date}

\setcounter{showSlideNumbers}{1}

\begin{document}
	\setcounter{showProgressBar}{0}
	\setcounter{showSlideNumbers}{0}

	\frame{\titlepage}

	\begin{frame}
		\frametitle{frame title here}
		\begin{enumerate}
			\item one \\
            \item two
		\end{enumerate}
	\end{frame}

	\setcounter{framenumber}{0}
	\setcounter{showProgressBar}{1}
	\setcounter{showSlideNumbers}{1}
	\section{section 1}
		\begin{frame}
			\frametitle{frame title here}
			\begin{itemize}
				\item item 1 \\
                \item item 2
			\end{itemize}
		\end{frame}
\end{document}

```

This theme was adapted from [this tutorial](http://hamaluik.com/posts/better-beamer-themes/).
