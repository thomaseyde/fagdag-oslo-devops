all: html pdf dslides

html: devops-intro.md
	pandoc -s --mathjax -t revealjs -o devops-intro.html devops-intro.md -V revealjs-url=./reveal.js  --slide-level=2 -V theme=solarized

pdf:
	pandoc -s -o devops-intro.pdf devops-intro.md

dslides:
	pandoc -s --mathml -i -t dzslides -o devops-intro-dslides.html devops-intro.md
