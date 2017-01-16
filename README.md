[![Build Status](https://travis.ibm.com/Bluemix/bluemix-components-react.svg?token=rxygQXh19ShfmuUT1G3v&branch=master)](https://travis.ibm.com/Bluemix/bluemix-components-react)
[![Coverage Status](https://pages.github.ibm.com/Bluemix/bluemix-components-react/coverage/badge.svg)](https://pages.github.ibm.com/Bluemix/bluemix-components-react/coverage/lcov-report/index.html)

# Bluemix Components React

**React component library for building websites and UIs for Atlas/Bluemix.**

This repository provides a collection of [Bluemix Components](https://github.ibm.com/Bluemix/bluemix-components) implemented using [React](https://facebook.github.io/react/). All of the components align with the latest UI given by [Bluemix Design System](http://design-system.stage1.mybluemix.net/).

## Usage

### List of Available Components

View available React Components [here](https://pages.github.ibm.com/Bluemix/bluemix-components-react/storybook). Usage information is available when you click the blue **?** icon in the top right corner of the selected component.

### Getting Started

Bluemix Components React is published on a private npm registry maintained by the Bluemix Ops Console team.

1. You'll need to create a `.npmrc` file and authenticate to the Whitewater `npm` registry using [these instructions](https://github.ibm.com/Whitewater/npm-enterprise) Add the following to your `.npmrc` file in your project folder in order to access the Console registry:

  ```
  //dev-console-npm.stage1.ng.bluemix.net/:_authToken="u6vjQywpRv51/eKBiRcAFA=="
  @console:registry=https://dev-console-npm.stage1.ng.bluemix.net/
  ```

2. If you haven't done so already, create a `package.json` for your project:

  ```
  $ npm init
  ```

3. Install `bluemix-components-react` via npm:

  ```
  $ npm install --save @console/bluemix-components-react
  ```

4. These components require the use of [Webpack](http://webpack.github.io/docs/tutorials/getting-started/) in your project. See our [`webpack.config.js`](/.storybook/webpack.config.js) for an example configuration.

5. Example usage:

  ```
  import { Loading } from '@console/bluemix-components-react';
  ReactDOM.render(
    <Loading className="example-loading" />,
    document.getElementById('example-container')
  );
  ```

## Development

Please refer to the [Contribution Guidelines](CONTRIBUTING.md) before starting any work.

### Using the server

We recommend the use of [React Storybook](https://github.com/storybooks/react-storybook) for developing components.

1. Start the server:

	```
	$ npm run storybook
	```

2. Open browser to `http://localhost:9001/`.

3. Develop components in their respective folders (`/components` or `/internal`).

4. Write stories for your components in `/.storybook`.

## a11y testing

This project is scanned according to [IBM a11y standards](https://w3-connections.ibm.com/wikis/home?lang=en-us#!/wiki/Wa7b684534a33_4971_b961_4529f9ad4a2e/page/CI%20162%20compliance%20information) when PRs are opened against it using [`@ibma/aat`](https://github.ibm.com/IBMa/Tools-Auto-Node/blob/master/src/README.md) to scan the components in the form of rendered HTML.  

These tests can also be ran locally at any time by running:

  ```
  $ npm run test-a11y
  ```

Pull requests that introduce more a11y violations than are currently present will not pass code review.

## Contributing

Please check out our [Contribution Guidelines](CONTRIBUTING.md) for detailed information on how you can lend a hand.

## Examples

Here is a list of projects found that use `bluemix-components-react`:

- [IBM Design](https://github.ibm.com/Design/ibm-design-dependencies)
- [Armada](https://github.ibm.com/alchemy-containers/armada-ui)
- [MLASS](https://github.ibm.com/db2z-ml/mlaas)
- [MLASS Dashboard](https://github.ibm.com/NGP-TWC/mlaas-dashboard)
- [API Connect Native Dashboard](https://github.ibm.com/apimesh/native-dashboard)
- [Atlas Access Management](https://github.ibm.com/IAM/access-management)
- [Hybrid Connect Client](https://github.ibm.com/C2C-HybridConnect/HCClient)
- [Bluemix Starter](https://github.ibm.com/Bluemix/generator-bluemix-ui-app)
- [Bluemix UnifiedSupport](https://github.ibm.com/gordonj/Bluemix.UnifiedSupport)
- [Radio Dashboard](https://github.ibm.com/chrisdhanaraj/radio-dashboard)
