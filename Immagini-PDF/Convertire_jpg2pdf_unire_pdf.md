# Come comprimere un file .jpg, convertirlo in .pdf e successivamente unire i .pdf.

sudo apt install imagemagick # Installa Image Magick

mogrify -compress jpeg -quality 50% *.jpg # Comprime i file del 50%

convert *.jpg -auto-orient document.pdf # Converte i file .jpg in .pdf

pdfunite *.pdf nomefile.pdf # Unisce i diversi .pdf creati
