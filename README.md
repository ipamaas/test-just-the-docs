# FabOS Documentation Site Template

https://ipamaas.github.io/test-just-the-docs/

## Usage

To use the template as starting point for your own documentation site, follow these steps:
1. Copy "docs" folder to your repository folder
2. Update ``_config.yml`` file with your title, repository url and footer.
3. Update the ``index.md`` file with your repository urls.
4. Test your site locally following [Development Guide](#development) below.
5. Publish your site on Github Pages following [Release Guide](#release-on-github-pages) below.

## Development

### Preparation
For local development, use VS Code and the "Remote Containers" externsion with Docker:
1. Install VS Code
2. Install Extension "Remote Containers" (Docker Runtime required!)

### Start development container

To develop and test your site inside a container using VS Code, follow these staps:
1. Type "Ctrl-Shift-P" and enter "Show Remote Menu"
2. In the "Remote Menu" select "Open Folder in Container ..." and select the "docs" folder
3. Wait for container created and started for VS Code remote development.
4. Start Jekyll server by ``bundle exec jekyll serve --livereload``
5. Open http://localhost:4000

## Release on Github Pages

To release the site via Github Pages, follow these steps:
1. Open the ``Settings`` tab of your github repository.
2. Go to ``Pages``
3. Enable Github Pages
4. In ``Source`` select your main branch
5. In ``Source`` select the "/docs" folder
6. Save
7. Check the ``Actions`` tab for build and deploy results.
8. Open your site at ``https://<user_or_org_name>.github.io/<repo_name>/``
