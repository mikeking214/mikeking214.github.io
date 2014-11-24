---
layout: article
permalink: /articles/learn-latex
title: "How to Produce Professional Documents with LaTeX"
description: "A simple guide to learning LaTeX for formatting your professional documents"
category: articles
tags: [latex, tex, xelatex, xetex, lualatex, learn, teach, yourself, how, to, how to, manual, easy, beginner, advanced, dummies, miktex, texshop, texworks, typesetting, format, professional, cv, curriculum vitae, resume, cover letter, report, paper, engineering, personal, Mike, Michael, Elliot, King, McGill]
---
*A simple guide to learning LaTeX for formatting your professional documents*

****

If you've seen a university level math or science assignment or read something published in an academic journal than you've seen the results of LaTeX, and you would likely recognize its fonts and formatting.


###What is <img style="height:30px" src="/images/latex_word.png">?

LaTeX (pronounced lay-tek, NOT lay-teks) is a free, digital typesetting system, used by professionals to produce beautiful, high-quality, publishable documents, typically in .pdf format. Rather than typing your document into a word processor, like Microsoft Word, the content of the document is written in plain text in a text editor, along with some code to provide instructions.  Everything is compiled using the LaTeX engine, which understands your code, applies the proper formatting, and outputs a professionally produced document.  LaTeX is very common in the academic world for assignments, papers, exams, and research, and is often used for resumés and books.  It requires a small learning curve, but the benefits are well worth it:

<figure>
	<img style="" src="/images/equation.png">	
	<figcaption>Navier-Stokes Equation, output in LaTeX</figcaption>
</figure>
<br>
<figure>
	{% highlight tex %}
\begin{equation}
	{\partial{\bf u}\over{\partial t}} + ({\bf u} \cdot \nabla) {\bf u} = - {1\over\rho} \nabla p + \gamma\nabla^2{\bf u} + {1\over\rho}{\bf F}
\end{equation}
	{% endhighlight %}
	<figcaption>The LaTeX code to create the equation</figcaption>
</figure>

####History
<a markdown="0" target="_blank" href="http://en.wikipedia.org/wiki/Donald_Knuth">Donald Knuth</a>, one of the most well known computer scientists to this day, wrote a series of books on computer programming in the 1970s and was so frustrated with the quality of the output by the electronic publishing tools that he spent years creating a better system.  This would become TeX, a complex system to give full control over document layout that would later be simplified by <a markdown="0" target="_blank" href="http://en.wikipedia.org/wiki/Leslie_Lamport">Leslie Lamport</a> to become the LaTeX system used today.  

###Why Use LaTeX?

#### Produce Beautiful Documents Like A Professional Publisher
What sets LaTeX apart from standard WYSIWYG (What You See Is What You Get) word processors like Microsoft Word or Open Office, is how it decides to process and format your content.  LaTeX takes the document as a whole and all its features into account and processes them through very fine-grained algorithms, to precisely format the text, paragraphs, and pages the same way a professional publishing company would.  Word processors, on the other hand, format on the fly, disregarding how the document should look as a whole and requiring the user to think about formatting as they type the content.  Any user of Word understands the frustrations of fitting paragraphs on a page, aligning text and images, referencing figures, adjusting the size and look of titles and sections, and simply undoing all the autoformatting that Word forced upon you. Each of these issues takes the user away from the task of creating written content, and the formatting will still need to be tweaked as the rest of the content is filled.  In LaTeX, you write in plain text, so the formatting is not considered when actually writing, and you simply define headers, sections, figures, and equations using commands that already have their own formatting.  

<figure class="half">
	<a target="_blank" href="/images/latex.pdf"><img style="border: 1px solid; width: 48%; margin: 2px" src="/images/latex.png"></a>
	<a target="_blank" href="/images/word.pdf"><img style="border: 1px solid; width: 48%; margin: 2px" src="/images/word.png"></a>
	<figcaption>Comparison of LaTeX and Word documents. (Sources: <a target="_blank" href="/images/LaTeX/latex.tex">LaTeX</a>, <a target="_blank" href="/images/word.docx">Word</a>)</figcaption>
</figure> 

####Advanced Features
In addition to creating beautiful text while separating content from formatting and being totally free, LaTeX has some advantages for more advanced users.  LaTeX is extremely portable as it is simply plain text, which is the most portable format, and the LaTeX system is available for every operating system.  This means that version control systems can be used, which is great for documents that are updated often, like resumes, and can be worked on by people on different operating systems.  For long documents, LaTeX does an amazing job arranging chapters, sections, references, and figures, and because it is so lightweight, crashes when documents become large are very rare (unlike Word).  An incredible number of packages have been created which add new functionality, and taking advantage of these allow for nearly unlimited control over the document's output.  The creation of math equations, elaborate tables, Gantt charts, flow charts, and even vector graphics can all be done with the available packages in LaTeX and are a quick Google search away.  

###How to Use LaTeX

