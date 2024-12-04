---
title : "Office 12, file formats"
author : "Niklas"
date : "2005-11-29"
categories : 
 - tech
---

Brian Jones has posted [this very interesting text](http://blogs.msdn.com/brian_jones/archive/2005/11/26/497226.aspx) plus [this PowerPoint-presentation](http://jonesxml.com/decks/xml2005.ppt) - which I've converted to [this flash presentation](https://niklasblog.com/wp-content/2005-11-29-XML2005) which I hope Brian will let me share - he's held at the XML 2005 conference. This presentation contains some quite interesting information concerning the Office 12 file-formats, e.g. _the default file formats to be_ when the next version of MS Office hits the streets.

Word documents have so far only popped up wearing the .doc file extension, but come Office 12, it's .docx. Anyway, I've found a load of interesting stuff in the new file format, and the most interesting bits I've found so far are these:

**1**. The new default file formats in Office 12 are in the XML-format. This means one can open files created in Office 12 through any application that handles XML; if I want to open an Office 12 database, and I don't have MS Access 12 installed, I can open it in Notepad. Or in a text-editor on a Linux-based machine. I wouldn't be able to see anything but the very raw data, but you get the idea: the new formats are to be based on open source standards, which means anybody will be able to create applications that use the XML that the Office 12-applications generate. This also means good news for developers, who no longer have to rely on the MS Office API's, but can access the files directly as they're built using open standards.

**2**. Files created through Office 12 are placed inside a "ZIP container". Now, what's that? You've probably heard of the ZIP compression-format. It's quite effective when it comes to shrinking text-files to small ones; for example, an MS Word-file of 100KB containing only text can be "zipped" to a file weighing in at just 5KB. That's what many of us are used to do, although not as much these days, as storage space is relatively cheap and bandwidth is skittling upwards. So what's the new feature? Well, Office 12 automatically zips the file. This is done _as you save your Office 12 file_. Many users and admins will probably think this is just a small feature, but consider this: as very few companies tend to prune files, i.e. delete (or store them on tape while deleting the originals) the old ones that are simply never touched, this is heaven-sent without them knowing it.

Techy detail: some think MS should use another, more effective, compression algorithm than the present one in Office 12. This would make the files smaller than if they'd use the current one. True, but using more effective algorithms will most probably we'll just have to wait and see

**3**. From Brian Jones' presentation:

> Corruption or absence of any part would not prohibit the file from being opened

I've actually not managed to make a single Office-file, that I've created in Office 12, go unusable and unrecoverable as of yet. Bog knows I've tried, but every single time - and I've tried this mostly in Word - Word has snapped up the corruption and asked me if I'd like to try to rescue the document, which has worked wonderfully every time. This will make for many happy users, especially whose who are going to upgrade from Office 97.

**4**. The new file formats will not open in Office 97. From said presentation:

> Backward Compatible: Office 2000, Office XP, Office 2003 will all support the new formats

Those users will be able to open, edit and save the new formats if they install a "patch" for this functionality. Users of Office 97, the word from MS to you is: upgrade or perish.
