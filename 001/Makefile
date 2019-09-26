ASCIIDOCTOR = asciidoctor-pdf
WORKBOOK = mariadb-001-workbook.pdf
PRESENTATION = mariadb-001-presentation.pdf
PDF = $(WORKBOOK) $(PRESENTATION)	
THEME = -a pdf-style=../theme/presentation-theme.yml

all: $(PDF)

$(WORKBOOK): workbook.adoc
	$(ASCIIDOCTOR) workbook.adoc -o $@

$(PRESENTATION): presentation.adoc
	$(ASCIIDOCTOR) $(THEME) presentation.adoc -o $@

clean:
	$(RM) $(PDF)
