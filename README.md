# deepdrivemd.github.io

This repository hosts the GitHub Pages website https://deepdrivemd.github.io/ with information on DeepDriveMD: Deep-Learning Driven Adaptive Molecular Simulations.

The repository is organized into three branches.
1. `main`: Stores the raw HTML, JS and content for the website
2. `source`: Stores the source code used to generate the website (HTML templates, JS and other Jekyll infrastructure)
3. `develop`: A branch to edit and explore changes to the website

To update the website please follow these instructions:

1. Clone the repository: `git clone https://github.com/DeepDriveMD/deepdrivemd.github.io.git`
2. Checkout the develop branch: `git checkout develop`
3. Make changes to files add & commit & push
4. Once the changes on the develop branch are approved, open a pull request to merge develop into the source branch
5. After merge, checkout the source branch: `git checkout source`
6. Get the latest changes to source: `git pull`
7. Build the website `_site/` directory: `bundle exec jekyll build`
8. Make a temporary copy of the `_site/` directory outside of the repository: `cp -r _site ..`
9. Checkout the main branch: `git checkout main`
10. CAUTION: make sure you are in the repository directory! Update the content: `rm -r * && cp -r ../_site/* .`
11. Add all the changed files, commit and push: `git add . && git commit -m 'deploy' && git push`
12. Clean up copied `_site/` directory: `rm -r ../_site`

To deploy locally and auto-update the page upon any change to the html (useful for development):
```
bundle exec jekyll serve --watch
```
