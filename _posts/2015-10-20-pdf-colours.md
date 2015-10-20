---
layout: post
title: PDF colours incorrect on iOS
---
PDFs for documents are often released online as well as printed.

There are rules of engagement for the use of PDFs online that aren’t always followed.  Take, by means of example to following:

![urgh](/img/Screenshot_20_10_2015__22_00.png)

This is a screengrab from a PDF released by the [European Resuscitation Council](https://www.erc.edu/).  Note the awful white text on lime green (illegible!).  Is this what they intended?  Of course not, the overall design is actually pretty impressive: what they have done is released a PDF intended for _print_ as fodder for web users.  It’s meant to look like this:

![ah](/img/Screenshot_20_10_2015__22_01.png)

Apple’s PDF viewers don’t contain a default CMYK profile, so documents built using this colour palate, the industry standard for print, show up incorrectly when viewed on Apple devices.

There are workarounds: using the Acrobat iOS app is one.  But I consider this unsatisfactory.  I don’t want to use an app for PDFs when functionality is built in to my device: I just want authors/publishers to **get it right**.

Document producers need to use sRGB (rather than CMYK) for PDFs intended for viewing on electronic devices, or the PDF colour profile can be adjusted using Acrobat:

1. Open PDF and click Tools
2. Click Tools then Optimize PDF

![screenshot1](/img/JointWelfareStatementRGB_pdf1.png)

3. Select the Preflight then Convert to sRGB option
4. Click Analyze and fix

![screenshot2](/img/Preflight_and_JointWelfareStatementRGB_pdf.png)
