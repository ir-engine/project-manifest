# project-manifest

To install all official open source projects for local development, use the following scripts inside your iR engine installation.

Install the core contributor test suite
```bash
npm run install-manifest -- --manifestURL="https://github.com/ir-engine/project-manifest/blob/main/ir-core.manifest.json" --branch="dev"
```

Install all plugins
```bash
npm run install-manifest -- --manifestURL="https://github.com/ir-engine/project-manifest/blob/main/ir-plugins.manifest.json" --branch="dev"
```

Install the demo scenes
```bash
npm run install-manifest -- --manifestURL="https://github.com/ir-engine/project-manifest/blob/main/ir-scenes.manifest.json" --branch="dev"
```

Install all the tutorials

*ir-tutorial-pong was removed from the tutorial manifest due to import errors, but should be added back when fixed.*
```bash
npm run install-manifest -- --manifestURL="https://github.com/ir-engine/project-manifest/blob/main/ir-tutorials.manifest.json" --branch="dev"
```

Note: to allow private repos to install correctly:
```bash
git config --global credential.helper cache
git config --global credential.helper 'cache --timeout=100000000'
```
then clone one repo to enter your Username & Personal Access Token, then run the rest of the clone commands


Cloning projects now requires github SSH keys to work to be compliant with github's policy:
```
1.- Open a terminal window
2.- Run the command ssh-keygen -t ed25519 -C "your_email@example.com" and press Enter
3.- When you're prompted to "Enter a file in which to save the key", you can press Enter to accept the default file location ( ~/.ssh ).
4.- At the prompt, "type a secure passphrase" press Enter

All of that should have created your ssh keys, once you have created SSH Keys, copy the contents from the id_rsa.pub and configure github with these keys.

1.- Open a browser window/tab
2.- Go to github.com
3.- Click on photo of your user located top right of the web page.
4.- Click on Settings
5.- Click on SSH and GPG Keys
6.- Click on "New SSH Key"
7.- Add key title and paste id_ed25519.pub contents
```

