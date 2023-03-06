# project-manifest

To install all official open source projects for local development, use the following script in the root of your `etherealengine` folder.

Note: commands starting with a # are not currently up to date with the engine - we are working diligently to get these up to date.

```bash
cd packages/projects/projects

git clone https://github.com/EtherealEngine/ee-bot
git clone https://github.com/EtherealEngine/ee-development-test-suite
git clone https://github.com/EtherealEngine/ee-vps-sample
# git clone https://github.com/EtherealEngine/ee-maps
# git clone https://github.com/EtherealEngine/ee-inventory
# git clone https://github.com/EtherealEngine/ee-i18n
# git clone https://github.com/EtherealEngine/ee-digital-beings
```

To do:

- [ ] Add a manifest.json that can be fetched and installed,
- [ ] Keep up to date when new projects are added with Github Actions
