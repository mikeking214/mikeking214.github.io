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

If you've seen a university level math or science assignment, or read something published in an academic journal, then you've seen the results of LaTeX and would recognize its fonts and formatting.


###What is <img style="height:30px" src="/images/latex_word.png">?

LaTeX **(pronounced lay-tek, NOT lay-tek*s*)** is a free, digital typesetting system used by professionals to produce beautiful, high-quality, publishable documents, typically in .pdf format. Rather than typing your document into a word processor, like Microsoft Word, your content is written in plain text in a text editor along with code to provide instructions.  Your content is compiled using the LaTeX engine--software that runs in the background--which interprets your code, applies formatting to your text, and outputs a professionally produced document.  LaTeX is common in the academic world for assignments, papers, exams, and research, and is often used for resumés and books.  It requires a small learning curve, but the benefits are worth it.

<figure>
	<img style="" src="/images/equation.png">	
	<figcaption>Elegantly formatted text produced by LaTeX: the Navier-Stokes Equation</figcaption>
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
<a markdown="0" target="_blank" href="http://en.wikipedia.org/wiki/Donald_Knuth">Donald Knuth</a>, a pioneer of computer science, wrote a series of books on computer programming in the 1970s and was so frustrated with the quality of the output by the electronic publishing tools that he spent years creating a better system.  This would become TeX, a complex system to give full control over document layout that would later be simplified by <a markdown="0" target="_blank" href="http://en.wikipedia.org/wiki/Leslie_Lamport">Leslie Lamport</a> to become the LaTeX system used today.  

###Why Use LaTeX?

#### Produce Beautiful Documents Like A Professional Publisher
What sets LaTeX apart from standard <a markdown="0" target="_blank" href="https://en.wikipedia.org/wiki/WYSIWYG">WYSIWYG (What You See Is What You Get)</a> word processors like Microsoft Word and Open Office is how it decides to process and format your content.  Like a publishing company, LaTeX considers the document and all its features a cohesive unit.  It processes the document through algorithms that precisely format the text, paragraphs, and pages into a complete, polished product.  Word processors, on the other hand, format on the fly. They disregard the document's complete aesthetic and require you to consider formatting as you type.  Any user of Word understands the frustrations of fitting paragraphs on a page, aligning text and images, referencing figures, adjusting the size and look of titles and sections, and undoing the autoformatting Word forced upon them. 

These issues distract you from the task of writing. LaTeX affords focusing on the content because the structure and format are defined within the text using logical commands which are *textual*, not *visual*. It requires you to consider only the content while you write and adjust formatting when you're finished.

<figure class="half">
	<a target="_blank" href="/images/latex.pdf"><img style="border: 1px solid; width: 48%; margin: 2px" src="/images/latex.png"></a>
	<a target="_blank" href="/images/word.pdf"><img style="border: 1px solid; width: 48%; margin: 2px" src="/images/word.png"></a>
	<figcaption>Comparison of LaTeX and Word documents using default formatting. (Sources: <a target="_blank" href="/images/LaTeX/latex.tex">LaTeX</a>, <a target="_blank" href="/images/word.docx">Word</a>)</figcaption>
</figure> 

####Advanced Features
LaTeX has advanced features beyond its efficiency, aesthetic, and price.  It is portable in size and compatibility; plain text files are light and the LaTeX system is available for every operating system.  This makes version control possible, which is great for documents that are updated often, like resumés and papers with multiple drafts. It also means a document can be worked on by people across different operating systems and at the same time.  

For long documents, LaTeX outperforms Word at arranging chapters, sections, references, and figures, and because it is lightweight, it won't crash when documents become large -- unlike Word.  There are also thousands of auxiliary packages that add functionality to the base LaTex system. You can create math equations, elaborate tables, Gantt charts, flow charts, and even vector graphics with the available packages. Take advantage of these for nearly unlimited control over a document's output.  A quick Google search will locate them.  

###How to Use LaTeX

#### Choose a Program
LaTeX differs from word processors in that it doesn't have a native graphical user interface, so there are a few ways it can be used.  The fastest way to start is with a web-based program that has nothing to install. These are free for personal use, have nice interfaces, and will make it easy to learn the basics of creating LaTeX documents.  However, I recommend turning off the auto-compile feature as this will not allow you to focus on the content of the work, as intended with LaTeX.  Try one of these websites, create an account, and get started.

##### Web Apps - Easiest Way to Start

