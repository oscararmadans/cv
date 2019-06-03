# Init server
hugo server -w

# Build
hugo --buildDrafts=true --theme=hugo-orbit-theme --destination=docs

# wkhtmltopdf 
#C:\Program Files\wkhtmltopdf\bin
wkhtmltopdf https://oscararmadans.github.io/cv/ ./docs/cv.pdf

# FireShot extension
chrome --headless --print-to-pdf="C:\\oarmadan\\hugo_0.55.1\\git\\cv\\docs\\index.pdf" https://oscararmadans.github.io/cv/

