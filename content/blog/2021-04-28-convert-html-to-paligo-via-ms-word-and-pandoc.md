---
title : "Convert HTML to Paligo via MS Word and pandoc"
author : "Niklas"
date : "2021-04-28"
categories : 
 - ms-office
 - tech
---

![drawing](https://niklasblog.com/wp-content/Share-ideas.png)

I love to use [pandoc](https://pandoc.org/) to convert files.

I have found a way to convert Microsoft Word files to a [DocBook](https://docbook.org/) format that [Paligo](https://paligo.net/) accepts, although it does leave a lot to be desired.

Bugs that I'm aware of:

- Numbered list entries all have '1' as number
- Images are not imported (no big surprise here, perhaps)

Requirements:

- MS Word
- pandoc
- Web browser

Please feel free to improve on this:

1. Open the HTML that you want to copy in a browser.
2. Select all that you want to copy.
3. Ctrl+C.
4. Open MS Word.
5. Create a new document.
6. Ctrl+V.
7. Save the document in the .docx format. Pick a file name without space characters.
8. Open pandoc.
9. In the folder where you have saved the .docx file, enter:  
      
    pandoc -f docx -t docbook -o newfile.dbk --standalone wordfile.docx  
      
    Note: swap 'wordfile.docx' for the name of your file.
10. Hit your enter button.  
      
    Pandoc has now created the newfile.dbk file.
11. Rename the file to 'newfile.xml'.
12. Compress it to .zip.
13. Open Paligo.
14. Pick a location where you want to import the file.
15. Hover your mouse over the location and select the ellipsis.
16. Select **Import content**.
17. Select **Docbook 4 (.xml)**.
18. Select **Select file** and the file that you compressed in step 12.
19. Select **OK**.

The contents are now imported into a publication. In other words, _only_ a publication will exists and contain content.
