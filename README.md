## Introduction

Hi. Here at GitHub I'm phdonner, but on most other platforms I use the signature pdonner. My native language is Swedish, but I was born in Tampere, which is a predominantly Finnish city. Therefore most of us had bilingual competence as a gift. That's a good start in learning English, German, French, Spanish, Kiswahili... other languages.

I've been working quite a lot in English speaking communities, but unidiomatic use of English will hopefully still be excused. If you have time to [write to me](https://github.com/phdonner/phdonner/blob/main/README.md#contact-information), you can be confident that politely expressed corrections will be most gratefully received.

---

## The village network cooperative

Right now my primary occupation is development of fiber optic network maintenance systems and tools. I'm doing more or less full-time voluntary work for our rural network cooperative: Kuhmon kyläverkko-osuuskunta (formerly Luoteis-Kuhmon kyläverkko-osuuskunta), which mainly operates in the north-western part of Kuhmo municipality, at the Russian border right on the middle latitude of Finland. 

Currently, the cooperative is preparing a smart rural project. Please study the cooperative's [Smart Rural 27 pages](https://nettinoste.fi/wp/category/smart-rural-27/), in case you would like to have a look at the preparatory work that we have been doing. The pages are a mix of Finnish and English content, but most often with summaries in both directions. [Multilingual methods](https://github.com/phdonner/phdonner/blob/main/README.md#multilingual-markdown) are actually one of the themes of this site.

