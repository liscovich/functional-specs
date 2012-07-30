latex input:		mmd-article-header  
Title:				Sample MultiMarkdown Document  
Base Header Level:	2  
latex mode:			memoir  
Keywords:			MultiMarkdown, Markdown, XML, XHTML, XSLT, PDF   
CSS:				fspecs.css	
xhtml header:		<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML">
</script>
copyright:			2011 Fletcher T. Penney.  
					This work is licensed under a Creative Commons License.  
					http://creativecommons.org/licenses/by-nc-sa/3.0/  
latex input:		mmd-natbib-plain
latex input:		mmd-article-begin-doc  
latex footer:		mmd-memoir-footer  



# Player Site

Players (subjects) play games on the Popper Player Website to contribute to social science research. Most social science experiments are currently run in social science laboratories, where players type information into a screen like the following.

<!---z-tree screenshot-->
## Audience 

Researchers recruit subjects from three sources: 

1. Online labor markets, like [Amazon Mechanical Turk](https://www.mturk.com/mturk/welcome) and [oDesk](www.odesk.com).
2. Their own subject pools.
3. Visitors who independently come to the Popper Player Site.

# Accounts

All players must have an account to play games on the Popper Player Website, since demographic information about the player, like age and sex, are usually necessary for the researcher to interpret results. Players cannot be anonymous. On the same token, player confidentiality is important and researchers should not know all information about their subjects. Player privacy, especially their names, should be protected so that players feel that they are making decisions in the game safely without the risk of stigma or judgment. For example, a player who chooses to "betray" other players in a game should be able to do so without worrying that the researcher or other players would be able to identify them in real life. 

## Log In

The landing page of the Popper Player Website is a Log In page. Players should not be able to see games unless they log in with a verified Popper account. <!--- internal link-->

Players must log in by using their Facebook account. We want to make sure that demographic information associated with each player is as accurate as possible, which is easier if the player logs in using an account linked with his real identity. Logging in with a Facebook account also reduces the amount of demographic information that the player has to provide manually, since the Player Site can pull the player's name, age, and sex from the player's Facebook account. The player is notified with a message on the Log In page that his individual choices in a game (for example, defection or cooperation) will never be publicized. This assurance is necessary so that the player does not alter his behavior based on the possibility that his friends will see how he played certain games.

We are considering making the background of the Log In page a blurry version of the Lobby, to give players an idea of what lies in the Player Website.

## Sign Up

The player is taken through the standard Facebook authorization process, and must allow Popper to post messages on the player's timeline saying that the player just played game XYZ. If the Player Website is unable to pull certain information from the player's Facebook page, the player sees a final screen, which asks the player to provide an age and sex so that the player is served a list of games that match the player's demographics. Other more detailed information is solicited from games on an as-needed basis, before the player begins the game.

Like the Log In page, the Sign Up page should feature the same blurry version of the Lobby.

# Lobby

The lobby is a dynamic gallery of every game that fits a player's demographic information. It features two types of games: non-paying and paying. Non-paying games are two stock games that we hope to develop, that attract and retain a core group of players. The purpose of non-paying games is to provide players with an available game even when no trials are running. At least initially, we anticipate that the Player Site will not feature a paying game 24/7. Hosting two 24/7 games thus appeals to the third type of subject mentioned above, those who independently come to the Player Site. 

Players see the following information about each game:

- Payoff range
- Brief description, provided by the researcher
- Number of participants
- Time stamp of when the trial was initiated
- A button to play the game

When the player clicks the play button, the Player Site checks whether the player's available demographic information matches what the researcher is looking for and asks the player to enter any additional demographic information that the researcher needs. These answers are then stored in the user's account and cannot be manually altered by the player. If the player's information does not match what the researcher is seeking, the player is alerted that he does not qualify for the game. We would like to minimize how often players see this message. As a player fills out more questionnaires prior to playing a game, more information will be gathered about the player and unsuitable games will not be displayed to the player in the first place. 

If the player selects a paying game but has not entered payment information (in order to get paid), the player is redirected to the Profile, where he can enter information to link his Popper account with his PayPal, Amazon Mechanical Turk, or oDesk account.

# Game

The game page is an imbedded iframe featuring the client, which is designed by the researcher.

# Player Profile

The player profile features the individual's name and payment information. Details like age and sex cannot be altered once the player has provided it or once it has been pulled from Facebook. In order to get paid, a player can enter his PayPal, Amazon Mechanical Turk, or oDesk information. 

# About

The About page is static and features a description of the Player Site and how players contribute to social science research by playing games. 




# Introduction  

As I  add increasing numbers  of features to  MultiMarkdown, I decided  it was
time to create  a sample document to  show them off. Many of  the features are
demonstrated in the [MultiMarkdown User's Guide][], but some are not.

Additionally,  it's easy  for those  features to  get lost  within all  of the
technical  documentation.  This document  is  designed  to *demonstrate*,  not
describe, most of the features of MultiMarkdown.


[MultiMarkdown User's Guide]: http://fletcherpenney.net/mmd/users_guide/
  "MultiMarkdown User's Guide"


# How to Use This Document #

I suggest comparing  the raw text source with the  various final outputs (e.g.
HTML, LaTeX,  PDF, OpenDocument)  in order  to see  what can  be accomplished.
There  will be  many  similarities  between output  formats,  but  also a  few
differences. Tables will end up in different places. Paragraphs won't break in
the same way. But these differences are superficial and are a result of trying
to optimize  each format,  without regard to  identical output  across formats
(which would be virtually impossible).

Remember, the main goal of Markdown\MultiMarkdown  is to allow you to create a
document in  plain text,  with minimal  distraction from  markup, that  can be
transformed into a variety of high quality outputs. Or, to quote John Gruber:

> The overriding design goal for Markdown's formatting syntax is to make it as
readable as possible. The idea is that a Markdown-formatted document should be
publishable as-is,  as plain text,  without looking  like it's been  marked up
with  tags  or  formatting  instructions. While  Markdown's  syntax  has  been
influenced by several existing text-to-HTML filters, the single biggest source
of  inspiration   for  Markdown's   syntax  is  the   format  of   plain  text
email.[#Gruber]


[#Gruber]: John Gruber.  Daring Fireball: Markdown. [Cited January 2006]. 
  Available from <http://daringfireball.net/projects/markdown/>.


# Where Can I Get a Copy? #

You can download a zipfile containing multiple formats of this document:

* [MultiMarkdown-Gallery](http://fletcher.github.com/MultiMarkdown-Gallery)


This file includes:

*	A plain text file in MultiMarkdown format
*	A Scrivener file
*	An HTML file
*	A PDF
*	An OpenDocument file
*	An OPML
*	A LaTeX file
*	And the included images

All files were generated automatically from the MultiMarkdown source document.


# So, What Can This Document Demonstrate? #


## Metadata ##

First, take  a look  at the  overall structure  of the  document. At  the very
beginning  is  metadata,  including   a  title,  author,  keywords,  copyright
information, etc.  Where possible,  this metadata is  put to  appropriate use,
otherwise it is  stored in a format  designed to be easily  read and minimally
distracting:

* In plain text and XHTML snippets[^snippets], it is located at the top of the
  document.

* In a full XHTML document, is located in the `<head>` section, and the title
  and CSS metadata, if present, are used appropriately.

* In a PDF generated from my XSLT files, metadata is used to generate the
  appropriate fields (title, author, keywords) in the PDF itself. Some PDF
  readers will let you examine this data. Additionally, the title, subtitle,
  author, and copyright are placed at the beginning of the document.

* In a Scrivener document, you can put the metadata in the first File in the
  Binder, but the preferred location is in the "MultiMarkdown Settings..."
  pane (in the File Menu.)

There are a lot of standard metadata keys  that can be used, or you can create
your own and use them as you see fit. Definitely a powerful feature.

[^snippets]: An XHTML  snippet is my terminology for XHTML  code that does not
include the `<html>`, `<head>`, and  `<body>` tags. Most browsers will display
it  properly, but  it is  not a  complete XHTML  document. Without  a `<head>`
section there is nowhere to put metadata(e.g. there is no `<title>`).


## Structure ##

The next thing  to look at is  the overall structure of the  document. You can
visualize  a Markdown  document as  an  outline, with  different sections  and
different levels within those sections. Based on your output format, these can
be used to generate headers, or sections,  or even chapters. It's all based on
what tools you use to process the XHTML output.

Even within the XHTML document, however, you can make use of this structure to
allow  easy navigation  within  the document.  You can  link  directly to  the
[Introduction][] (and to [][Introduction] when using LaTeX), for instance. And
if you are creating  a PDF, it will contain a hierarchy  of section names that
you  can use  to  allow easy  navigation,  if your  PDF  reader supports  this
function.


## Footnotes ##

Footnotes are  very easy to  implement in  MultiMarkdown, as described  in the
MultiMarkdown Syntax Guide.[^somesamplefootnote]

[^somesamplefootnote]: Here is the text of the footnote itself.


## Tables ##

Tables  can be  quite useful  for  showing data  in  a meaningful  way. As  an
example, here is a table comparing [MultiMarkdown vs. Crayons][].


[This is a caption with *italics*][MultiMarkdown vs. Crayons]  
| Features                          | MultiMarkdown |  Crayons |  
----------------------------------- | :-----------: | :------: |  
Melts in warm places                |       No      |    Yes   |  
Mistakes can be easily fixed        |      Yes      |    No    |  
Easy to copy documents for friends  |      Yes      |    No    |  
Fun at parties                      |  No[^parties] | Why not? |  

Minimum markup for maximum quality? |      Yes      |    No    |  



[^parties]: I guess it depends on what kind of parties you go to...


## Typographical conventions ##

By incorporating John Gruber's [SmartyPants][] program into your workflow, you
can generate more  "correct" typographic punction in your XHTML  pages, and in
your  LaTeX source  if  you are  generating PDF's---this  includes  en and  em
dashes, and ellipses....

Very nice when you want to focus on writing, not grammar.


[SmartyPants]: http://daringfireball.net/projects/smartypants/


## Image Support ##

If you choose to incorporate images in your documents, this can be easily done
as well. MultiMarkdown  makes it easier to link to  images and include various
attributes.

As   an  example,   here  is   an  image   from  my   website  ---   [Nautilus
Star](#nautilusstar). If you  have a local copy of the  image, you can include
the image in a pdf.

![This is a **bolded** caption][Nautilus Star]

[Nautilus Star]: Nautilus_Star.png "Nautilus Star" width="3in" height="2.4in"


## Bibliography Support ##

MultiMarkdown offers  several mechanisms  for managing bibliographies.  It has
built-in  support   for  basic   citation  and  bibliography   management  and
formatting, or you  can rely on external  tools to handle this  for you. There
aren't  many  citations in  this  document,  but I  think  it  gets the  point
across.[p. 42][#fake]


[#fake]: John Doe. *A Totally Fake Book*.  Vanity Press, 2006.


## Glossary Support ##

MultiMarkdown  has  a  special  format for  footnotes  that  should  represent
glossary terms. This  doesn't make much difference in XHTML  (because there is
no such thing as a glossary in XHTML),  but can be used to generate a glossary
within LaTeX documents.

For example,  let's have  an entry for  `glossary`.[^glossary] And  what about
ampersands?[^amp]

Since we  want the ampersand  entry to  be sorted with  the a's, and  not with
symbols, we put in the optional sort key `ampersand` to control sorting.

	[^glossary]: glossary: Glossary 
		A section at the end ...
		
	[^amp]: glossary: & (ampersand)
		A punctuation mark ...

[^glossary]: glossary: Glossary 
	A section at the end ...

[^amp]: glossary: & (ampersand)
	A punctuation mark ...


## Math Support ##

It's pretty easy to include mathematical equations:

\\[ {e}^{i\pi }+1=0 \\]

\\[ {x}_{1,2}=\frac{-b\pm \sqrt{{b}^{2}-4ac}}{2a} \\]


You can also include formulas within a sentence, such as
\\({x}^{2}+{y}^{2}=1\\).


# Now What? #

Get out there and try it. Let me know what you think. Let me know what doesn't
work. Let me know what you think is missing.

In other words, help me make it better!

You can get more information on my web site:

*	<http://fletcherpenney.net/multimarkdown>

You can also:

* Email me:  
	<mailto:owner@fletcherpenney.net>

* Join the MultiMarkdown discussion list:  
	<http://groups.google.com/group/multimarkdown>

* Join the Markdown discussion list:  
	<http://six.pairlist.net/mailman/listinfo/markdown-discuss>