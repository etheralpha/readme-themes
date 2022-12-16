# readme-themes

This repo consists of [themes](https://github.com/etheralpha/readme-themes/) for simple sites built from README.md files.

Steps to use:

1. Add the following to the top of your README.md file, replacing `${theme-name}` and `${site-name}` with the name of the theme you want to use and what the name of your site is.
    ```
    <meta name="viewport" content="width=device-width,initial-scale=1">
    <title>${site-name}</title>
    <link rel="stylesheet" href="https://etheralpha.github.io/readme-themes/${theme-name}.css">
    ```
1. (Optional) To add the Github link to the bottom of the page add the follow at the bottom of your README.md file, replacing `${github-repo}` with the link to your repo.
    ```
    ##

    <a id="github-link" href="${github-repo}" target="_blank">
      <svg height="40" width="40" aria-hidden="true" viewBox="0 0 16 16" version="1.1" width="32" data-view-component="true" class="octicon octicon-mark-github v-align-middle">
          <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
      </svg>
    </a>
    ```
1. Publish the repo through Github Pages, Netlify, or somilar service.
    - Netlify Settings:
      - Build command: `pandoc -f markdown -t html -o index.html README.md`
    - Github Pages Settings: 
      - Built from root
      - No theme added
