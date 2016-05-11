BUILD_DIR = build
BOOK_FILE_NAME = Mobile_business
TITLE = title.txt
METADATA = metadata.xml

CHAPTERS = \
01_Foreword.md \
02_Passion.md \
03_Product.md \
04_Metrics.md \
05_Market.md \
06_Development.md \
07_Client.md \
08_Design.md \
09_Best_Practices.md \
10_Audience.md \
11_Sharing.md \
12_Marketing.md \
13_Search.md \
14_Testing.md \
15_Monetizing.md \
16_Voice_Calls.md \
17_Company.md \
18_Investments.md \
19_Trends.md \
20_Epilogue.md


TOC = --toc --toc-depth=3
COVER_IMAGE = ../images/book_frontcover.jpeg
LATEX_CLASS = report

all: book

book: epub 

clean:
	rm -r $(BUILD)

epub: $(BUILD_DIR)/epub/$(BOOK_FILE_NAME).epub

 

$(BUILD_DIR)/epub/$(BOOK_FILE_NAME).epub: $(TITLE) $(CHAPTERS)
	mkdir -p $(BUILD_DIR)/epub
	pandoc $(TOC) -S --epub-metadata=$(METADATA) --epub-cover-image=$(COVER_IMAGE) -o $@ $^

 

.PHONY: all book clean epub 


