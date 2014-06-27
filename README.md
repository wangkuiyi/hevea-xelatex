# Hevea XeLaTeX Template

I am going to write a book in Chinese.  I hope that I can publish its
chapters on my blog, so I can get feedback before it is printed.  This
requires that I can convert my manuscript into HTML format (for
publishing in my blog) and PDF format (for printing).

I tried to write in Emacs Org mode, Wiki and Markdown.  However, none
of them support equatons well.  So I decided to use LaTeX.

I tried several tools to convert LaTeX source into HTML, including
`htlatex` and `pandoc`.  `htlatex` does not support Chinese well, and
`pandoc` supports only few LaTeX syntax.  Finally, I decided to use
[Hevea](http://hevea.inria.fr/), which works good to me.

I use XeLaTeX to convert LaTeX to PDF.  Compared with PDFLaTeX,
XeLaTeX works better with UTF-8 and TrueType Chinese fonts.

However, Hevea and XeLaTeX have different requirements with the
preamble of LaTeX source.  So I created tempaltes for them
respectively.  These templates use LaTeX's `\input` directive to
include a LaTeX source file containing the real text.