#### Choose a Program
LaTeX is different from Microsoft Word and there are a few ways it can be used.  The fastest way to get started is with a web-based program that is all set up and has nothing to install. These are free for personal use, have nice interfaces, and will make it easy to learn the basics of creating LaTeX documents.  However, I recommend turning off the auto-compile feature as this will not allow you focus on the content of the work, as intended with LaTeX.  Try one of these websites, create an account, and get started.

##### Web Apps - Easiest Way to Start

* <a markdown="0" target="_blank" href="https://www.writelatex.com/">WriteLaTeX</a>
* <a markdown="0" target="_blank" href="https://www.sharelatex.com/">ShareLaTeX</a>

If you would like to work entirely on your own computer and manage all your files locally, rather than deal with the website every time, there are many free available programs. They are all very similar, but I would suggest <a markdown="0" target="_blank" href="http://sourceforge.net/projects/texstudio/?source=dlp">TeXstudio</a>.  It has some great features that make learning the language and debugging very easy, and the interface is great. These applications are installed like any other program and include all the packages you need.  If you are going to be using LaTeX for more than just a resumé, having it on your computer is ideal.  Follow the installation instructions and start a new document.

##### Programs to Compile on Your Own Computer

* <a markdown="0" target="_blank" href="http://sourceforge.net/projects/texstudio/?source=dlp">TeXstudio</a> - (Mac, Linux and Windows - Recommended!)
* <a markdown="0" target="_blank" href="http://www.tug.org/texworks/">TeXworks</a> - (Mac, Linux and Windows)
* <a markdown="0" target="_blank" href="http://pages.uoregon.edu/koch/texshop/">TeXshop</a> - (Mac only)
* <a markdown="0" target="_blank" href="http://miktex.org/download">MiKTeX</a> - (Windows only)

For the more advanced user, I recommend adding the <a markdown="0" target="_blank" href="https://github.com/SublimeText/LaTeXTools">LaTeXTools</a> compiler plugin to <a markdown="0" target="_blank" href="http://www.sublimetext.com/">Sublime Text</a> through <a markdown="0" target="_blank" href="http://wbond.net/sublime_packages/package_control">Package Control</a>.  <a markdown="0" target="_blank" href="http://www.sublimetext.com/">Sublime Text</a> is an amazing text editor with great features and customization, and with the LaTeXTools plugin, preparing large documents with many chapters, figures, and citations is a breeze.  Begin by creating a new blank text document and saving it as a .tex file.  

##### Advanced Users - Text Editor with Compiler

* <a markdown="0" target="_blank" href="http://www.sublimetext.com/">Sublime Text 2</a> - Great text editor for developers (Free unlimited trial version)
* <a markdown="0" target="_blank" href="http://wbond.net/sublime_packages/package_control">Package Control</a> - Manager for the add-ons to Sublime Text
* <a markdown="0" target="_blank" href="https://github.com/SublimeText/LaTeXTools">LaTeXTools</a> - Plugin to compile LaTeX right in Sublime Text

#### The Basics

LaTeX is a markup language, like HTML, and uses "tags" to describe formatting and structure the document.  These are typically very intuitive and should not be difficult to remember.  All tags and commands usually begin with a backslash and are followed by curly brackets.  All new tags and commands start on new lines, so spacing and tabs are irrelevant, and no notation is needed to end a line. To create a section heading, the code is simply

{% highlight tex %} \section{This Is My Section Heading} {% endhighlight %} 

When your document is compiled, this will be formatted to look like a section heading, but you don't have to worry about any specifics while you create your content.  This syntax works for many one-line commands like

{% highlight tex %}
\chapter{Chapter Title}
\section{Section Heading}
\subsection{Subsection Heading}
\subsubsection{Subsubsection Heading}
\paragraph{The Heading of a Paragraph}
\label{identifier for some item in my document} 
{% endhighlight %}

Some parts of the document require bookend tags to define what is part of that object.  This is done by creating a `\begin` and `\end` tag, and putting the content between them like this:

{% highlight tex %}
\begin{document}

	\begin{figure}
		\includegraphics[width=4in]{boat.jpg}
	\end{figure}

	\begin{equation}
		{ x_{1} = {-b + sqrt{b^{2}-4ac}} } \over {2a}
	\end{equation}

\end{document}
{% endhighlight %}

Formatting is done in a very simple manner, using a tag to begin the formatted text and brackets surrounding the text to be formatted.

{% highlight tex %}
\begin{center} % Center text (followed by \end{center} of course)
\begin{flushleft} % Left justified
\begin{flushright} % Right justified

\textbf{text} % Bold 
\textit{text} % Italic
\underline{text} % Underline

{\tiny text} % tiny font size
{\small text} % small font size
{\large text} % large font size
{\huge text} % huge font size
{% endhighlight %}

As seen above, using a percent symbol begins a comment, which should be used to describe your code to make it more clear and easier to understand later.  Everything that follows the `%` on a line of code will not be printed when the document is compiled.  I recommend using them when inserting commands that are not clear and you may forget later, or to mark sections of text for easy navigation of long documents.  Comments are also a good tool for debugging, by "commenting out" some lines rather than deleting them.

