# my-awesome

Git-based bookmarking tool powered by GitHub actions, integrated with Telegram, built with Hugo and hosted on GitHub pages

* [Demo](https://my-awesome.github.io/my-awesome-template)

> why ???

* Ask HN: [Do you curate links/bookmarks?](https://news.ycombinator.com/item?id=22158218)
* Ask HN: [How do you manage your bookmarks?](https://news.ycombinator.com/item?id=22105561)
* See [Web Archiving Community](https://github.com/ArchiveBox/ArchiveBox/wiki/Web-Archiving-Community) for alternatives

## How it works

> TODO for now you must have your own bot

Rules:
* every multi-line text is evaluated independently
* the order of the content doesn't matter
* a message must contains a valid **url** or it will be ignored i.e. a word that starts with `http`
* if a line contains a word starting with *underscore* it will be used as **path** e.g. `_folder_subfolder`
    - optional, default is root `/`
    - you can defined only 1 path
* if a line contains a word starting with *hash* it will be used as **tag**
    - optional, by default a `telegram` tag is added
    - you can defined multiple tags

## Setup

> TODO

1. "Use this template"
2. create bot
3. save env (show how to retrieve user_id)
4. diagram

## Development

Resources

* [GitHub Actions](https://docs.github.com/en/actions)
* [Starter Workflows](https://github.com/actions/starter-workflows)
* [GitHub CLI](https://cli.github.com/manual)
* [Telegram Bot API](https://core.telegram.org/bots/api#getupdates)
* [Hugo](https://gohugo.io/documentation)
* [20 Minute Hugo](https://www.youtube.com/playlist?list=PLbWvcwWtuDm1OpcbohZTOwwzmc8SMmlBD) (video)
* [Hugo GitHub Action](https://github.com/marketplace/actions/hugo-setup)

Telegram

```bash
# an update is considered confirmed as soon as getUpdates
# is called with an offset higher than the latest update_id
http https://api.telegram.org/bot<TELEGRAM_API_TOKEN>/getUpdates?offset=<TELEGRAM_OFFSET>

# invoke manully (uncomment "source")
.github/scripts/telegram.sh
# requires
cat telegram.secrets 
#DATA_PATH="./data/telegram.json"
#TIMESTAMP=$(date +%Y%m%d-%H%M%S)
#TELEGRAM_API_TOKEN=
#TELEGRAM_FROM_ID=
```

Hugo

```bash
sudo snap install hugo --channel=extended

# generate hugo skeleton
hugo new site . --force

# run locally
# http://localhost:1313
hugo server -D
```
