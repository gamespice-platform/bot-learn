Offline learning for [GameSpice Bot](https://github.com/gamespice-platform/bot). It will read the anonymous episodes that GameSpice Bot's demonstration recorder stored and write plain files that bots load: verified ride routes, navigation hints and tuned bot parameters. It runs outside the game, on a developer machine or a GPU box. Part of the [GameSpice](https://github.com/gamespice-platform) family.

**Status: design only.** Nothing is built yet, so there is no test suite to run and no game vendors it. [docs/design.md](docs/design.md) is the whole content, and there is nothing to install.

## What it is and is not

| It is | It is not |
| --- | --- |
| A set of offline tools that turn recordings into export files. | A runtime addon. A game never depends on it; GameSpice Bot only reads the files it writes. |
| Dependent on GameSpice Bot's file formats (episode JSON, export manifest). | The recorder. The recorder, schema and stores live in [GameSpice Bot Record](https://github.com/gamespice-platform/bot-record) and GameSpice Bot. |
| Free of player data. Exports carry no identifier of any person. | A place to keep player data. |

## Working on it

Read the family `CLAUDE.md` and the [CLAUDE.md](CLAUDE.md) in this repository first.

## Used by

### Zee's Games

Zee's Games is a collection of games I made on GameSpice, for demonstration and for fun. They show what the platform can do, and they run on live servers you can join. Anybody can create games on GameSpice, and everything in the family is its own repository and can be used separately from the games.

No game uses it yet, because there is no code. The bots in [Zee's Games](https://zeesgames.com) run on [GameSpice Bot](https://github.com/gamespice-platform/bot), and this repository describes the offline step that would feed it. It is built with Claude Code, like the rest of the family. The whole collection is at [zeesgames.com](https://zeesgames.com).

## Licence

MIT. Only the TMC back-end web infrastructure is not open source.
