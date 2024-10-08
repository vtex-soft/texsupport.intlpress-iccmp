# LaTeX author support for the International Press book series *Proceedings of the International Consortium of Chinese Mathematicians* (*ICCMP*)

## Table of Contents

* [About](#about)
* [Package content](#package-content)
* [Setup](#setup)
* [Recomended usage of `ipbook` package](#recomended-usage-of-ipbook-package)
* [Submission](#submission)
* [Bug reports](#bug-reports)

## About

Author support service provides LaTeX style files and `*.tex` file templates designed for International Press book series
Proceedings of the International Consortium of Chinese Mathematicians (ICCMP) manuscripts.

## Package content

The following files are given in the repository (or directly in `*.zip` archive):

* `ipbook.cls` - LaTeX style files designed for International Press book series.
  Please do not change them. These files are already loaded in the respective template files;
* `iccmp-template.tex` - topmatter template (should be used for manuscript preparation);
* `iccmp-sample.tex` - book series sample article;
* `iccmp-sample.pdf` - book series sample article (`PDF` file);

## Setup
* Clone the repository or download the `*.zip` archive. Rename the package to `<your-project-name>`.
* Install `ipbook.cls` file in your TeX system (suggested directory: `ipbook`).
* Use the file `iccmp-template.tex` to start your article as a template.
* Use the file `iccmp-sample.tex` as a reference for how to prepare a topmatter of your article.

## Recommended usage of `ipbook` package

Use `iccmp-template.tex` as a template.

### Document class options

For the ICCMP journal `iccmp` option must be set
in a `\documentclass[]{ipbook}`:
```latex
\documentclass[iccmp]{ipbook}
```

### LaTeX document preamble content

The preamble of your LaTeX document should look like this:

```latex
\documentclass[iccmp]{ipbook}

\title{Title}

\author{First Author}
\address{Address of the First Author, Country}
\email{first@somewhere.com}
\thanks{First Author is supported by ...}
\author{Second Author}
\address{Address of the Second Author, Country}
\email{second@somewhere.com}

\begin{document}

    \begin{abstract}
        ...
    \end{abstract}

    \maketitle

    \tableofcontents

    Your manuscript content

\end{document}
```

## Submission

Submit one single file as a `ZIP` archive.
Pack your root folder `<your-project-name>` with files and subfolders.

## Bug reports

Please submit bug report or feature requests at
[github](https://github.com/vtex-soft/texsupport.intlpress-iccmp/issues) page.