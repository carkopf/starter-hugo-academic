# Fixing website

The problem is that some pdfs don't render properly. This became apparent first with the ICML paper. I had made a publication file for that paper, which seemed normal. But when you click on the pdf you get a greyed out page, and when you download the file, it is corrupted. 

I played around a bunch and found: 

1. When I put other pdfs in, they have similar loading problems. I often see white pages with a message about when the pdf was downloaded on the side. When I made a test pdf from iAWriter with just a few words in it, it did behave properly. 
2. When I put pdfs into the static folder and navigate there directly, they do seem to load fine. 
3. So the problem seems to be with the way that Hugo is loading pdfs stored in each publication folder.


