# [myawesome.dev](https://myawesome.dev)

[![my-awesome-telegram](https://github.com/niqdev/my-awesome/actions/workflows/my-awesome-telegram.yml/badge.svg)](https://github.com/niqdev/my-awesome/actions/workflows/my-awesome-telegram.yml)

Git-based bookmarking tool powered by GitHub actions, integrated with Telegram, built with Hugo and hosted on GitHub pages

## Development

* [Hugo](https://gohugo.io/documentation)
* [Flexbox Grid](http://flexboxgrid.com)
* Theme inspired by [Archie](https://github.com/athul/archie) and [Cactus](https://github.com/monkeyWzr/hugo-theme-cactus)

```bash
# run locally
# http://localhost:1313
hugo server -D
```

***TODO***

* pagination issue: https://discourse.gohugo.io/t/data-files-and-pagination/2334/5
* add button at the bottom "scroll to the top"
* set auto tag archive if starts with `https://web.archive.org`
* `my-awesome/actions/telegram-action`: update description
    - remove prefix `GitHub - ` from repository
    - remove suffix `· GitHub` from a gist
    - remove suffix `.` (final dot)
    - follow redirects, i.e. avoid `301 Moved Permanently`
* order TAGS by auto and name in `telegram.json`

<!--

https://blog.bitsrc.io/13-css-ui-grid-systems-and-libraries-for-2018-5918104cb591
https://github.com/spech66/hugo-best-practices
https://github.com/rwxrob/hugo-tutorial-link-data-to-type
https://www.jakewiesler.com/blog/hugo-taxonomies
https://www.kiroule.com/article/add-series-taxonomy-to-hugo-theme

https://github.com/gohugoio/hugo/issues/140
https://cyrillschumacher.com/2014/12/21/data-driven-content-with-gohugo.io
https://github.com/kidsil/hugo-data-to-pages

-->
