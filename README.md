## Introduction

Hi. Here at GitHub I'm phdonner, but on most other platforms I use the signature pdonner. My native language is Swedish, but I was born in Tampere which is a predominantly Finnish city. Therefore most of us had bilingual competence as a gift. That's a good start in learning English, German, French, Spanish, Kiswahili... many languages.

I've been working quite a lot in English speaking communities, but unidiomatic use of English will hopefully still be excused. If you have time to [write to me](https://github.com/phdonner/phdonner/blob/main/README.md#contact-information), you can be confident that politely expressed corrections will be most gratefully received.

---

## The village network cooperative

Right now my primary occupation is development of fiber optic network maintenance systems and tools. I'm doing more or less full-time voluntary work for our rural network cooperative: Luoteis-Kuhmon kyläverkko-osuuskunta, which operates in the north-western part of Kuhmo municipality, at the Russian border right on the middle latitude of Finland. Currently, the cooperative is preparing a smart rural project. Please study the cooperative's [Smart Rural 27 pages](https://nettinoste.fi/wp/category/smart-rural-27/), in case you would like to have a look at the preparatory work that we have been doing. The pages are a mix of Finnish and English content, but most often with summaries in both directions. [Multilingual methods](https://github.com/phdonner/phdonner/blob/main/README.md#multilingual-markdown) are actually one of the themes of this site.

![Nettinoste banner](https://nettinoste.fi/wp/wp-content/uploads/2014/05/copy-header_1260_240.png)

---

## How to convert Markdown to HTML with PowerShell?

I would like to collaborate with developers who would be willing to contribute in transforming PowerShell automation into a way of empowering rural developers. It could be important to state an example of how bottom-up oriented, open-source voluntary collaboration can be a smart concept which wins over passivating, profit-based top-down work. Here I'll start quite modestly by producing a simple test case. It is a bilingual tutorial on methods of setting up a low-cost computer environment, which enables rural developers to produce HTML pages. This task will be achieved without resorting to commercial services, such as Facebook or WhatsApp. Let's see where the project takes us.

Planning is a conceptual activity. To be effective, we are trying to outline a workflow which will guide our work. The next subheadings are a list of some of the topics and immediate tasks that we are facing right now.

```mermaid
flowchart LR
    id1(Visual Studio Code)
    id2(Git and GitHub)
    id3(Markdown)
    id4(Powershell)
    id5(HTML)
    id1-->id2-->id3-->id4-->id5
```

---

## Visual Studio Code

Before the appearance of the open-source Linux operating system, Microsoft Windows was by far the most appealing platform for software developers. With a low license fee the entrance threshold was low. With COM-based technologies MS made a leap into easy-going development of automated systems. Dependency on proprietary arrangements is, however, in the long run a stumbling block for any non-profit oriented developer. Therefore, the initiative to place both the Visual Studio IDE and the PowerShell scripting environment into the domain of open-source and cross-platform development were most welcome moves.

---

## Git and GitHub

At GitHub I’m currently trying to discover how Git, GitHub and related open-source tools and services could be beneficial in information society construction. This is an experimental site. So please, don't expect that the content would be static somehow. On the contrary: If the structure and the content develops dynamically, then that could be taken as a sign of active and perhaps even productive work.

---

## Markdown

Our project is based on the assumption that we are experiencing the first phases of an emerging mode of production. In the information society, the major aspects of production are dependent on information technology. We don't want to be spectators of that process, but active agents. Deep understanding and early adoption of the new tools can be an asset in rural, scarcely populated environments.

Markdown is an asset in information society construction. Apart from providing ways of organizing the content of individual documents, it is very handy in preparing web pages, writing email, making task lists and so forth. [Learn the 10 basic notations](https://www.markdownguide.org/basic-syntax/) and you will quickly discover quite a number of real life applications.

Have a look at the [GitHub Markdown sample page](https://gist.github.com/rt2zz/e0a1d6ab2682d2c47746950b84c0b6ee) and push the 'Raw' button to see the source.

---

## Comments in Markdown

One of the first observations I made while outlining the concept framework, was the fact that the author of the language hadn't provided a way of commenting Markdown content. It could be useful to have a way of jotting down preliminary thoughts, interesting sources and of course comments to be remembered by the author, but which wouldn't be shown to readers of the rendered document. There is an [interesting discussion on this topic](https://stackoverflow.com/questions/4823468/comments-in-markdown) at the Stack Overflow site which could be followed up by further debate and additional experiments.

---

## Multilingual Markdown

In line with earlier work, the tutorial will be published at least in English and Finnish. This is not a unique undertaking, but the aim presents a couple of challenges. It is assumed that this problem has already been tackled in the GitHub community. After assessing those solutions, an attempt will be made to define a set of good practices to be used in other aspects of the project. Perhaps we will be able to reproduce the content in other languages, as well.

---

## Emoji fonts in Markdown and on WWW pages

When I started this README I received a lot of redundant images, which looked like emoji ;) symbols. It would, however, be nice to know where all these decorative characters are coming from: 😕 👔 👗 👋 🌱 🐶 🌼 🌻. OK, some of them are provided with Microsoft Windows 11 Segoe UI Emoji font and similar projects (cf. [Emoji Objects](https://emojipedia.org/objects), [Open Source OpenMoji](https://openmoji.org/) contains literally thousands of them). 

As you can see: Here at GitHub the emoji characters can be embedded straight into the Markdown source document. For the time being, these fonts aren't apparently portable out of the box. While experimenting with this interesting resource you may discover that the characters are sometimes rendered with colors, and sometimes in black and white. The meaning of some of the mini sized images may be a bit difficult to figure out. Therefore mastering Markdown font sizes matters. Meanwhile, we should also validate that our solution renders Emoji characters correctly in other environments, outside GitHub.

---

## Mermaid diagrams in Visual Studio Code and on GitHub

GitHub supports a convenient Markdown inspired way of creating the mindmaps needed during our planning. It is called *Mermaid*. You can design diagram in many flavors: mindmaps, flow charts, sequence diagrams, Git Graphs etc.. Again, many of the mermaid notations are rather easy to learn (cf. the [Mermaid cheat sheet](https://jojozhuang.github.io/tutorial/mermaid-cheat-sheet/) at the Jekyll site). Study the markdown code behind the example diagram by copying it to text processor. You'll see that the basic symbols are quite easy to learn.

```mermaid
mindmap
    Shapes
        Default
        [Square]
        (Rounded)
        ((Circle))
        ))Bang((
        )Cloud(
        {{Hexagon}}
```

This diagramming and charting functionality depends on JavaScript. In order to use such mindmaps outside GitHub, we would need to know how the package is installed on the local machine and on our web server.

---

## PowerShell

PowerShell is a scripting language created by developers at Microsoft, but nowaday maintained by an open-source community. A quite remarkable change of focus came about when this undertaking shaked off its roots and turned into a cross-platform language, which is nowadays available for Windows, Apple and Linux operating systems. Raspberry OS support was initially experimental, but since some time our installations have been quite stable. As an extension to the Visual Studio Code integrated development environment, PowerShell has become a viable tool for users and administrators with cross-platform needs.

Starting apparently with PowerShell 7.3 PowerShell has integrated some useful functionality which facilitates integration between Mardown, PowerShell and VisualStudio Code.

    # Render Markdown content in Visual Studio Code (or any VT100 compatible console):
    Show-Markdown -Path .\page.md
   
    # Render Markdown content to be displayed the current browser:
    Show-Markdown -Path .\page.md -UseBrowser

Even more useful is the conversion command `ConvertFrom-Markdown` which translates a Markdown page into HTML usable at your WWW site. Here you are:

    # Translate Markdown to HTML which is usable as a WWW page in a HTTP service
    ConvertFrom-Markdown -Path ./page.md | Select-Object -ExpandProperty Html | Set-Content -Path ./page.htm

---

## Contact information

This is how you should be able to reach me: Try pdonner at the cooperative's nettinoste.fi domain. There is a lot of spam among those mails, but I'm reading the messages of that post office once or twice every week. 

<!---
phdonner/phdonner is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
