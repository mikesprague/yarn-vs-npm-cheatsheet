Last Updated: October 23, 2016

# Yarn vs NPM Commands Cheat Sheet

Markdown version of [Medium post](https://shift.infinite.red/npm-vs-yarn-cheat-sheet-8755b092e5cc#.tctsw3s17) by
[Gant Laborde](https://twitter.com/GantLaborde). Many thanks for his work writing the original post.

---

Okay, so you’ve heard about this new JavaScript package manager called [yarn](https://github.com/yarnpkg/yarn),
installed it with `npm i -g yarn`, and now you want to know how to use it? For the most part if you know NPM,
you’re already set! Here are the key notes for switching.

---

## What you need to know

* `npm install` === `yarn` — Install is the default behavior.

* `npm install taco --save` === `yarn add taco` — The Taco package is saved to your package.json immediately.

* `npm uninstall taco --save` === `yarn remove taco` — `—-save` can be defaulted in NPM by `npm config set save true`
but this is non-obvious to most developers. Adding and removing from package.json is default in Yarn.

* `npm install taco --save-dev` === `yarn add taco --dev`

* `npm update --save` === `yarn upgrade` — Great call on upgrade vs update, since that is exactly what it is doing!
Version number moves, upgrade is happening! **_WARNING_** `npm update --save` seems to be [kinda broken in 3.11](https://github.com/npm/npm/issues/13555)

* `npm install taco@latest --save` === `yarn add taco`

* `npm install taco --global` === `yarn global add taco` — As always, use global flag with care.

## What you already know about yarn
The packages are the same as on the NPM registry. Yarn is basically a new installer, where NPM structure and registry is the same.

* `npm init` === `yarn init`

* `npm link` === `yarn link`

* `npm outdated` === `yarn outdated`

* `npm publish` === `yarn publish`

* `npm run` === `yarn run`

* `npm cache clean` === `yarn cache clean`

* `npm login` === `yarn login`

* `npm logout` === `yarn logout`

* `npm test` === `yarn test`

## Things yarn has that NPM doesn’t
I'm skipping the items that they warn against using like [`yarn clean`](https://yarnpkg.com/en/docs/cli/clean)

* `yarn licenses ls` — Allows you to inspect the licenses of your dependencies

* `yarn licenses generate-disclaimer` — Automatically create your license dependency disclaimer

* `yarn why taco` — Identify why 'taco' package is installed, detailing which other packages depend upon it

* :arrow_up: Emojis

* Speed :running::zap:

* Automatic shrinkwrap with the yarn lockfile

* Security-centric design

## Things NPM has that yarn doesn’t

* `npm xmas` === **NO EQUIVALENT**

* `npm visnup` === **NO EQUIVALENT**

## Useful Links

* [:notebook: Official Documentation - https://yarnpkg.com/en/docs/](https://yarnpkg.com/en/docs/)

  * [:fast_forward: Migrating From npm - https://yarnpkg.com/en/docs/migrating-from-npm](https://yarnpkg.com/en/docs/migrating-from-npm)

* [:bird::speech_balloon: Yarn on Twitter - https://twitter.com/yarnpkg](https://twitter.com/yarnpkg)

* [:octocat: Yarn on GitHub - https://github.com/yarnpkg/yarn](https://github.com/yarnpkg/yarn)

## Printable (PDF) Version

[![Yarn vs NPM PDF Cheat Sheet Preview](https://github.com/mikesprague/yarn-vs-npm-cheatsheet/blob/master/assets/yarn-vs-npm-pdf-cheatsheet-preview.png?raw=true "Yarn vs NPM PDF Cheat Sheet Preview (Click to Download)")](https://github.com/mikesprague/yarn-vs-npm-cheatsheet/blob/master/assets/yarn-vs-npm-cheatsheet.pdf?raw=true)

[Download PDF](https://github.com/mikesprague/yarn-vs-npm-cheatsheet/blob/master/assets/yarn-vs-npm-cheatsheet.pdf?raw=true)
