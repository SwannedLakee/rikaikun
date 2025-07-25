# rikaikun <!-- omit in toc -->

[![Chrome Web Store](https://img.shields.io/chrome-web-store/v/jipdnfibhldikgcjhfnomkfpcebammhp?style=flat)](https://chrome.google.com/webstore/detail/rikaikun/jipdnfibhldikgcjhfnomkfpcebammhp)
[![Chrome Web Store Users](https://img.shields.io/chrome-web-store/users/jipdnfibhldikgcjhfnomkfpcebammhp?style=flat)](https://chrome.google.com/webstore/detail/rikaikun/jipdnfibhldikgcjhfnomkfpcebammhp)
[![Mergify Status](https://img.shields.io/endpoint.svg?url=https://api.mergify.com/v1/badges/melink14/rikaikun&style=flat)](https://mergify.com)
[![codecov](https://codecov.io/gh/melink14/rikaikun/branch/main/graph/badge.svg?token=4nZ7madoqJ)](https://codecov.io/gh/melink14/rikaikun)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/e342d582357449f38d9255c247e37159)](https://www.codacy.com/gh/melink14/rikaikun/dashboard?utm_source=github.com&utm_medium=referral&utm_content=melink14/rikaikun&utm_campaign=Badge_Grade)
[![semantic-release: conventional](https://img.shields.io/badge/semantic--release-conventional-commits?logo=semantic-release)](https://github.com/semantic-release/semantic-release)
[![Code Style: Prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat)](https://github.com/prettier/prettier)
[![License GPL-3.0](https://img.shields.io/github/license/melink14/rikaikun?style=flat)](https://github.com/melink14/rikaikun/blob/main/LICENSE)
[![Standard Readme Compliant](https://img.shields.io/badge/standard--readme-OK-green.svg?style=flat)](https://github.com/RichardLitt/standard-readme)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg?style=flat)](https://conventionalcommits.org)
[![All Contributors](https://img.shields.io/github/all-contributors/melink14/rikaikun?color=orange)](#contributors)
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](CODE_OF_CONDUCT.md)

rikaikun is a Chrome extension that helps you to read Japanese web pages by showing the reading and English definition of Japanese words when you hover over them.

## Table of Contents <!-- omit in toc -->

- [Background](#background)
  - [Current Goals](#current-goals)
- [Install](#install)
  - [Via the Chrome Web Store](#via-the-chrome-web-store)
  - [Via Microsoft Edge Add-ons](#via-microsoft-edge-add-ons)
  - [As an Unpacked Extension](#as-an-unpacked-extension)
- [Usage](#usage)
  - [Features](#features)
  - [Options](#options)
    - [Keyboard Shortcuts](#keyboard-shortcuts)
- [Maintainers](#maintainers)
- [Credits](#credits)
- [Contributing](#contributing)
  - [Contributors ✨](#contributors-)
- [License](#license)

## Background

rikaikun is a port of [Rikaichan](https://www.polarcloud.com/getrcx/) I started in 2010 when Chrome released its extension API. It was originally hosted on Google Code until Google Code was canceled and everything was migrated to GitHub.

Rikaichan was a Firefox extension that emulated the popup translations of RikaiXUL. It was the best Japanese-to-English inline translation tool in the browser.

I started with the idea that I would create the Chrome equivalent of Rikaichan from scratch using my own ideas. However, after I tried Rikaichan, I realized that it was already quite good, and starting from scratch would be wasting the excellent work of its developers. Instead, I forked Rikaichan and updated the APIs to work with the Chrome extension model.

In 2018, Firefox killed the extension model that Rikaichan was based on, but other similar extensions have since been created and ported to various browsers. Not much was happening with rikaikun during that time but we've started to work on it again!

### Current Goals

- Refactor code base such that it becomes very easy to maintain and contribute to.
- Fix bugs in dictionary output.
- Work on new features like other dictionaries, OCR, and static popup/lookup bar. Feel free to suggest/:thumbsup: more.

## Install

### Via the Chrome Web Store

Visit rikaikun on the [Chrome Web Store](https://chrome.google.com/webstore/detail/rikaikun/jipdnfibhldikgcjhfnomkfpcebammhp) and click 'Add to Chrome'.

### Via Microsoft Edge Add-ons

Visit rikaikun on [Microsoft Edge Add-ons](https://microsoftedge.microsoft.com/addons/detail/rikaikun/ebdggalafggfhdllgohjbpgnmfppdfih) and click 'Get'.

### As an Unpacked Extension

You can also install rikaikun from the source as an unpacked extension:

- Get the [latest release](https://github.com/melink14/rikaikun/releases/latest) from Github:
- Follow [these instructions](https://github.com/web-scrobbler/web-scrobbler/wiki/Install-an-unpacked-extension) from the web-scrobbler Chrome extension. (substituting rikaikun where appropriate)

## Usage

Activate the extension by clicking on the 理 in the top right. When the introductory pop up appears, rikaikun is ready for action.

When rikaikun is active, hovering over Japanese words will trigger a translation pop-up.

See it in action in this [Youtube demo](https://www.youtube.com/watch?v=DFRTt6d0s3c) by [Tariq Sheikh](https://www.youtube.com/channel/UCRAL2bcBZ1Cw-xyPwelpi8A).

### Features

- Read out the Japanese words using Chrome Text To Speech capabilities. (Off by default)
- Change where the popup appears on your screen. (Where your mouse cursor is by default)
- Copy current definitions to they keyboard.
- Add a delay before popup is shown to avoid constant distractions.
- Require a modifier key to be held down in order to see popups.
- Hide definitions to see only the readings of words.

### Options

You can access the options from [the extension page](chrome://extensions/?options=jipdnfibhldikgcjhfnomkfpcebammhp) if you have it installed or by right clicking on the rikaikun icon.

#### Keyboard Shortcuts

<!-- Generated with https://www.tablesgenerator.com/markdown_tables -->

| Key         | Explanation                |
| ----------- | -------------------------- |
| A           | Alternate popup location   |
| Z           | Zoom popup                 |
| Y           | Move popup location down   |
| C           | Copy to clipboard          |
| D           | Hide/show definitions      |
| Shift/Enter | Switch dictionaries        |
| B           | Previous character         |
| M           | Next character             |
| N           | Next word                  |
| J           | Scroll back definitions    |
| K           | Scroll forward definitions |

## Maintainers

[@melink14](https://github.com/melink14)

## Credits

- [Jon Zarate](https://www.polarcloud.com/) for their work on [Rikaichan](https://www.polarcloud.com/getrcx/)
- [Todd Rudick](http://www.rikai.com) for their work on the original [RikaiXUL](http://rikaixul.mozdev.org)
- This extension uses [JMdict/EDICT](http://www.edrdg.org/wiki/index.php/JMdict-EDICT_Dictionary_Project) and [KANJIDIC](http://www.edrdg.org/wiki/index.php/KANJIDIC_Project) dictionary files. These files are the property of the [Electronic Dictionary Research and Development Group](http://www.edrdg.org/), and are used in conformance with the Group's [licence](http://www.edrdg.org/edrdg/licence.html).

## Contributing

Contribute by submitting pull requests, filing bug reports, requesting features and more!

See the [contributing file](CONTRIBUTING.md) for the full details!

Small note: If editing the README, please conform to the [standard-readme](https://github.com/RichardLitt/standard-readme) specification.

### Contributors ✨

Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<table>
  <tbody>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://qui.suis.je/"><img src="https://avatars2.githubusercontent.com/u/1272018?v=4?s=100" width="100px;" alt="Aaron Muir Hamilton"/><br /><sub><b>Aaron Muir Hamilton</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=xorgy" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://eiennohito.blogspot.com/"><img src="https://avatars1.githubusercontent.com/u/1021694?v=4?s=100" width="100px;" alt="Arseny Tolmachev"/><br /><sub><b>Arseny Tolmachev</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=eiennohito" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Baardman82"><img src="https://avatars.githubusercontent.com/u/82510978?v=4?s=100" width="100px;" alt="Baardman82"/><br /><sub><b>Baardman82</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/issues?q=author:Baardman82+label:bug" title="Bug Reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://www.bazz1.com/"><img src="https://avatars0.githubusercontent.com/u/2224787?v=4?s=100" width="100px;" alt="Bazz"/><br /><sub><b>Bazz</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=bazzinotti" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://birtles.wordpress.com/"><img src="https://avatars1.githubusercontent.com/u/1232595?v=4?s=100" width="100px;" alt="Brian Birtles"/><br /><sub><b>Brian Birtles</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=birtles" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://bruno-queiroz.vercel.app/"><img src="https://avatars.githubusercontent.com/u/122624016?v=4?s=100" width="100px;" alt="Bruno Queiroz"/><br /><sub><b>Bruno Queiroz</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=bruno-queiroz" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/bryanjenningz"><img src="https://avatars.githubusercontent.com/u/7637655?v=4?s=100" width="100px;" alt="Bryan Jennings"/><br /><sub><b>Bryan Jennings</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=bryanjenningz" title="Code">💻</a> <a href="https://github.com/melink14/rikaikun/issues?q=author:bryanjenningz+label:enhancement" title="Ideas & Planning">🤔</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ChocoChopin"><img src="https://avatars1.githubusercontent.com/u/53260343?v=4?s=100" width="100px;" alt="ChocoChopin"/><br /><sub><b>ChocoChopin</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/issues?q=author:ChocoChopin+label:bug" title="Bug Reports">🐛</a> <a href="https://github.com/melink14/rikaikun/issues?q=author:ChocoChopin+label:enhancement" title="Ideas & Planning">🤔</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Dalyn-Boyd"><img src="https://avatars.githubusercontent.com/u/77029116?v=4?s=100" width="100px;" alt="Dalyn"/><br /><sub><b>Dalyn</b></sub></a><br /><a href="#a11y-Dalyn-Boyd" title="Accessibility">️️️️♿️</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://www.darrenlester.com/"><img src="https://avatars2.githubusercontent.com/u/19534488?v=4?s=100" width="100px;" alt="Darren Lester"/><br /><sub><b>Darren Lester</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=darren-lester" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://daviesodu.com/"><img src="https://avatars0.githubusercontent.com/u/11047321?v=4?s=100" width="100px;" alt="Davies Odu"/><br /><sub><b>Davies Odu</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=Davodu" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://erekspeed.com"><img src="https://avatars3.githubusercontent.com/u/1176550?v=4?s=100" width="100px;" alt="Erek Speed"/><br /><sub><b>Erek Speed</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=melink14" title="Code">💻</a> <a href="https://github.com/melink14/rikaikun/pulls?q=is%3Apr+reviewed-by%3Amelink14" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/melink14/rikaikun/issues?q=author:melink14+label:bug" title="Bug Reports">🐛</a> <a href="#projectManagement-melink14" title="Project Management">📆</a> <a href="https://github.com/melink14/rikaikun/issues?q=author:melink14+label:enhancement" title="Ideas & Planning">🤔</a> <a href="https://github.com/melink14/rikaikun/commits?author=melink14" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="http://games.greggman.com"><img src="https://avatars.githubusercontent.com/u/234804?v=4?s=100" width="100px;" alt="Greggman"/><br /><sub><b>Greggman</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/issues?q=author:greggman+label:bug" title="Bug Reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/JakeH"><img src="https://avatars1.githubusercontent.com/u/3156017?v=4?s=100" width="100px;" alt="Jake"/><br /><sub><b>Jake</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=JakeH" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Konstantin-Glukhov"><img src="https://avatars.githubusercontent.com/u/24302271?v=4?s=100" width="100px;" alt="Konstantin-Glukhov"/><br /><sub><b>Konstantin-Glukhov</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/issues?q=author:Konstantin-Glukhov+label:enhancement" title="Ideas & Planning">🤔</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/MayamaTakeshi"><img src="https://avatars3.githubusercontent.com/u/5127023?v=4?s=100" width="100px;" alt="MayamaTakeshi"/><br /><sub><b>MayamaTakeshi</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=MayamaTakeshi" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/maawisul"><img src="https://avatars.githubusercontent.com/u/83802443?v=4?s=100" width="100px;" alt="Muhammad Afham Awisul Islah"/><br /><sub><b>Muhammad Afham Awisul Islah</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=maawisul" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/SamDunlap"><img src="https://avatars.githubusercontent.com/u/59478617?v=4?s=100" width="100px;" alt="Samuel Dunlap"/><br /><sub><b>Samuel Dunlap</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=SamDunlap" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Stephie"><img src="https://avatars0.githubusercontent.com/u/325983?v=4?s=100" width="100px;" alt="Stephie"/><br /><sub><b>Stephie</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/pulls?q=is%3Apr+reviewed-by%3AStephie" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/melink14/rikaikun/commits?author=Stephie" title="Code">💻</a> <a href="https://github.com/melink14/rikaikun/commits?author=Stephie" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tobiowo"><img src="https://avatars3.githubusercontent.com/u/1762224?v=4?s=100" width="100px;" alt="Tobi Owoputi"/><br /><sub><b>Tobi Owoputi</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=tobiowo" title="Code">💻</a> <a href="https://github.com/melink14/rikaikun/issues?q=author:tobiowo+label:bug" title="Bug Reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tora-pan"><img src="https://avatars.githubusercontent.com/u/81494248?v=4?s=100" width="100px;" alt="Travis Pandos"/><br /><sub><b>Travis Pandos</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=tora-pan" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/versusvoid"><img src="https://avatars0.githubusercontent.com/u/3686499?v=4?s=100" width="100px;" alt="Versus"/><br /><sub><b>Versus</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=versusvoid" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/vikohone"><img src="https://avatars2.githubusercontent.com/u/963718?v=4?s=100" width="100px;" alt="Ville Kohonen"/><br /><sub><b>Ville Kohonen</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=vikohone" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/Vwing"><img src="https://avatars2.githubusercontent.com/u/9121881?v=4?s=100" width="100px;" alt="Vwing"/><br /><sub><b>Vwing</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=Vwing" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/YaSh8202"><img src="https://avatars.githubusercontent.com/u/91831606?v=4?s=100" width="100px;" alt="Yash Bajaj"/><br /><sub><b>Yash Bajaj</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=YaSh8202" title="Documentation">📖</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/deshaun93"><img src="https://avatars1.githubusercontent.com/u/11935435?v=4?s=100" width="100px;" alt="deshaun93"/><br /><sub><b>deshaun93</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/commits?author=deshaun93" title="Code">💻</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/ollkorrekt"><img src="https://avatars.githubusercontent.com/u/40447847?v=4?s=100" width="100px;" alt="ollkorrekt"/><br /><sub><b>ollkorrekt</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/issues?q=author:ollkorrekt+label:bug" title="Bug Reports">🐛</a></td>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/qkjosh"><img src="https://avatars.githubusercontent.com/u/14936049?v=4?s=100" width="100px;" alt="qkjosh"/><br /><sub><b>qkjosh</b></sub></a><br /><a href="https://github.com/melink14/rikaikun/issues?q=author:qkjosh+label:bug" title="Bug Reports">🐛</a> <a href="https://github.com/melink14/rikaikun/commits?author=qkjosh" title="Code">💻</a></td>
    </tr>
    <tr>
      <td align="center" valign="top" width="14.28%"><a href="https://github.com/sdcr"><img src="https://avatars3.githubusercontent.com/u/1684738?v=4?s=100" width="100px;" alt="sdcr"/><br /><sub><b>sdcr</b></sub></a><br /><a href="https://github.com/sdcr/heisig-kanjis" title="Data">🔣</a></td>
    </tr>
  </tbody>
</table>

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!

## License

[GPL-3.0 © 2020 Erek Speed](LICENSE)
