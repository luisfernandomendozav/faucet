# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `npm run build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)

### Course 'Solidity & Ethereum in React (NextJs):The complete Guide' below is the progres:
1. Introduction: 100%
2. How to approach errors: 100%
3. Init App: 100%
4. Remove React JS content: 100%
5. Terminology: 100%
6. [AI] What is Blockchain: 100%
7. [AI] Smart Contracts: 100%
8. [AI] Miners, Networks, Wallet: 100%
9. [AI] Ethereum Remix: 100%
10. Important Note - Truffle: 100%
11. Truffle init: 100%
12. Installing Ganache: 100%
    - To migrate the contract first we have to open Ganache to run the local Blockchain
    - Then we have to select the truffle-config.js file when selecting new workspace
    - Then we have to verify that the same port is in the RPC server on ganache, and in the truffle-config.js, in this case is Port: 7545
    - Then we run `truffle migrate`
    - If we open ganache and select transactions we should see a `CONTRACT CREATION` marked in red, if we click that the bytecode of our contract is the TX DATA.
13. First smart contract: 100%
14. [AI] Ints: 100%
    - uint: max value: (2^256) - 1, min value: 0
    - int: max value: (2^255) - 1, min value: -2^255
15. [AI] Int Correction: 100%
16. Migrating Facuet: 100%
    - ABI in build/contracts/Migrations.json - ABI = Application binary Interface.
    - For compiling the smart contracts we run `truffle compile` this will create a new Json file with the name of the contract in build/contracts.
    - Not all the byte code is deployed int he blockchain, we have another property in json file called deployedBytecode that is actually what is deployed on the blockchain.
    - To migrate we have to create another file in the migrations file, in this case since we are trying to depoyed the Faucet contract we will create a specific migration file for this called: `2_faucet_migration.js`.
    - Then we can run `truffle migrate`.
