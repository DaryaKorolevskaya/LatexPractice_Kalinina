### LaTeX Guide

LaTeX is a language typing and layout system. Typesetting and layout systems are usually used for downloading text. The package allows you to automate many tasks of typing and preparing articles, including typing in several languages, numbering of sections and formulas, cross-references, placing illustrations and tables on a page, maintaining a bibliography, etc.


There are many programs for working with latex, however, for beginners, it will be most convenient to use the [overleaf](https://www.overleaf.com) online environment.

You can create a document with these commands

```sh
\begin{document}
.
.
.
\end{document}
```

When creating a document, you must specify the type of document - article, report or beamer. 
You can also indicate the author and date of creation of the document on the title page.

```sh
\title{Your Title}
\author{Your name}
\date{19.10.1917}
\maketitle
```
To work with text, you need commands:
`\newline` 
`\newpage` 
`\table of content` 
`\section{}` 
`\chapter{}` 
`\textbf{}` 

For center alignment, use the command:
`\begin{center}`
     
      `\end{center}`


Also in latex you can create lists and tables. 
For this, the command `begin` is used. 

```sh
\begin{tabular}{ l c r }
  1 & 2 & 3 \\
  4 & 5 & 6 \\
  7 & 8 & 9 \\
\end{tabular}
```
Example of the simple table. 

```sh
\begin{itemize}
                
                        \item 
                  
                        \begin{enumerate}
                
                              \item 
                  
                              \item ...
                  
                        \end{enumerate}
                  
                  \end{itemize}
```
Example of the list. You can create enumerated, nested and not enumerated lists. For the last option use `\begin{itemize}[noitemsep]`.
    
In order to use latex pictures in a document, a `\usepackage{graphicx}` package is required

`\includegraphics[scale=1]{pic.png}` - command to insert picture.
    
To write a bibliography use command `\begin{thebibliography}{}` and `\bibitem{}` for each source
For writing formulas you can use `\begin{equation}` and special command for mathematical symbols and actions. For example `/frac{}{}`, `\lim_{x \to 2} f(x) =`

Also you can make simple presentation in Latex. For presentation you can use this template:
```sh
\documentclass{beamer}
\usepackage[utf8]{inputenc}

\usetheme{Hannover}
\usecolortheme{default}

\hypersetup{
    colorlinks=true,
    linkcolor=black,
    filecolor=magenta,      
    urlcolor=cyan,
    pdftitle={Overleaf Example},
    pdfpagemode=FullScreen,
    }
```
To create a new slide use:
```sh
\begin{frame}
\frametitle{title}
\end{frame}
```

So, it was a very brief view on basic features of Latex. Latex has many more features, commands and tools that were not mentioned in this guide. Latex is very interesting and useful and it makes sense to study it more deeply)
