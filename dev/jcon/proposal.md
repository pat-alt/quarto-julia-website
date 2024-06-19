# Quarto Extensions for the Julia Community

**Abstract**: [Quarto](https://quarto.org/) is an open-source scientific and technical publishing system that was first presented at JuliaCon 2022. We propose new extensions and workflows that we hope will help the community embrace this promising new tool and boost developers' efforts toward effective communication and reproducibility. 

## Description

What if there was a single tool, an engine that can turn your work into all kinds of different output formats? Markdown, PDF, LateX, beamer, HTML, reveal.js, ePub, MS Office, OpenOffice, entire websites, dashboards … all of that starting from the same place: a plain Markdown document blended with chunks of your favorite programming language. That is the prospect that Quarto offers.

### 🤕 Those Damn Edge Cases ...

The problem is that this is a very ambitious prospect. Even though Quarto is being continuously improved by a committed and responsive development team, there will always be edge cases that require customization. Your presentation at work, for example, might have to comply with certain styling rules. Similarly, the journal you are targeting for your next research project almost definitely has very specific editing guidelines that (if you're lucky enough) are specified in a LaTeX template. In both cases, you will need to invest some time into modifying or extending the behavior of Quarto.

### 🚑 Quarto Extensions to the Rescue

Thankfully - and in true open-source spirit - Quarto has come up with a way to ensure that such efforts never go in vain: [extensions](https://quarto.org/docs/extensions/). Producing and sharing extensions is so simple that it feels almost like a by-product of tailoring Quarto to your specific use case. 

> When I first learned about extensions, I had already created a custom template for myself to create reveal.js presentations in the iconic white-blue theme of Delft University of Technology. Releasing that [template](https://github.com/pat-alt/quarto-tudelft) to the public was almost as easy as creating my first Julia package (obligatory hat tip to the folks behind PkgTemplates.jl). 
>
> — Speaker 1
 
A few months later, Speaker 1 heard from at least a few of their colleagues that they had presented pretty HTML slides in white and blue right from their browser. 

### 🔴🟢🟣 Julia-Themed Quarto

[Julia-Themed Quarto](https://www.patalt.org/quarto-julia-website/) presents a number of Quarto extensions that are specific to Julia and will be the topic of this talk. 

1. The [quarto-julia](https://github.com/pat-alt/quarto-julia) extension contributes various basic format templates for Julia-themed HTML content. It ships with standard Julia colors and fonts to provide your next presentation with a beautiful look. 
2. The [quarto-juliacon-proceedings](https://github.com/pat-alt/quarto-juliacon-proceedings) extension is a more ambitious project. This extension adds support for writing JuliaCon Proceedings papers in Quarto. It is based on the existing [JuliaCon Proceedings LaTeX template](https://github.com/JuliaCon/JuliaConSubmission.jl) and can be used to render standard [PDF](https://www.patalt.org/quarto-juliacon-proceedings/template.pdf) while leveraging all of Quarto's functionalities such as executable code chunks. On top of that, it provides a new [HTML](https://www.patalt.org/quarto-juliacon-proceedings/template.html) template that currently inherits the style of [quarto-julia](https://github.com/pat-alt/quarto-julia). This provides new opportunities for JuliaCon Proceedings papers to include animated and interactive content.
3. Finally, the [Julia-Themed Quarto](https://www.patalt.org/quarto-julia-website/) website also includes a section on the marriage of Quarto and Documenter.jl. This has not yet been turned into a fully-fledged extension but we provide guides for common workflows that facilitate this marriage. This topic will be presented by Speaker 2. 

### 🎯 Goals and Limitations

The [quarto-juliacon-proceedings](https://github.com/pat-alt/quarto-juliacon-proceedings) is not yet officially supported and there remain some [issues](https://github.com/pat-alt/quarto-juliacon-proceedings/issues) that need to be addressed to make it fully compatible with the existing LaTeX template. Similarly, there is scope for improvement concerning the experience of using Quarto with Documenter.jl. We hope that through this talk we can stimulate discussion in the community and encourage others to contribute to these efforts. 

## Notes

To cover everything we have set out for this presentation we would ideally need more than <10 minutes and have therefore decided to submit this for a main talk, despite not presenting any pure Julia developments. Nonetheless, we would also be happy to consider another track that reviewers might deem more suitable. 