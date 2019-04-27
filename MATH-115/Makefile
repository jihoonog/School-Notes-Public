# This will build all the latex notes within the current directory of this makefile 
# 
# Author: Jihoon Og
# Date: 2/27/2019
# 
# Current directory in this case means the present working directory of this Makefile

# Latex compiler selection and options
BUILDER=rubber
OPT=--synctex --pdf -v
SOURCE=MATH-115-Notes

# Build Section
# This will build all the latex files within the current directory
all: | print full

# This will build a print friendly version of the notes, i.e. no paper background
print:
	sed -i -e 's/bg=full/bg=print/' ${SOURCE}.tex
	${BUILDER} ${OPT} --jobname ${SOURCE}-print $(SOURCE)

# This will build with the full background 
full:
	sed -i -e 's/bg=print/bg=full/' ${SOURCE}.tex
	${BUILDER} ${OPT} --jobname ${SOURCE}-full ${SOURCE}

# this will clean everything except for the pdfs
clean:
	$(BUILDER) --clean ${SOURCE}
	${BUILDER} --jobname ${SOURCE}-print --clean  $(SOURCE)
	${BUILDER} --jobname ${SOURCE}-full  --clean $(SOURCE)