# NOSTERIIHI PowerShell

<!-- This is a placeholder for PowerShell content on this site -->

Here I will present details on PowerShell Markdown functionality, including sections on:

* Assemble code fragments to a full HTML document
* Define Web page style with CSS and PowerShell 
* Extend Markdown with PowerShell table functionality
* Convert Markdown to PDF
* Fine-tune how markdown is rendered on a VT100 console

---

## Display Markdown in your default browser

Starting with version 7.2, PowerShell includes useful functionality which facilitates integration between Mardown, PowerShell and VisualStudio Code. If you have a sample document called page.md in the current location of your local terminal, you should be able to view your Markdown file in a WWW browser. Execute a single command, Show-Markdown with the -UseBrowser argument:

    # Render Markdown content to be displayed with the default browser:
    Show-Markdown -Path .\page.md -UseBrowser

---

## Conversion from Markdown to HTML

Most useful is the PowerShell conversion command `ConvertFrom-Markdown` which translates a Markdown page into HTML usable at your WWW site. 

Here you are:

    # Translate Markdown to HTML which is directly usable as a WWW page in a HTTP service
    ConvertFrom-Markdown -Path ./page.md | Select-Object -ExpandProperty Html | Set-Content -Path ./page.htm

---

## Conversion from Markdown to a VT100 encoded string

This variation is useful in a configuration equipped with a VT100 console. This is the case if development work is e.g. carried out on the Visual Studio Code IDE.

    # Render Markdown content in Visual Studio Code (or any VT100 compatible console):
    Show-Markdown -Path .\page.md
   
The conversion can be fine-tuned with a related PowerShell command Set-MarkdownOption which sets the color and style used for rendering Markdown text:

    Set-MarkdownOption

The command also supports two themes, that is two predefined color sets called  `Dark` and `Light`. Like this:

    Set-MarkdownOption -Theme Dark
  
The PowerShell documentation states the obvious fact, that "If the terminal doesn't support ANSI color escape sequences (VT100), then colors are not displayed."

<!-- Check out https://github.com/read-0nly/PSRepo/tree/master/colorDemo -->
