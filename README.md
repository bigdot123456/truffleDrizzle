## setup
This project comes with everything you need to start using smart contracts from a react app with Drizzle. It includes drizzle, drizzle-react and drizzle-react-components to give you a complete overview of Drizzle's capabilities.

## Installation
First ensure you are in a new and empty directory.

Run the unbox command via npx and skip to step 3. This will install all necessary dependencies. A Create-React-App is generated in the app directory.

npx truffle unbox drizzle
Alternatively, you can install Truffle globally and run the unbox command.
```
npm install -g truffle
truffle unbox drizzle
```
Run the development console.
```
truffle develop
```
Compile and migrate the smart contracts. Note inside the development console we don't preface commands with truffle.
```
compile
migrate
```
In the app directory, we run the React app. Smart contract changes must be manually recompiled and migrated.

// in another terminal (i.e. not in the truffle develop prompt)
cd app
npm run start
Truffle can run tests written in Solidity or JavaScript against your smart contracts. Note the command varies slightly if you're in or outside of the development console.

// inside the development console
test

// outside the development console
truffle test
Jest is included for testing React components. Compile your contracts before running Jest, or you may receive some file not found errors.

// ensure you are inside the app directory when running this
npm run test
To build the application for production, use the build script. A production build will be in the app/build folder.

// ensure you are inside the app directory when running this
npm run build
FAQ
Where do I find more information about Drizzle?

Check out our documentation or any of the three repositories (drizzle, drizzle-react, drizzle-react-components).

Where is my production build?

The production build will be in the app/build folder after running npm run build in the app folder.

Where can I find more documentation?

This box is a marriage of Truffle and a React setup created with create-react-app. Either one would be a great place to start!
