# Pygments lexer for SQL PL

SQL PL (SQL Procedural Language) is the DB2 implementation of ANSI SQL/PSM. This module extends the `SqlLexer` lexer of [Pygments](http://pygments.org/) to support more keywords of SQL PL.

## Installation

    $ cd pygments-sql-pl-lexer
    $ [sudo] python setup.py install

## Check if the lexer is present

Simply grep the output of the following command for `sqlpl`

    $ pygmentize -L lexers | grep sqlpl

## Use the lexer in LaTeX

Replace &lt;language&gt; with **sqlpl**:

    \begin{minted}{<language>}
        <code>
    \end{minted}

For example:

    \begin{minted}[linenos=true,frame=single]{sqlpl}
    --#SET TERMINATOR @

    CREATE OR REPLACE MODULE project @
    \end{minted}

produces

![](https://github.com/mitakas/pygments-sql-pl-lexer/blob/master/docs/example.png)
