# This will build all the latex notes within the current directory of this makefile 
# 
# Author: Jihoon Og
# Date: 2/27/2019
# 
# Current directory in this case means the present working directory of this Makefile

# Latex compiler selection and options
LATEX=pdflatex
OPT= "-synctex=1 -interaction=nonstopmode -file-line-error"

# Build Section
# This will build all the latex files within the current directory
all:
	@for f in $(shell ls *.tex); do echo "Compiling" $${f}; ${LATEX} ${OPT} $${f}; ${LATEX} ${OPT} $${f}; ${LATEX} ${OPT} $${f}; echo "Done Compiling" $${f}; done; latexmk -c

clean:
	 latexmk -c

