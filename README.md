# SatisMeter React Native (react-native-satismeter)


<p align="center">
<!-- START social-badges -->
<a href="https://github.com/React-Native-Nation/react-native-satismeter/watchers"><img src="https://img.shields.io/github/watchers/React-Native-Nation/react-native-satismeter.svg?style=social" alt="Watch on GitHub" /></a>
<a href="https://github.com/React-Native-Nation/react-native-satismeter/stargazers"><img src="https://img.shields.io/github/stars/React-Native-Nation/react-native-satismeter.svg?style=social" alt="Star on GitHub" /></a>
<a href="https://twitter.com/intent/tweet?text=Satismeter React Native Support! https://github.com/React-Native-Nation/react-native-satismeter"><img src="https://img.shields.io/twitter/url/https/github.com/React-Native-Nation/react-native-satismeter.svg?style=social" alt="Tweet!" /></a>
<!-- END social-badges -->
</p>

<p align="center">
<!-- START description -->
From ReactNativeNation.com Community
<!-- END description -->
</p>

<p align="center">
<!-- START status-badges -->
<a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="PRs Welcome" /></a>
<a href="#contributors"><img src="https://img.shields.io/badge/all_contributors-7-blue.svg?style=flat-square" alt="All Contributors" /></a>
<a href="https://travis-ci.org/React-Native-Nation/react-native-satismeter"><img src="https://img.shields.io/travis/React-Native-Nation/react-native-satismeter.svg?style=flat-square" alt="Build Status" /></a>
<a href="https://codecov.io/github/React-Native-Nation/react-native-satismeter"><img src="https://img.shields.io/codecov/c/github/React-Native-Nation/react-native-satismeter.svg?style=flat-square" alt="Code Coverage" /></a>
<a href="https://greenkeeper.io"><img src="https://badges.greenkeeper.io/React-Native-Nation/react-native-satismeter.svg?style=flat-square" alt="Greenkeeper" /></a>
<!-- END status-badges -->
</p>

<p align="center">
<!-- START npm-badges -->
<a href="https://npmjs.com/package/react-native-satismeter"><img src="https://img.shields.io/npm/v/react-native-satismeter.svg?label=react-native-satismeter&style=flat-square" alt="react-native-satismeter"></a>
<!-- END npm-badges -->
</p>


SatisMeter is mobile and web platform for collecting customer feedback, based on Net Promoter Score. 

This package contains a survey widget that can be easily integrated into any **React Native** application.

## Installation,  It's Mostly automatic installation

`$ yarn add react-native-satismeter`

## Usage

### Registration

First of all you should create your account in https://satismeter.com

### Identify user

Add the following code to your RN application.


```javascript
import Satismeter from 'react-native-satismeter';

Satismeter.hook('<USER_ID>', '<WRITE_KEY>', {}, (message) => {
    this.setState({
    status: 'Hi Satismeter',
    });
});
```

Replace the `WRITE_KEY` with the one found in SatisMeter settings / Integrations / API Keys.

Replace `USER_ID` with the ones of the currently logged-in user.

#### Add custom traits

Pass an object containing string values to set custom user traits.

```javascript
import Satismeter from 'react-native-satismeter';

Satismeter.hook('<USER_ID>', '<WRITE_KEY>', {
  "name": "Sam Harris",
  "twitter": "@SamHarrisOrg"
}, (message) => {
    this.setState({
    status: 'Hi Satismeter',
    });
});
```


## Contributors

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table>
  <tr>
    <td align="center"><a href="https://jamesjara.me"><img src="https://avatars2.githubusercontent.com/u/780219?v=4" width="100px;" alt="James Jara"/><br /><sub><b>James Jara</b></sub></a><br /><a href="#infra-jamesjara" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/React-Native-Nation/react-native-satismeter/commits?author=jamesjara" title="Code">💻</a> <a href="https://github.com/React-Native-Nation/react-native-satismeter/commits?author=jamesjara" title="Tests">⚠️</a> <a href="https://github.com/React-Native-Nation/react-native-satismeter/commits?author=jamesjara" title="Documentation">📖</a></td>
  </tr>
</table>

## Contributing

<!-- START contributing -->

If you have any question, suggestion or recommendation, please [open an issue](issues/new) about it.

If you decided you want to introduce something to the project, please read [contribution guidelines](./docs/contributing.md) first.


## License

react-native-satismeter is available under the MIT license. See the LICENSE file for more info.
