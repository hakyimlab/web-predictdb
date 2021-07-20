[![Netlify Status](https://api.netlify.com/api/v1/badges/7133b7c3-0703-4aef-a249-2f96ade817ec/deploy-status)](https://app.netlify.com/sites/cocky-mirzakhani-e469d0/deploys)

## Lab notes in Rmarkdown

For this setup to work, you need to have blogdown and hugo installed on your computer. 
- `install.packages('blogdown') `
- `blogdown::install_hugo()`
- Open RStudio by double clicking `lab-notes.Rproj`
- Start a new analysis by adding a `New Post` from the addin option at the top of the `source` panel

<img src=https://github.com/hakyimlab/web-haky-personal-notes/blob/master/static/new-post-addin.png width="400x"> 

- Choose the title, author, tags
- In format select `R Markdown (.Rmd)` option
- git add, commit and push

Netlify is hosting the content  [here](https://lab-notes.hakyimlab.org)
