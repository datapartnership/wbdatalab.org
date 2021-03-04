# [World Bank Data Lab Site](http://wbdatalab.org)

## Editing:
* Navigate to [forestry](forestry.io)
* If you have not been added as a collaborator, initialize the repo using the `master` branch.
* If you are already a collaborator, edit away!

## Running Locally ():
You should only run locally if you want to do template or layout edits. Workshops and Lab Reports should be edited through Forestry.
* [Install Hugo](https://gohugo.io/getting-started/installing/)
* Clone the repository: `git clone git@github.com:datapartnership/wbdatalab_org.git`
* In the directory, run `hugo serve -D -E -F`
* The site will be available at `http://localhost:1313` in your browser

### Deployment and Workflow
The workflow is as follows:
* Make edits on the `master` or feature branches.
* Once a commit is made to `master`, a Github Action builds the site and commits the result to `gh-pages`.
* The site is deployed through Github's environment.  It is available at `wbdatalab.org` per GoDaddy configured A Records and CNAME.


### Folders and Files
***If a folder is not included in the list below, please don't edit there***

* `/content/`
    * All folders here except `/lab-reports/` and `/workshops-and-clinics/` are placeholders, since most pages on the site are custom and don't follow a set pattern.
    * The folders mentioned above are editable in Forestry.
* `/layout/`
    * `/partials/`: contains pieces of content reused throughout the site.
        * `/base/`: Footer / header / navbar used across the site.
        * `/blocks/`:  Section cards for the front page, workshops listing, lab reports listing, directory, etc.
        * `/list-partials/`:  Workshops lists page, other list pages.
        * `/single-pages/`: Single pages (not linked ATM).

    
* `/static/`
    * Contains everything that will be exported to the `/public/` folder;  Includes JS, SCSS and images.
* `config.toml`
    * Contains various pieces of contant reused across the site.  Change it here, it changes everywhere.