{% highlight tex %}
% \begin{figure}
%	\includegraphics[width=4in]{boat.jpg}
% \end{figure}
{% endhighlight %}

All documents will require some preamble code to set up things like document type, author, title, date, fonts, colors, symbols and any packages you want to use.  This will all be defined at the top of your code, before the `\begin{document}` tag. Document class is what always goes first and defines the type of document you are creating, which can be either an article, report, letter, book, proc, or slides. Modifiers can be added to some commands that specify details like font size, paper size, double-sided, or a titlepage.  These are added between `[ ]` brackets inside the command like this:

{% highlight tex %}
\documentclass[12pt, letterpaper]{article}
{% endhighlight %}

If your document has a title, author, or specific date, you can define it like this in the preamble:

{% highlight tex %}
\title{My First \LaTeX{} Document}
\author{My Name}
\date{\today}
{% endhighlight %}

This will all show up in the title according the default formatting dictated by the document class that you have chosen.  It is then placed into the document like this:

{% highlight tex %}
\begin{document} 
\maketitle 
	Your document content goes here
	...
\end{document}
{% endhighlight %}

#### Try it Out

Now that we've gone over the basics, let's try creating our first LaTeX document!  Type the following code into the program you have chosen:

{% highlight tex %}
\documentclass[12pt, letterpaper]{article}

\title{My First \LaTeX{} Document}
\author{Michael Elliot King}
\date{\today}

\begin{document}
\maketitle

\section{Hello World}

	Hello World!

\end{document}
{% endhighlight %}

To compile, it varies for each application, but a button like **Compile**, **Typeset**, or **PDF** should give you an output that looks like this:

<figure>
	<a target="_blank" href="/images/latex_doc.pdf"><img style="border: 1px solid; align: center; width: 48%; margin: 2px" src="/images/latex_doc.png"></a>
	<figcaption>The output for "My First LaTeX Document"</figcaption>
</figure>
<br>

Hopefully everything worked and you now have your first LaTeX document!  You can begin writing some of your own content and getting the hang of things.  

If it didn't work the first time don't worry.  It is very common to get errors in your code, for misspelled words or incorrect syntax, so inspect the log that explains the error and use the line number given to locate the mistake.  Some debugging is necessary when it doesn't recognize a part of your code, and this can be the most frustrating part.  If I forgot the second `e` in `\maketitle` on line 10, the error log will look like this: 

{% highlight tex %}
There were errors in your LaTeX source

./latex_doc.tex:10: Undefined control sequence. [\maketitl]
{% endhighlight %} 

The error should follow a similar pattern of `[filename]:[line number where error is]:[Error description]. [the incorrect content]`

#### Troubleshooting

When it comes to learning LaTeX, the answer is always a quick Google search away. It seems no matter what you want to create or what problem you run into, someone else has already found the solution.  For more concrete help, some resources are:

- <a target="blank" href="http://www.stdout.org/~winston/latex/latexsheet.pdf">The LaTeX Cheat Sheet</a> - Great tool to keep on your computer and refer to
- <a target="blank" href="http://tobi.oetiker.ch/lshort/lshort.pdf">Introduction to LaTeX by Tobias Oetiker</a> - A full length document on everything you could ever know about LaTeX
- An in-depth example of writing mathematics - The <a target="blank" href="http://www.ams.jhu.edu/~ers/learn-latex/paper.pdf">PDF</a> and the <a target="blank" href="http://www.ams.jhu.edu/~ers/learn-latex/paper.tex">LaTeX source file</a>

### LaTeXing your Resumé

LaTeX is an excellent tool for making a pedestrian resumé look polished, but starting from scratch is really tough.  A lot of LaTeX templates exist for resumés however, so I would suggest starting with one of these and customizing it to make it your own.  There are tons out there that apply to different fields and styles, but here is a list to get started: 

- <a target="_blank" href="http://github.com/mikeking214/latexresumetemplate">My own template</a>
- <a target="_blank" href="http://www.latextemplates.com/cat/curricula-vitae">LaTeXtemplates.com</a>
- <a target="_blank" href="https://www.sharelatex.com/templates/cv/">ShareLaTeX.com</a>
- <a target="_blank" href="https://github.com/smholloway/resume/blob/master/latex/resume.tex">Template by Seth Holloway</a>


I have included the template I used for my CV, which I based off  a template by <a target="_blank" href="http://nitens.org/taraborelli/cvtex">Dario Taraborelli</a>, with some help from <a target="_blank" href="jaan.io">Jaan Altosaar</a>, and customized for my needs. A great way to learn LaTeX is to study a completed document, so I have filled the template with comments to explain what does what in the code.  It is an academic resume and contains more sections than you'll need, so include only what applies to you and make changes as you please.  In addition to formatting help, I have tried to include general resumé tips I've picked up, so use those as you wish. 

######Download the template from my <a target="_blank" href="https://github.com/mikeking214/LatexResumeTemplate">GitHub page</a> and get started!######

Additionally, I am happy to answer any questions by <a target="blank" href="mailto:{{ site.owner.email }}">email</a>. 




