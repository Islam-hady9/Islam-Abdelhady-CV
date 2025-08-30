CV_TEX=../cv/Islam_Abdelhady_CV.tex
BUILD_DIR=../cv/build
DIST_DIR=../dist
OUT_PDF=$(BUILD_DIR)/Islam_Abdelhady_CV.pdf
DIST_PDF=$(DIST_DIR)/Islam_Abdelhady_CV.pdf

all: pdf copy

pdf:
	@mkdir -p $(BUILD_DIR)
	latexmk -pdf -output-directory=$(BUILD_DIR) $(CV_TEX)

copy: pdf
	@mkdir -p $(DIST_DIR)
	@cp -f $(OUT_PDF) $(DIST_PDF)

clean:
	@latexmk -C -output-directory=$(BUILD_DIR)
	@rm -f $(DIST_PDF)

.PHONY: all pdf copy clean