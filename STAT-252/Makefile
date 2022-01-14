# This will build all the latex notes within the current directory of this makefile 
# 
# Author: Jihoon Og
# Date: 2/27/2019
# 
# Current directory in this case means the present working directory of this Makefile

# Latex compiler selection and options
BUILDER=rubber
OPT=--synctex --pdf -v --shell-escape
# The main .tex file without the .tex
SOURCE=STAT-252-Notes

# Build Section
# This will build all the latex files within the current directory
all: | full 


# This will build with the full background 
full:
	${BUILDER} ${OPT} --jobname ${SOURCE} ${SOURCE}


# this will clean everything except for the pdfs
clean:
	$(BUILDER) --clean ${SOURCE}
	${BUILDER} --jobname ${SOURCE} --clean  $(SOURCE)
