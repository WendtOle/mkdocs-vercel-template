# How it works

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## How make the project deployable to Vercel

* add `requirements.txt` to root folder
    * with entry `mkdocs`
* add `package.json` to root folder 
    * with `"dev": "mkdocs serve"`
    * with `"build": "mkdocs build -d public"`

## How to install it on Mac

* `brew install mkdocs`

## How create a new Project

* `mkdocs new my-project` - create new project
* `cd my-project` - step into project
* `mkdocs serve` - serve project locally

## How navigation and different pages works?

* adding in `mkdocs.yml` an entry `nav`:
```
nav:
   - Home: index.md
   - About: about.md
```
* also works without the entry in mkdocs.yml - but then in the navigation the files appear just with there file name and ending

## Sources:

* <https://www.mkdocs.org> - documentation of mkdocs
* <https://github.com/fu-sen/Vercel-MkDocs> - easy to deploy to vercel mkdocs template
* <https://www.mkdocs.org/#adding-pages> - adding pages
