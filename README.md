# Resume Template

This was created for the benefit of students unfamiliar with git/version control and are starting out in building their resumes in college.

## Why?
The most common tool used for resumes is a word editor like Microsoft Word. It has the benefit of being convenient, accessible and generally hassle-free. 

However, this setup also has many problems

![Alt text](res/msword_problems.png?raw=true "msword_problems")

As can be seen, when you have multiple versions of your resume - or even multiple resumes for different applications, this can get really annoying without some kind of version control, which git provides. 

The second issue is that different versions of MS Word will display slightly different formatting - something you do not want. 

The third reason is that it can be difficult sometimes to have fine control over the spacing in between sections and bullet points. 

As such, this template was created as a substitute. 

## How to use?
You will first need to have a tex distribution installed. From there, you will need to ensure that all the packages used in main.tex are available.

````{verbatim, lang = "latex"}
\usepackage[utf8]{inputenc}
\usepackage[T1]{fontenc}
\usepackage{CormorantGaramond}
\usepackage[empty]{fullpage}
\usepackage{titlesec}
\usepackage{verbatim}
\usepackage{enumitem}
\usepackage[pdftex]{hyperref}
\usepackage{fancyhdr}
\usepackage{multirow}
\usepackage{xcolor}
````

Next, you will edit the contents of your resume in the various section .tex files in the contents folder. In this template I have provided examples of various resume scenarios you might face (for e.g. multiple roles at same company) and my formatting solution in latex. 

In order to ensure your contents fit nicely in a single page, you might want to play around with the first line of main.tex where you can adjust the font size. I am using 11.8 now, which fits the template contents nicely in a single page. 

## Custom sections
If you would like to have finer control of how the bullets look, the spacing, etc., you can look into main.tex where all the commands used are defined. You might want to adjust various \vspace values to create the perfect alignment and formatting you desire. 

Do take note that most of the multi-column formatting is done by using a table (left aligned on the first column and right aligned on the second).
