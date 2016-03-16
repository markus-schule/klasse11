# Online LaTeX Editoren
* https://www.sharelatex.com/
* https://www.overleaf.com/

# Erste Schritte mit LaTeX
* https://www.overleaf.com/latex/learn/free-online-introduction-to-latex-part-1.pdf

# LaTeX Wikibook
* https://en.wikibooks.org/wiki/LaTeX

# Beispiel: Erstes Dokument

```latex
\documentclass{article}
\title{Bald ist Ostern}
\author{Hans-Martin Ramsl}
\date{Maerz 2016}
\begin{document}
   \maketitle
   Dies ist ein Hello World Beispiel
\end{document}
```

# Beispiel 2: Listen

https://en.wikibooks.org/wiki/LaTeX/List_Structures

```latex
\documentclass{article}
\usepackage{blindtext}
\begin{document}
\begin{itemize}
\item \blindtext
\item \blindtext
\end{itemize}
\begin{enumerate}
\item \blindtext
\item \blindtext
\end{enumerate}
\begin{description}
\item [Ant] \blindtext
\item [Elephant] \blindtext
\end{description}
\end{document}
```

# # Beispiel 3: Fußnoten
https://en.wikibooks.org/wiki/LaTeX/Footnotes_and_Margin_Notes


```latex
\documentclass{article}
\title{Bald ist Ostern}
\author{Hans-Martin Ramsl}
\date{Maerz 2016}
\begin{document}
   \maketitle
   Dies ist ein Beispiel mit Fußnote.
   
   
   Creating a footnote is easy.\footnote{An example footnote.}
   
\end{document}
```

