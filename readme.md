[![Build Status](https://travis-ci.com/ether42/resume.svg?branch=master)](https://travis-ci.com/ether42/resume)

To build:
```shell
context_directory=ConTeXt

mkdir "$context_directory"
(cd "$_"
  # http://minimals.contextgarden.net/setup/
  rsync -ptv rsync://contextgarden.net/standalone/setup/first-setup.sh .
  ./first-setup.sh --modules=all --engine=luatex
)

. "$context_directory"/tex/setuptex
context resume.tex
```
