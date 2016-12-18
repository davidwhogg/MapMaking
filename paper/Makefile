LATEX       = pdflatex
CHECK_RERUN = grep "Rerun to get" $*.log

all: l1l2.pdf

%.pdf: %.tex
	${LATEX} $<
	( ${CHECK_RERUN} && ${LATEX} $< ) || echo "Done."
	( ${CHECK_RERUN} && ${LATEX} $< ) || echo "Done."
