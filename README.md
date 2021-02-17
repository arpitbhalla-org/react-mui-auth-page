# react-mui-auth-page

![npm](https://img.shields.io/npm/v/react-mui-auth-page?style=flat-square) ![npm](https://img.shields.io/npm/dm/react-mui-auth-page?style=flat-square) ![NPM](https://img.shields.io/npm/l/react-mui-auth-page?style=flat-square) ![Snyk Vulnerabilities for npm package](https://img.shields.io/snyk/vulnerabilities/npm/react-mui-auth-page?style=flat-square) ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/npm/react-mui-auth-page?style=flat-square)

## Getting Started

`npm i react-mui-auth-page`

## [Demo](https://react-mui-auth-page.surge.sh)

## Usage

```js
import { DialogAuth, BoxAuth, FullWidthAuth } from "react-mui-auth-page";
```

## Examples

<img src='./example/Demo.png'>

#### Dialog

```js
import React from "react";
import { DialogAuth } from "react-mui-auth-page";
import Button from "@material-ui/core/Button";

const Dialog = () => {
  const handleSignIn = ({ email, password }) => {
    console.log({ email, password });
  };
  const handleSignUp = ({ email, name, password }) => {
    console.log({ email, name, password });
  };
  const handleForget = ({ email }) => {
    console.log({ email });
  };
  const handleLinkedIn = () => {
    console.log("Do Linkedin call");
  };
  const handleGithub = () => {
    console.log("Do Github call");
  };

  return (
    <>
      <DialogAuth
        open={true}
        onClose={() => {}}
        handleSignUp={handleSignUp}
        handleForget={handleForget}
        handleSignIn={handleSignIn}
        handleSocial={{
          Linkedin: handleLinkedIn,
          Github: handleGithub,
        }}
      />
    </>
  );
};

export default Dialog;
```

## Local Run

```
npm install
```

```
npm run dev
```

## Get Involved!

- Pull requests are welcome!
- Submit github issues for any feature enhancements, bugs or documentation problems

## Maintainer

[arpitBhalla](https://github.com/arpitbhalla)
