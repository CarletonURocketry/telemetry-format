TARGET=data_logging_format

# $(TARGET).pdf is phony so that we always call latexmk
.PHONY: $(TARGET).pdf all clean

all: $(TARGET).pdf

$(TARGET).pdf: $(TARGET).tex
	latexmk -pdf -pdflatex="pdflatex -interaction=nonstopmode" -use-make $<

clean:
	latexmk -CA

