# project-manifest

To install all official open source projects for local development, use the following scripts inside your ethereal engine installation.

Install the demo scenes
```bash
npm run install-manifest -- --manifestURL="https://github.com/EtherealEngine/project-manifest/blob/main/ee-scenes.manifest.json" --branch="main"
```

Install all the tutorials
```bash
npm run install-manifest -- --manifestURL="https://github.com/EtherealEngine/project-manifest/blob/main/ee-tutorials.manifest.json" --branch="main"
```

Install all plugins
```bash
npm run install-manifest -- --manifestURL="https://github.com/EtherealEngine/project-manifest/blob/main/ee-plugins.manifest.json" --branch="main"
```

Install the core contributor test suite
```bash
npm run install-manifest -- --manifestURL="https://github.com/EtherealEngine/project-manifest/blob/main/ee-core.manifest.json" --branch="main"
```

Note: to allow private repos to install correctly:
```bash
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=100000000'
```
then clone one repo to enter your Username & Personal Access Token, then run the rest of the clone commands


To do:

- [x] Add a manifest.json that can be fetched and installed [See more](https://github.com/EtherealEngine/etherealengine/issues/5648)
- [ ] Keep up to date when new projects are added with Github Actions


