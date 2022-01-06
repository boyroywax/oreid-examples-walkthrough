# Aikon Tutorial Walkthrough

Tutorial Used for this Walktrhough: [*https://help.aikon.com/developers/oreid-getting-started-guide*](https://help.aikon.com/developers/oreid-getting-started-guide)

[TOC]

## Test System

1. MacBook Pro (32GB Ram, Intel Proc)
2. OSX Version 11.6 (20G165)

## Pre-requisites

### Assumed knowledge

* Basic command line usage.
* Basic git (Git Hub) knowledge.

### Install Node & npm

1. Download the latest LTS installer for your system.

    <img src="imgs/Screen Shot 2022-01-05 at 6.03.30 PM.png" alt="Screen Shot 2022-01-05 at 6.03.30 PM" style="zoom:35%;" />

2. Check the installed version using the terminal.

```shell
node --version
```

3. Find the location of the node version being used.

```shell
which node
```

4. Look up more information about the particular npm version.

```shell
npm config ls -l
```

5. A Node version manager can be used on Mac OS X.  (And other operating systems.)

```shell
brew install nvm
nvm current
nvm install --lts
```

Additional Resource: [*Downloading and installing Node.js and npm*](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) 

## Running the Sample App

### Online Sample App

View the online example - [https://react-example.oreid.io](https://react-example.oreid.io/)

### How to Run the Sample App - [Step 1: Login](https://github.com/TeamAikon/ore-id-docs/tree/master/examples/react/tutorial/step1-login)

Sample app is an example created by Create React App.

1. Clone the sample app repository.

```shell
git clone https://github.com/TeamAikon/ore-id-docs.git
```

2. Change directory to the React Sample App #1 - Login.

```shell
cd ore-id-docs/examples/react/tutorial/step1-login
```

3. Install the dependencies.

```shell
npm i
```

4. Run the bootstrapped react app.

```shell
yarn start
```

5. Allow node to open your browser to http://localhost:3000
6. Test logining in using FaceBook :white_check_mark: and Google :white_check_mark:

> :red_circle: ISSUE: Login with IdToken is not clickable.

<img src="imgs/Screen Shot 2022-01-06 at 9.26.29 AM.png" alt="Screen Shot 2022-01-06 at 9.26.29 AM"  />

7. When logging in to the sample app for the first time, the system asks you to create a 4 digit PIN number.

> :red_circle: ISSUE: PIN is pre-filled with password and is hard to erase.
>
> :red_circle: ISSUE: Logout of account does not clear cookies.  Can only login using the same Google/FaceBook account.  No choice to select account after already signed in and logged out.

### Signing Transactions with the sample app - [Step 2: Sign](https://github.com/TeamAikon/ore-id-docs/tree/master/examples/react/tutorial/step2-sign)

1. Navigate to the step2-sign folder.

```shell
cd ../step2-sign
```

2. Install the dependencies.

```shell
npm i
```

3. Run the second sample app

```shell
yarn start
```

4. Let node open your browser to http://localhost:3000.
5. Sign in using FaceBook :white_check_mark: and Google :white_check_mark:

> :red_circle: ISSUE: No logout button.

6. Test the "Sign with ORE-ID" function :white_check_mark:.
7. Enter PIN into boxes to sign transaction :white_check_mark:.
8. Receive Transaction ID, process ID, and state from signed transaction return :white_check_mark:.

### Using the Web-widget - [Step 3: Web-Widget](https://github.com/TeamAikon/ore-id-docs/tree/master/examples/react/tutorial/step3-web-widget)

1. Navigate to the step3-web-widget folder.

```shell
cd ../step3-web-widget
```

2. Install the dependencies.

```shell
npm i
```

3. Run the third sample app

```shell
yarn start
```

4. Let node open your browser to http://localhost:3000.
5. Login using FaceBook :white_check_mark: and Google :white_check_mark:.
5. Sign Transactions with web-widget using FaceBook :white_check_mark:  and Google :white_check_mark: .

> :red_circle: ISSUE: Logout does not clear cookies. Can only re-login using same account.

