# requires v0.6.6 or newer of d2lang.com
SRC = s3c-consumers.d2 \
	s3c-producers-establish.d2 \
	s3c-producers-generate.d2 \
	s3c-producers-share.d2 \
	s3c-producers.d2

PNG = ${SRC:.d2=.png}
SVG = ${SRC:.d2=.svg}

all: all-svg all-png

${PNG}: %.png: %.d2
	d2 $< $@

${SVG}: %.svg: %.d2
	d2 $< $@

all-svg: ${SVG}

all-png: ${PNG}

clean:
	rm -f *.png *.svg
