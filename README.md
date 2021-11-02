# Developer Blog

## Dev Setup

Install hugo

```shell
brew install hugo
```

Add the following submodules

```shell
git submodule add https://github.com/austinmcconnell/hugo-strata-theme themes/hugo-strata-theme
git submodule add --branch gh-pages https://github.com/austinmcconnell/resume content/resume
```

If you want to send emails, create an account at formspree.io and set the following environment variable in your .env file.

```
export HUGOxPARAMSxCONTACTxFORMSPREE_FORM_ID=REPLACE_WITH_FORM_ID
```

Otherwise, set formspree_form_id in the config.toml to any string value. It just can't be blank.

## Serve the website

Serve the production version like so

```shell
hugo server
```

Serve the development version like so

```shell
hugo server --buildDrafts --buildFuture
```
