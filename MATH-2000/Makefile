# This will build all the latex notes within the current directory of this makefile 
# 
# Author: Jihoon Og
# Date: 2/27/2019
# 
# Current directory in this case means the present working directory of this Makefile

# Latex compiler selection and options
BUILDER=rubber
OPT=--shell-escape --synctex --pdf -v
# The main .tex file without the .tex
SOURCE=MATH-2000-Notes

# Build Section
# This will build all the latex files within the current directory
all: | print full

# This will build a print friendly version of the notes, i.e. no paper background
print:
	sed -i -e 's/bg=full\|bg=none/bg=print/' ${SOURCE}.tex
	${BUILDER} ${OPT} --jobname ${SOURCE}-print $(SOURCE)
	sed -i -e 's/bg=print/bg=none/' ${SOURCE}.tex


# This will build with the full background 
full:
	sed -i -e 's/bg=print\|bg=none/bg=full/' ${SOURCE}.tex
	${BUILDER} ${OPT} --jobname ${SOURCE}-full ${SOURCE}
	sed -i -e 's/bg=full/bg=none/' ${SOURCE}.tex


# this will clean everything except for the pdfs
clean:
	$(BUILDER) --clean ${SOURCE}
	${BUILDER} --jobname ${SOURCE}-print --clean  $(SOURCE)
	${BUILDER} --jobname ${SOURCE}-full  --clean $(SOURCE)
	cd Chapters ; latexmk -C ; *.synctex.gz ; cd ..
