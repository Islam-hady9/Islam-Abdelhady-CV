CV_TEX=../cv/Islam_Abdelhady_CV.tex
BUILD_DIR=../cv/build
DIST_DIR=../dist
ASSETS_DIR=../cv/assets

OUT_PDF=$(BUILD_DIR)/Islam_Abdelhady_CV.pdf
DIST_PDF=$(DIST_DIR)/Islam_Abdelhady_CV.pdf
PREVIEW=$(ASSETS_DIR)/preview.png

all: pdf preview copy

pdf:
	@mkdir -p $(BUILD_DIR)
	latexmk -pdf -output-directory=$(BUILD_DIR) $(CV_TEX)

# Generate a PNG of page 1 from the built PDF (needs poppler-utils)
preview: pdf
	@mkdir -p $(ASSETS_DIR)
	# create preview.png at ~1600px wide
	pdftoppm -png -singlefile -f 1 -l 1 -scale-to 1600 $(OUT_PDF) $(ASSETS_DIR)/preview

copy: pdf
	@mkdir -p $(DIST_DIR)
	@cp -f $(OUT_PDF) $(DIST_PDF)
	# ensure a minimal landing page exists
	@[ -f $(DIST_DIR)/index.html ] || printf '%s\n' '<!doctype html><title>Islam AbdElhady — CV</title><a href="Islam_Abdelhady_CV.pdf">Download CV (PDF)</a>' > $(DIST_DIR)/index.html

clean:
	@latexmk -C -output-directory=$(BUILD_DIR)
	@rm -f $(DIST_PDF)

.PHONY: all pdf preview copy clean