# Setup mkdocs with github pages

- [Setup mkdocs with github pages](#setup-mkdocs-with-github-pages)
  - [Instruction](#instruction)
  - [Requirements](#requirements)

## Instruction

This webpages are static generated markdown documents that are generated from my github repository.
A push or merge to the master branch triggers a github action that starts the [mkdocs](https://www.mkdocs.org/) static site generator, witch builds this whole website and puts the static html documents inside an own branch. I use the github webpage hosting service and my own domain to serve the html documents to the internet. 

The benifits of this approach are:

* free webhosting if you already have a github pro account
* Using git and markdown workflow to write/edit and deploy your content
* No maintenance for a CMS like wordpress, no security updates, no bugs
* Third part contribution with pull requests

  
## Requirements


* Github Pro
* Domain