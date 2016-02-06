[![Build Status](https://travis-ci.org/ether42/resume.svg?branch=master)](https://travis-ci.org/ether42/resume)

To build:
```shell
context_directory=ConTeXt

mkdir "$context_directory"
(cd $_
  rsync -av rsync://contextgarden.net/minimals/setup/first-setup.sh .
  sh ./first-setup.sh --modules=all --engine=luatex
)

. "$context_directory"/tex/setuptex
context resume.tex
```
