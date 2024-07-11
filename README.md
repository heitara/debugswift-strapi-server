# NodeJS based backend

This project is a basic Strapi v. 4.25.3 setup.
The codebase in TS. The configured DB is sqlite.

This configuration is to locally simulate multipart requests.

## How to check if everything works as expected?

1. Be sure that you have node v 18 or newer.
1. Run `npm i` to install all dependencies in the root folder.
1. Rund `npm run develop` to start the local server. The default config is going to start a server on the following address: `localhost:1337`.
1. Run the following command to check if the upload works fine.
If you want to create an article with an associated asset.
```bash
curl --location 'http://localhost:1337/api/articles' \
--form 'data="{\"title\":\"Sample article\", \"body\":\"plain text\"}"' \
--form 'files.assets=@"/FULL.PATH.TO.JPG"'
```
If you want to upload a media.
```bash
curl --location 'http://localhost:1337/api/upload' \
--form 'files=@"/FULL.PATH.TO.JPG"' \
```

To open the admin use the following credentials: `heitara  [at] gmail.com`.
With the following Password007.


## 🚀 Getting started with Strapi

Strapi comes with a full featured [Command Line Interface](https://docs.strapi.io/dev-docs/cli) (CLI) which lets you scaffold and manage your project in seconds.

### `develop`

Start your Strapi application with autoReload enabled. [Learn more](https://docs.strapi.io/dev-docs/cli#strapi-develop)

```
npm run develop
# or
yarn develop
```

### `start`

Start your Strapi application with autoReload disabled. [Learn more](https://docs.strapi.io/dev-docs/cli#strapi-start)

```
npm run start
# or
yarn start
```

### `build`

Build your admin panel. [Learn more](https://docs.strapi.io/dev-docs/cli#strapi-build)

```
npm run build
# or
yarn build
```

## ⚙️ Deployment

Strapi gives you many possible deployment options for your project including [Strapi Cloud](https://cloud.strapi.io). Browse the [deployment section of the documentation](https://docs.strapi.io/dev-docs/deployment) to find the best solution for your use case.

```
yarn strapi deploy
```

## 📚 Learn more

- [Resource center](https://strapi.io/resource-center) - Strapi resource center.
- [Strapi documentation](https://docs.strapi.io) - Official Strapi documentation.
- [Strapi tutorials](https://strapi.io/tutorials) - List of tutorials made by the core team and the community.
- [Strapi blog](https://strapi.io/blog) - Official Strapi blog containing articles made by the Strapi team and the community.
- [Changelog](https://strapi.io/changelog) - Find out about the Strapi product updates, new features and general improvements.

Feel free to check out the [Strapi GitHub repository](https://github.com/strapi/strapi). Your feedback and contributions are welcome!

## ✨ Community

- [Discord](https://discord.strapi.io) - Come chat with the Strapi community including the core team.
- [Forum](https://forum.strapi.io/) - Place to discuss, ask questions and find answers, show your Strapi project and get feedback or just talk with other Community members.
- [Awesome Strapi](https://github.com/strapi/awesome-strapi) - A curated list of awesome things related to Strapi.

---

<sub>🤫 Psst! [Strapi is hiring](https://strapi.io/careers).</sub>