* <a markdown="0" target="_blank" href="https://www.writelatex.com/">WriteLaTeX</a>
* <a markdown="0" target="_blank" href="https://www.sharelatex.com/">ShareLaTeX</a>

If you want to manage your files locally, rather than deal with the website every time, there are many free available programs. All are similar, but I would suggest <a markdown="0" target="_blank" href="http://sourceforge.net/projects/texstudio/?source=dlp">TeXstudio</a>.  It has features that make learning and debugging easy, and the interface is approachable. These applications install like any program and include all the packages you need to begin.  **If you are going to be using LaTeX for more than just a resumé, having it on your computer is ideal.**  Follow the installation instructions and start a new document.

##### Programs to Compile on Your Own Computer

* <a markdown="0" target="_blank" href="http://sourceforge.net/projects/texstudio/?source=dlp">TeXstudio</a> - (Mac, Linux and Windows - Recommended)
* <a markdown="0" target="_blank" href="http://www.tug.org/texworks/">TeXworks</a> - (Mac, Linux and Windows)
* <a markdown="0" target="_blank" href="http://pages.uoregon.edu/koch/texshop/">TeXshop</a> - (Mac only)
* <a markdown="0" target="_blank" href="http://miktex.org/download">MiKTeX</a> - (Windows only)

For the advanced user, I recommend adding the <a markdown="0" target="_blank" href="https://github.com/SublimeText/LaTeXTools">LaTeXTools</a> compiler plugin to <a markdown="0" target="_blank" href="http://www.sublimetext.com/">Sublime Text</a> through <a markdown="0" target="_blank" href="http://wbond.net/sublime_packages/package_control">Package Control</a>.  Sublime Text is an amazing text editor with great features and customization. The LaTeXTools plugin makes preparing large documents with chapters, figures, and citations a breeze.  Begin by creating a new blank text document and saving it as a .tex file.  

##### Advanced Users - Text Editor with Compiler

* <a markdown="0" target="_blank" href="http://www.sublimetext.com/">Sublime Text 2</a> - Great text editor for developers (Free unlimited trial version)
* <a markdown="0" target="_blank" href="http://wbond.net/sublime_packages/package_control">Package Control</a> - Manager for the add-ons to Sublime Text
* <a markdown="0" target="_blank" href="https://github.com/SublimeText/LaTeXTools">LaTeXTools</a> - Plugin to compile LaTeX right in Sublime Text

#### The Basics

LaTeX is a <a markdown="0" target="_blank" href="https://en.wikipedia.org/wiki/Markup_language">markup language</a> like HTML and uses "tags" to describe formatting and structure the document.  Tags are typically intuitive or at least easily remembered.  Most tags and commands begin with a backslash and are followed by curly brackets.  All new tags and commands start on new lines, so spaces and tabs are irrelevant and notation is not needed to end a line. To create a section heading, the code is:

{% highlight tex %} \section{This Is My Section Heading} {% endhighlight %} 

When your document is compiled, this will be formatted to look like a section heading.  This syntax works for many one-line commands:

{% highlight tex %}
\chapter{Chapter Title}
\section{Section Heading}
\subsection{Subsection Heading}
\subsubsection{Subsubsection Heading}
\paragraph{The Heading of a Paragraph}
\label{identifier for some item in my document} 
{% endhighlight %}

Some parts of the document require bookend tags to define the contents of the object.  This is done by creating a `\begin` and `\end` tag, and putting the content between them:

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

Formatting is done using a tag to begin the formatted text and brackets surrounding the text to be formatted:

{% highlight tex %}
\begin{center} % Center text (followed by \end{center} of course)
\begin{flushleft} % Left justified
\begin{flushright} % Right justified

\textbf{text} % Bold 
\textit{text} % Italic
\underline{text} % Underline

{\tiny text} % tiny font size - relative to the default size
{\small text} % small font size
{\large text} % large font size
{\huge text} % huge font size
{% endhighlight %}

As seen above, using a percent symbol begins a comment.  Comments -- everything that follows the `%` on a line of code -- will not be printed when the document is compiled.  Use them as hidden notes when inserting new or unclear commands, or to mark sections of text for easy navigation.  Comments are also a good tool for debugging, by "commenting out" some lines rather than deleting them:

{% highlight tex %}
% \begin{figure}
%	\includegraphics[width=4in]{boat.jpg}
% \end{figure}
{% endhighlight %}

All documents will require preamble code to set up document type, author, title, date, fonts, colors, symbols and additional packages.  This will be defined at the top of your code, before the `\begin{document}` tag. Document class always goes first to define the type of document, which can be an article, report, letter, book, proc, or slides. Modifiers are added to commands to specify details like font size, paper size, double-sided, or a titlepage.  These are added between square brackets inside the command:

