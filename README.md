# deepdrivemd.github.io

To update the website please follow these instructions.

1. Clone the repository: `git clone https://github.com/DeepDriveMD/deepdrivemd.github.io.git`
2. Checkout the develop branch: `git checkout develop`
3. Make changes to files add & commit & push
4. Once the changes on the develop branch are approved, open a pull request to merge develop into the source branch
5. After merge checkout the source branch: `git checkout source`
6. Build the website `_site/` directory: `bundle exec jekyll serve`
7. Make a temporary copy of the `_site/` directory


To deploy locally and auto-update the page upon any change to the html 
```
bundle exec jekyll serve --watch
```
