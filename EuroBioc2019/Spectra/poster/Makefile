## posterdown needs pagedown which needs Google Chrome/Chromium installed to
## convert html to pdf
## on Debian: apt install chromium
poster.pdf: poster.Rmd
	R --vanilla --silent -e "pagedown::chrome_print('poster.Rmd')"
