# Full Restore

A FOSS web app designed for processing and archiving Pokémon Showdown tournaments and replays, along with any associated video content.

## Prerequisites
- Node.js version 23 or higher
- PostgreSQL 16
- Docker Engine (Linux, recommended), or Docker Deskop (any OS)

## Repo structure overview

```
|-super-potion (web client)
|
|-fullrestore-server
| \
| |-api
| |-migration
| |-service
|   \
|   |-@fullrestore/service
|   
|-fullrestore-database
| \
| |-container
|
|-fullrestore-importer
|
|-fullrestore-assistant
```
## Local Setup Instructions

1. Clone [super-potion](https://github.com/full-restore/super-potion) and [fullrestore-server}(https://github.com/full-restore/fullrestore-server) somewhere accessible (optionally [fullrestore-importer](https://github.com/full-restore/fullrestore-importer), and [fullrestore-assistant](https://github.com/full-restore/fullrestore-assistant))
2. Run `docker pull --platform linux/amd64 ghcr.io/full-restore/fullrestore-database:main` to fetch a database instance, and run it
3. populate `.env` files in super-potion as well as fullrestore/packages/api, both have example files

Ask for help on any of this, the current setup is somewhat fragile, and this documentation will be expanded in due time.

## Contributing
Fork whichever repo you're working on and open a pull request, and I'll take a look. Detailed guidance will come shortly.

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
