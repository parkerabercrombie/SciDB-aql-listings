This package provides a language definition for the LaTeX listings
package, and adds support for SciDB's Array Query Language and Array
Functional Language.

Author: Parker Abercrombie

$ Usage

Import the style in the document preamble, and select language aql:

```latex
\usepackage{listings-aql}

\lstset{
    language=aql,
    basicstyle=\small,
    breaklines=true
}
```

Use the listing package as normal with SciDB AFL and AQL queries:

```latex
\begin{lstlisting}
select avg(evi) from mod13q1
where day_of_year <= 31
group by pixel
\end{lstlisting}
```

See demo.tex for a full working demonstration.
