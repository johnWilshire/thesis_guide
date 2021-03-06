Very Rough template / Guide to using RMarkdown for writing your thesis\!
================

## Rmarkdown preamble:

    output:
      #word_document
      pdf_document:
        fig_caption: yes
    fontsize: 12pt
    bibliography: bibliography.bib
    linkcolor: blue
    csl: journal-of-ecology.csl

## Bibliography

  - [Rstudio’s guide:
    authoring\_bibliographies\_and\_citations](https://rmarkdown.rstudio.com/authoring_bibliographies_and_citations.html)

My workflow:

0.  Install the Google Scholar browser extension

1.  Open a paper you want to cite, for example [this
    paper](https://besjournals.onlinelibrary.wiley.com/doi/full/10.1111/j.2041-210x.2012.00261.x)

2.  Click on the extensions icon, click the quote symbol, then click
    bibtex

3.  You should then be on a page that looks like this:

<!-- end list -->

    % comments are preceded by a % sign
    @article{nakagawa2013general, % the documents id
      title={A general and simple method for obtaining R2 from generalized linear mixed-effects models},
      author={Nakagawa, Shinichi and Schielzeth, Holger},
      journal={Methods in Ecology and Evolution},
      volume={4},
      number={2},
      pages={133--142},
      year={2013},
      publisher={Wiley Online Library}
    }

4.  Copy this into your `bibliography.bib`

5.  You can then cite it from within your document by writing:
    `[@nakagawa2013general]` (Nakagawa and Schielzeth 2013)

or unquoted `@nakagawa2013general` Nakagawa and Schielzeth (2013)

Cite mulitple authours by typing `[@nakagawa2013general;
nakagawa2013general]`, seperating them with a `;`

## Title page

Title pages can be included from other files, different chapters can be
included in a similar way

    \```{r child = 'title_page.Rmd'}
    \```

## Useful links

  - [combining several .Rmds into one
    document](https://stackoverflow.com/questions/25824795/how-to-combine-two-rmarkdown-rmd-files-into-a-single-output)
  - [Rmarkdown
    guide](http://kbroman.org/knitr_knutshell/pages/Rmarkdown.html)
  - \[Writing your thesis with R Markdown\]
    (<https://rosannavanhespenresearch.wordpress.com/2016/02/03/writing-your-thesis-with-r-markdown-1-getting-started/>)
  - (thesisdown)\[<https://github.com/ismayc/thesisdown>\]

<div id="refs" class="references">

<div id="ref-nakagawa2013general">

Nakagawa, Shinichi, and Holger Schielzeth. 2013. “A General and Simple
Method for Obtaining R2 from Generalized Linear Mixed-Effects Models.”
*Methods in Ecology and Evolution* 4 (2). Wiley Online Library: 133–42.

</div>

</div>
