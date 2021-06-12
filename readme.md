# How to Create a Customized Template for R Markdown

This is a r package named `rdrafts` created for customizing rmarkdown templates. 

## Steps by Step Guide

1. Create an R package (`new Project -> R Package`), then create new folders, `inst/rmarkdown/templates/`, following the same structure as described in  [17.1 Template structure](https://bookdown.org/yihui/rmarkdown/template-structure.html)

* Each template should have its own folder. 

2. Add the template meta information in `inst/rmarkdown/templates/blog_article/template.yaml`

```r
name: Customized Blog Article
description: A template for Blog Post
```

3. Add the Rmd skeleton in `inst/rmarkdown/templates/blog_article/skeleton/skeleton.Rmd`. This should be your template. 


4. Optional: you can add custom pandoc template in `inst/rmarkdown/templates/templateName/resources/template.tex` if needed. 

5. Then install the R package via `Build - > Install and Restart`. Or devtools::install("rdraft").  

6. Your template can be found under the "Create from template". 

Examples of package and template structure: 

* `draft` package created by [duckmayr](https://github.com/duckmayr/draft)
* `rmarkdown` package created by [yihui](https://github.com/rstudio/rmarkdown/tree/master/inst/rmarkdown/templates/html_vignette)


