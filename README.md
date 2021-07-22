# opensourcestories.org

## Setup

1. Install [go](https://golang.org)
1. Install [hugo](https://gohugo.io)
1. Clone this repository
1. Add the theme submodule: `$ git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke`

## Run the server

To run locally:

`$ hugo server`

To run locally with drafts enabled:

`$ hugo server -D`

Navigate to [localhost:1313](http://localhost:1313)

## Generate the site

To generate the HTML, run:

`$ hugo`

The static files will be stored in the `public/` subdirectory.