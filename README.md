# project-manifest

To install all official open source projects for local development, use the following script inside your ethereal engine installation.

npm run install-manifest -- --manifestURL="https://raw.githubusercontent.com/EtherealEngine/project-manifest/main/manifest.json" --branch="dev"

Note: to allow private repos to install correctly:
```bash
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=100000000'
```
then clone one repo to enter your Username & Personal Access Token, then run the rest of the clone commands


To do:

- [x] Add a manifest.json that can be fetched and installed [See more](https://github.com/EtherealEngine/etherealengine/issues/5648)
- [ ] Keep up to date when new projects are added with Github Actions


