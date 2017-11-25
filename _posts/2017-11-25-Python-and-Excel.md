---
layout: post
title: "Python and Excel"
date: 2017-11-25
---

I never learned Python in my degree (Computer Science), but I used it a few times in school and at work and 
was always amazed at how easy it made tasks. With the goal of increasing my Python proficiency, I am spending 
time coding whatever I can in Python. Yesterday I learnt that you can interact with Excel and OpenOffice Calc in Python!

its as easy as... 
<p>
  <code> import openpyxl </code>
  
  <code> wb = openpyxl.load_workbook('NAME.xlsx')</code>
  
  <code> sheet1 = wb.get_sheet_by_name('SHEET_NAME') </code>
  
  you can do whatever data analytics and transformations your heart desires! 

<p>
I'm a little too excited about this revelation...
