# project-manifest

To install all official open source projects for local development, use the following script in the root of your `etherealengine` folder.

```bash
cd packages/projects/projects

git clone https://github.com/EtherealEngine/ee-ar-demos &
git clone https://github.com/EtherealEngine/ee-assets-basic &
git clone https://github.com/EtherealEngine/ee-bot &
git clone https://github.com/EtherealEngine/ee-ethereal-village &
git clone https://github.com/EtherealEngine/ee-development-test-suite &
git clone https://github.com/EtherealEngine/ee-static-build-template &
git clone https://github.com/EtherealEngine/ee-vps-sample &
# the following projects are currently outdated
# git clone https://github.com/EtherealEngine/ee-maps &
# git clone https://github.com/EtherealEngine/ee-template &
# git clone https://github.com/EtherealEngine/ee-inventory &
# git clone https://github.com/EtherealEngine/ee-productivity &
# git clone https://github.com/EtherealEngine/ee-i18n &
# git clone https://github.com/EtherealEngine/ee-digital-beings &
wait
```

Note: commands starting with a # are not currently up to date with the engine - we are working diligently to get these up to date.

Note: to allow private repos to install correctly:
```bash
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=100000000'
```
then clone one repo to enter your Username & Personal Access Token, then run the rest of the clone commands


To do:

- [ ] Add a manifest.json that can be fetched and installed [See more](https://github.com/EtherealEngine/etherealengine/issues/5648)
- [ ] Keep up to date when new projects are added with Github Actions
