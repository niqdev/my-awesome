# my-awesome

Git-based bookmarking tool powered by GitHub actions, integrated with Telegram, built with Hugo and hosted on GitHub pages

## Development

* [Hugo](https://gohugo.io/documentation)
* [Flexbox Grid](http://flexboxgrid.com)
* Theme inspired by [Archie](https://github.com/athul/archie) and [Cactus](https://github.com/monkeyWzr/hugo-theme-cactus)

```bash
# run locally
hugo server -D

http://localhost:1313
```

<!--

TODO:
* sanitize tags [a-zA-Z0-0_-/]
* path vs tag
* tag: name/type:auto/custom/path-folder ???
* exclude `source:telegram` tag
* add tag count in `/tags` page
* add pagination in `/tag` page
* in homepage group and list by `path` (folder): show only the first N (configurable) without pagination ordered by timestamp
* add `/path` page: list all items in that page with pagination

https://blog.bitsrc.io/13-css-ui-grid-systems-and-libraries-for-2018-5918104cb591
https://github.com/spech66/hugo-best-practices
https://github.com/rwxrob/hugo-tutorial-link-data-to-type
https://www.jakewiesler.com/blog/hugo-taxonomies
https://www.kiroule.com/article/add-series-taxonomy-to-hugo-theme

https://github.com/gohugoio/hugo/issues/140
https://cyrillschumacher.com/2014/12/21/data-driven-content-with-gohugo.io
https://github.com/kidsil/hugo-data-to-pages

https://stackoverflow.com/questions/5014632/how-can-i-parse-a-yaml-file-from-a-linux-shell-script

---

# offline

hugo v0.84.0+extended linux/amd64 BuildDate=2021-06-18T22:58:08Z
ERROR 2021/06/22 09:09:01 Failed to get JSON resource "https://api.twitter.com/1/statuses/oembed.json?id=877500564405444608&dnt=false": Get "https://api.twitter.com/1/statuses/oembed.json?id=877500564405444608&dnt=false": dial tcp: lookup api.twitter.com: Temporary failure in name resolution
If you feel that this should not be logged as an ERROR, you can ignore it by adding this to your site config:
ignoreErrors = ["error-remote-getjson"]
Built in 75 ms
Error: Error building site: logged 1 error(s)

-->