{% highlight tex %}
\documentclass[12pt, letterpaper]{article} % defines an "article" style document, font size, and paper size
{% endhighlight %}

If your document has a title, author, or specific date, define it in the preamble:

{% highlight tex %}
\title{My First \LaTeX{} Document}
\author{My Name}
\date{\today}
{% endhighlight %}

This will show up in the title according to the default formatting dictated by the document class.  Insert your title with '\maketitle':

{% highlight tex %}
\begin{document} 
\maketitle 
	Your document content goes here
	...
\end{document}
{% endhighlight %}

#### Try it Out

Now that we've covered the basics, try creating your first LaTeX document.  Type the following code into a blank document:

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

Compile the code using a button like **Compile**, **Typeset**, or **PDF** -- these vary by application. Your output should look like this:

<figure>
	<a target="_blank" href="/images/latex_doc.pdf"><img style="border: 1px solid; align: center; width: 48%; margin: 2px" src="/images/latex_doc.png"></a>
	<figcaption>The output for "My First LaTeX Document"</figcaption>
</figure>
<br>

Hopefully everything worked and you now have your first LaTeX document!  Time to begin writing your own content and getting the hang of things.  

If it didn't work the first time, don't worry.  It's common to get errors in your code, for misspelled words or incorrect syntax, so inspect the log that explains the error and use the line number to locate the mistake.  Some debugging is necessary when it doesn't recognize a part of your code, which can be frustrating.  

If I forgot the second `e` in `\maketitle` on line 10, the error log will look like this: 

{% highlight tex %}
There were errors in your LaTeX source

./latex_doc.tex:10: Undefined control sequence. [\maketitl]
{% endhighlight %} 

The error should follow a similar pattern of `[filename]:[line number where error is]:[Vague error description]. [the incorrect content]`

#### Troubleshooting

If your errors are more complicated than unknown commands and spelling mistakes, go to Google.  Your questions can almost always be answered with a quick search. It seems no matter what you want to create or what problem you have, someone else has already found the solution.  For more concrete help, some resources are:

- <a target="blank" href="http://www.stdout.org/~winston/latex/latexsheet.pdf">The LaTeX Cheat Sheet</a> - A great tool to keep on your computer
- <a target="blank" href="http://tobi.oetiker.ch/lshort/lshort.pdf">Introduction to LaTeX by Tobias Oetiker</a> - A full length document on everything you could ever know about LaTeX
- An in-depth example of writing mathematics - The <a target="blank" href="http://www.ams.jhu.edu/~ers/learn-latex/paper.pdf">PDF</a> and the <a target="blank" href="http://www.ams.jhu.edu/~ers/learn-latex/paper.tex">LaTeX source file</a>

### LaTeXing your Resumé

LaTeX is an excellent tool for making a pedestrian resumé look polished, but starting from scratch is tough.  However, a lot of LaTeX templates exist for resumés, so I would suggest starting with one and customizing it.  There are tons that apply to different fields and styles, but here is a list to get started: 

- <a target="_blank" href="http://github.com/mikeking214/latexresumetemplate">My own template</a>
- <a target="_blank" href="http://www.latextemplates.com/cat/curricula-vitae">LaTeXtemplates.com</a>
- <a target="_blank" href="https://www.sharelatex.com/templates/cv/">ShareLaTeX.com</a>
- <a target="_blank" href="https://github.com/smholloway/resume/blob/master/latex/resume.tex">Template by Seth Holloway</a>


I have included the <a target="_blank" href="https://github.com/mikeking214/LatexResumeTemplate">template I used for my CV</a>, which I based on a template by <a target="_blank" href="http://nitens.org/taraborelli/cvtex">Dario Taraborelli</a>, with some help from <a target="_blank" href="jaan.io">Jaan Altosaar</a>, and customized for my needs. A great way to learn LaTeX is to study a completed document, so I have filled the template with comments to explain what does what in the code.  It is an academic resume and contains more sections than you'll need, so include only what applies to you and make changes as you please.  In addition to formatting help, I have tried to include general resumé tips I've picked up, so use those as you wish. 

######Download the template from my <a target="_blank" href="https://github.com/mikeking214/LatexResumeTemplate">GitHub page</a> and get started!######

If you spot a mistake in this article or you have something to add, please <a target="blank" href="mailto:{{ site.owner.email }}">email</a> me. 




