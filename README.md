# CS-1400 Reference Website
> I created this website as a reference for my students as they complete their programming assignments.

## Features
- Website automatically redeploys with every new commit.
- More pages can be added to the website by creating another page in the _pages directory.
  - Use an existing page as a template.
- Interactive code snippets are embedded html via [repl.it](https://repl.it/~). If you fork or clone this repo, be sure to replace these embeds with your own repl.it embeds. I cannot guarantee my embedded repl.it's will always be there. repl.it accounts are free, as is embedding your own saved replits.
- Automatically syncs with its parent repo (CS-1030/CS-1030.github.io) every Thursday night at 11pm UTC
  - The frequency and exact timing can be adjusted [here](https://github.com/CS-1400/CS-1400.github.io/blob/e3801251b0c36a5188c5e4eec6d3db3e329eef69/.github/workflows/fork-news.yml#L6)
  - The autosync will not delete any additions or edits made to this fork, it will simply produce a pull request for review.
  - The sync can also be run manually. Open the **Actions** tab, click **Fork News**, then click **Run workflow**.

## Future Features
- Maybe... set this repo up as a parent repo for CS 1410's website. Then all changes can go "downhill"

## Attributions
- [just-the-docs](https://github.com/pmarsceill/just-the-docs) theme: [Patrick Marsceill](https://github.com/pmarsceill), GitHub Product Designer

## Copyright
CS-1400 with Ruiz is © 2021 by Bianca Ruiz.

## License
CS-1400 with Ruiz is distributed by an [MIT license]().
