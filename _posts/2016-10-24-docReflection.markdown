---
layout: post
title:  "Documentation Reflection"
date:   2016-10-24
categories: "projects"
assignment: "true"
---

# Written Work
My written work is a copy of my first community event description, a list of upcoming INLS events, a few quotes about how it's important to learn how to code, and a picture of coffee that relates to coding.

# Conversion Description
On 10/22, I wrote a script that will take a markdown file and convert it to HTML, DOCX, ODT, and PDF formats. I started off the script with an if statement. I made sure that I had my if statement syntax right and then started to read in README.md as my test file. I kept getting errors. I realized that by taking in my input as README.md and using that input variable as the argument in my pandoc commands, I was creating documents like "README.md.docx". That's not what I wanted to do, so I started going through bash syntax to figure out how to get rid of parts of string variables. After I figured that out, I was able to take in a file input and extract the filename from it. My life got a lot easier after I figured that out. I had an executable script that did what the assignment needed me to do. I stopped working on this then.

On 10/24, in class, I realized that I didn't account for smart quotes, so I added the -s flag to all of my pandoc commands and put them into a function. That took me a few minutes to understand bash syntax as well because I kept calling the function with `$` in front of it. This made me get an error. After taking out the dollar sign, the script worked again. Afterwards, I realized that my error statement wasn't red, like I wanted it to be, because I forgot to add the -e tag. I added that, and everything worked like I wanted it to.

On 10/26, I tried to get my output files to put below in the list of files. The script wasn't working anymore. I was so frustrated because it was working a few days ago. It was glitching at the if statement, so I thought something was wrong with my syntax. I ended up taking out the wildcard in my string comparison, and I used a direct string comparison. To explain further, I took the file input and removed the filename, leaving only the file extension. For example, if a user types in `README.docx`, the if statement will only read the `docx` portion, see that it is not equal to `md`, and produce an error.

# List of Files
## Click on filename to get to connecting Github page
1. Source: [commEventToConvert.md](https://github.com/inls161/assignment-3-pillaim/blob/5489558d33704c6939ae7f7e14aabb87a551fa24/commEventToConvert.md)
2. Output: [commEventToConvert.doc](https://github.com/inls161/assignment-3-pillaim/blob/ff8f2b6276999f290f9d28cdcff8a157bdac905b/commEventToConvert.docx)
3. Output: [commEventToConvert.html](https://github.com/inls161/assignment-3-pillaim/blob/ff8f2b6276999f290f9d28cdcff8a157bdac905b/commEventToConvert.html)
4. Output: [commEventToConvert.pdf](https://github.com/inls161/assignment-3-pillaim/blob/ff8f2b6276999f290f9d28cdcff8a157bdac905b/commEventToConvert.pdf)
5. Output: [commEventToConvert.odt](https://github.com/inls161/assignment-3-pillaim/blob/ff8f2b6276999f290f9d28cdcff8a157bdac905b/commEventToConvert.odt)

# Script
## Click on filename to get to connecting Github page
- [pillaim-convert-docs.sh](https://github.com/inls161/assignment-3-pillaim/commit/0309cab0863296de9a3d723c25887657d20b82d0)

