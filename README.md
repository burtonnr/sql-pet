# SQL Pet Tutorial

**Table of Contents**

1. [Project organization](#project-organization)
1. [Book](#book)
1. [Prerequisites](#prerequisites)
1. [Packages used in the book](#packages-used-in-the-book)
1. [How to contribute](#how-to-contribute)
1. [Code of Conduct](#code-of-conduct)
1. [License](#license)

## Project organization

* Meeting agenda items go here: https://github.com/smithjd/sql-pet/projects/1
* Kanban is here: https://github.com/smithjd/sql-pet/projects/2 
* Slack: [self-invite is here](http://pdxdata.org/slack/)

## Book

* Tutorial materials from this repo go in the online book, "[Exploring Enterprise Databases with R: A Tidyverse Approach](https://smithjd.github.io/sql-pet/)".
* Each chapter is written so it can be executed independently once the Docker container is built in Chapter 5. We are using a [Knit-then-Merge](https://bookdown.org/yihui/bookdown/new-session.html) approach, so each chapter of the book can be Knitted separately.  
* The book depends on the [sqlpetr](https://github.com/smithjd/sqlpetr) package, which can be installed using:

    `remotes::install_github("smithjd/sqlpetr", force = TRUE, quiet = TRUE, build = TRUE, build_opts = "")`

## Prerequisites
You will need:

* A computer running one of:
  + macOS; or
  + Any Linux distribution that will run [Docker Community Edition](https://hub.docker.com/search/?type=edition&offering=community), [R](https://ftp.osuosl.org/pub/cran/), and [RStudio](https://www.rstudio.com/products/rstudio/download/); or
  + Windows, where version 10-Pro is recommended, but at least Windows 7 64-bit or later.
* Current versions of [R and RStudio](https://www.datacamp.com/community/tutorials/installing-R-windows-mac-ubuntu)
* [Docker](https://www.docker.com/)

## Packages used in the book

Here are the R packages that are used in this project and are discussed in the book:

* [DBI](https://cran.r-project.org/package=DBI)
* [DiagrammeR](https://cran.r-project.org/package=DiagrammeR)
* [RPostgres](https://cran.r-project.org/package=RPostgres)
* [dbplyr](https://cran.r-project.org/package=dbplyr)
* [devtools](https://cran.r-project.org/package=devtools)
* [downloader](https://cran.r-project.org/package=downloader)
* [glue](https://cran.r-project.org/package=glue)
* [here](https://cran.r-project.org/package=here)
* [knitr](https://cran.r-project.org/package=knitr)
* [skimr](https://cran.r-project.org/package=skimr)
* [tidyverse](https://cran.r-project.org/package=tidyverse)
* [sqlpetr](https://github.com/smithjd/sqlpetr) (installs with: `remotes::install_github("smithjd/sqlpetr", force = TRUE, quiet = TRUE, build = TRUE, build_opts = "")`)
* [bookdown](https://cran.r-project.org/package=bookdown)

## How to contribute
If you'd like to contribute to this project, start by searching through the [issues](https://github.com/smithjd/sql-pet/issues) and [pull requests](https://github.com/smithjd/sql-pet/pulls) to see whether someone else has already raised a similar idea or question.

If you don't see your idea listed, and you think it fits into the goals of this project, do one of the following:

* If your contribution is minor, such as a typo fix, open a pull request.
* If your contribution is major, such as a new learning module or a significant restructuring of current code and training material, start by opening an issue first. That way, before you do any work, other people can weigh in on the discussion to make sure that your goals are aligned with the direction of the project.

We provide more guidelines for coding style and developer's workflow in the [Contributing](https://github.com/smithjd/sql-pet/blob/master/Contributing.md) document. The [project wiki](https://github.com/smithjd/sql-pet/wiki) is also a good source of information for developers.

To compile the book, you need to [install webshot](https://bookdown.org/yihui/bookdown/html-widgets.html), so that HTMLwidgets are displayed properly:

```
   install.packages("webshot")
   webshot::install_phantomjs()
```

Then run the [build_book.R](./build_book.R) script to compile the book.

## Code of Conduct
If you plan to participate in the project in any way, such as a developer, reviewer, contributor, committer, or student, you are expected to follow the project's [Code of Conduct](https://github.com/smithjd/sql-pet/blob/master/CODE_OF_CONDUCT.md). Please review those guidelines before choosing to participate in the project.

## License
Software in this project is licensed under the [MIT License](https://github.com/smithjd/sql-pet/blob/master/LICENSE).