![Nettinoste banner](https://nettinoste.fi/wp/wp-content/uploads/2014/05/copy-header_1260_240.png)

---

## The information society

Our project is based on the assumption that we are experiencing the first phases of an emerging new mode of production. In the information society, the many aspects of production are dependent on information technology. Rural inhabitants in our environment don't want to be spectators of that process, but active agents. Deep understanding and early adoption of the new tools of production can be an asset in rural, scarcely populated environments.

Market driven production creates a lot of unnecessary expenses. These are often motivated by IT expenses. Think of quickly growing bank fees. Often the concrete production costs are obscured by abstract concepts like digitization or artificial intelligence. At the same time some of the most potential advantages of information society construction - first of all automation - remains unused. The focus here is a reverse one. The project stresses the importance of simple but effective IT tools and bottom-up and peer oriented collaboration as inroads on the way towards the zero margin society.

---

## How can Markdown documents be rendered and published on the World Wide Web?

This is a personal undertaking which contributes to the NOSTERIIHI smart rural development project. I would, of course, also like to collaborate with other developers, who would be willing to contribute in transforming PowerShell automation into a way of empowering rural developers. It could be important to state an example of how bottom-up oriented, open-source voluntary collaboration can be a smart concept which wins over passivating, profit-based top-down work. Welcome to the zero-margined collaborative community.

Here I'll start quite modestly by producing a simple test case, where simple Markdown will become usable as Web pages. The NOSTERIIHI project will gradually evolve into a bilingual tutorial on methods of setting up a low-cost computer environment, which enables rural developers to produce HTML pages for use in the WWW . This task will be achieved without resorting to commercial services, such as Facebook or WhatsApp. Let's see where the project takes us.

---

## The workflow

Planning is a conceptual activity. To be efficient, we could outline of the various workflows which can be followed. The diagram will hopefully guide our work. 

```mermaid
flowchart LR
    id1([Markdown])
    id2(GitHub)
    id3([WWW])
    id4(Git)
    id5(GitHub)
    id6(Visual Studio Code)
    id7(Powershell)
    id8(HTML)
    id1-->id2-->id3;
    id1-->id4-->id5-->id3;
    id1-->id6-->id7-->id8-->id3;
style id1 fill:#f9f;
style id3 fill:#f9f;
```

If you are curious to know how the above diagram was designed, check out my Markdown subtopic on [Mermaid](markdown.md#mermaid-diagrams-a-way-of-visualizing-conceptual-frameworks), which is a free diagram design and rendering tool. 

The next subheadings are a list of some of the topics and immediate tasks that we are facing right now.

---

## Markdown

Although Markdown is easy to learn, it can become a powerful resource in information society construction. Apart from providing ways of organizing the content of individual documents, it is very handy in preparing web pages, writing email, making task lists and so forth. [Learn the 10 basic notations](https://www.markdownguide.org/basic-syntax/) and you will quickly discover quite a number of real life applications.

Have a look at the [GitHub Markdown sample page](https://gist.github.com/rt2zz/e0a1d6ab2682d2c47746950b84c0b6ee) and push the 'Raw' button to see what the source looks like.

To take advantage of some of the more interesting features of Markdown I listed the following subtopics of this theme:

* Comments in Markdown
* Multilingual Markdown
* Emoji fonts in Markdown and on WWW pages
* Mermaid diagrams for Visual Studio Code and GitHub documentation

You can have closer look at these topics by navigating the [Markdown page](markdown.md) of the NOSTERIIHI project.

---

## Git and GitHub

*Git* is the command language for the safe creation and maintenance of documents. It provides a safe and elegant mechanism for _version control_ and hides a way all the stages of updating the documents in an invisible document of the file system. By documenting the various stages of the update history, the user can easily retrieve earlier versions. _Collaboration_ is an other aspect of the development process that Git facilitates. Developers can work concurrently on various aspects of the content without the risk of colliding updates.

*GitHub* is a free resource where developers of open-source code can create and share new content. By paying a modest yearly fee, developers get access to a number of extra features which are not available to the ordinary registered user. There or other similar services with varying focus. 

At GitHub I’m currently trying to discover how Git, GitHub and related open-source tools and services could be beneficial in information society construction. 

---

## WWW pages at GitHub

There is a special section of GitHub, located at pages.github.com which is dedicated to WWW publication. Navigate to the [GitHub pages](https://pages.github.com/) where you can find a tutorial which introduces the ways of constructing a site for your personal use or for your organization. Alternatively the pages can become a forum for your project.

This is an experimental site. So please, don't expect that the content would be static somehow. On the contrary: If the structure and the content develops dynamically, then that could be taken as a sign of active and perhaps even productive work.

---

## Visual Studio Code

Before the appearance of the open-source Linux operating system, Microsoft Windows was by far the most appealing platform for software developers. With a low license fee the entrance threshold was low. With the so called COM-based technologies MS made a leap into easy-going development of automated systems. Dependency on proprietary arrangements is, however, in the long run a stumbling block for any non-profit oriented developer. Therefore, the initiative to place both the Visual Studio IDE and the PowerShell scripting environment into the domain of open-source and cross-platform development were most welcome moves.

---

## Rendering and transforming Markdown into HTML with PowerShell 

PowerShell is a scripting language created by developers at Microsoft, but nowadays maintained by an open-source community. A quite remarkable change of focus came about when this undertaking shook off its roots and turned into a cross-platform language, which is nowadays available for Windows, Apple and Linux operating systems. Raspberry OS support was initially experimental, but since some time our installations have been quite stable. As an extension to the Visual Studio Code integrated development environment, PowerShell has become a viable tool for users and administrators with cross-platform needs.

Starting with version 7.2, PowerShell includes useful functionality which facilitates integration between Mardown, PowerShell and VisualStudio Code. If you have a sample document called page.md in the current location of your terminal, you should execute the following commands:

    # Render Markdown content in Visual Studio Code (or any VT100 compatible console):
    Show-Markdown -Path .\page.md
   
    # Render Markdown content to be displayed the current browser:
    Show-Markdown -Path .\page.md -UseBrowser

Even more useful is the conversion command `ConvertFrom-Markdown` which translates a Markdown page into HTML usable at your WWW site. Here you are:

    # Translate Markdown to HTML which is directly usable as a WWW page in a HTTP service
    ConvertFrom-Markdown -Path ./page.md | Select-Object -ExpandProperty Html | Set-Content -Path ./page.htm

---

## Contact information

This is how you should be able to reach me: Try pdonner at the cooperative's nettinoste.fi domain. There is a lot of spam among those mails, but I'm reading the messages of that post office once or twice every week. 

<!---
phdonner/phdonner is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
