# typescript

This-repo-has-N-stars typescript version.

## Environment

| name               | description                                      | value                   |
| ------------------ | ------------------------------------------------ | ----------------------- |
| __GITHUB_TOKEN__   | GitHub Token                                     | Required                |
| __WEBHOOK_SECRET__ | Website Secret                                   | Required                |
| __REPO_URL__       | Repo URL                                         | Required                |
| __PORT__           | Websocket Port                                   | Optional @default: 3000 |
| __ACTING_URL__     | Websocket Acting Url [smee.io](https://smee.io/) | Optional                |

## Settings

create a new webhook in `settings -> Webhooks -> add webhook`
![](./.github/settings-webhooks.jpg)
set `Payload URL` to `<Your Webhook Server URL>`
set `Content type` to `application/json`
set `Secret` to any string
set `Which events would you like to trigger this webhook?` to `Let me select individual events.` then select `Stars`
![](./.github/watch-event.jpg)

## Start

command:

```sh
yarn install --production
yarn start
```

---

docker:

```sh
docker build -d -t This-repo-has-N-stars-typescript .
```

## Developer

```sh
yarn install
```