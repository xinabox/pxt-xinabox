# MakeCode for XinaBox

This repo contains the editor hosted at https://makecode.xinabox.cc .

## Local Dev setup

These instructions assume familiarity with dev tools and languages.

* install [Node.js 8+](https://nodejs.org/en/download/)
* (optional) install [Visual Studio Code](https://code.visualstudio.com/)

In a common folder,

* clone https://github.com/Microsoft/pxt to ``pxt`` folder
* clone https://github.com/Microsoft/pxt-common-packages to ``pxt-common-packages`` folder
* clone https://github.com/xinabox/pxt-xinabox to ``pxt-xinabox`` folder
* go to ``pxt`` and run

```
npm install
npm run build
```

* go to ``pxt-common-packages`` and run

```
npm install
npm link ../pxt
```

* go to ``pxt-xinabox`` and run

```
npm install
npm link ../pxt
npm link ../pxt-common-packages
```

## to run the local server

From root github folder,

```
cd pxt-xinabox
pxt serve --cloud
```

## to build and deploy a single package via command line

```
cd libs/core
pxt deploy
```

## License
MIT
