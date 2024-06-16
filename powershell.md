# NOSTERIIHI PowerShell

<!-- This is a placeholder for PowerShell content on this site -->

Here I will present details on PowerShell Markdown functionality, including sections on:

* Basic PowerShell Markdown commands
* Fine-tune how markdown is rendered on a VT100 console
* Convert Markdown to PDF
* Extend Markdown with PowerShell table functionality
* Assemble code fragments to a full HTML document
* Define Web page style with CSS and PowerShell 

## Conversion from Markdown to HTML

Starting with version 7.2, PowerShell includes useful functionality which facilitates integration between Mardown, PowerShell and VisualStudio Code. If you have a sample document called page.md in the current location of your terminal, you should be able to execute the following commands:

    # Render Markdown content in Visual Studio Code (or any VT100 compatible console):
    Show-Markdown -Path .\page.md
   
    # Render Markdown content to be displayed with the default browser:
    Show-Markdown -Path .\page.md -UseBrowser

Even more useful is the conversion command `ConvertFrom-Markdown` which translates a Markdown page into HTML usable at your WWW site. Here you are:

    # Translate Markdown to HTML which is directly usable as a WWW page in a HTTP service
    ConvertFrom-Markdown -Path ./page.md | Select-Object -ExpandProperty Html | Set-Content -Path ./page.htm

