# New JS Project

To start a new JS project, first run:

```
yarn init
```
Answer the questions about the project. Options between parentheses are the defaults.

## [name](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#name)
Not required, unless you plan to publish it:

```
question name (new-js-project):
```

## [version](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#version)
Also not required unless planning to publish. For personal private projects I like starting with `0.0.1`:

```
question version (1.0.0): 0.0.1
```
## [description](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#description)
Optional and recommended if planning to publish the package:

```
question description: a new JS project
```


## [entry point (main)](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#main)
Indicates the path to the primary package export or the main file that will be executed. Not required if the package will not be imported by other packages.

```
question entry point (index.js):
```

## [repository url (repository)](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#repository)
The URL for the repository. To add a shorthand for a GitHub repo, use this:

`git+https://github.com/user/repo.git`

Note: yarn understands the following versions.

Short version:

```json
{
  "repository": "github:user/repo"
}
```
Long version (from npm docs):
```json
{
  "repository": {
    "type": "git",
    "url": "https://github.com/user/repo.git"
  }
}
```
Prompt will look like this:

```
question repository url: "github:simona1/new-js-project"
```


## [author](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#author)
This prompt is for adding the author name. To have your `.gitconfig` settings for email and username auto-filled, run `yarn init` from the root of a git repo.

```
question author: Stela Palii
```


## [license](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#license)

Public open source projects often use the MIT license. If your project is private you can start with UNLICENSED.

```
question license (MIT): UNLICENSED
```


## [private](https://docs.npmjs.com/cli/v9/configuring-npm/package-json?v=true#private)
A good default for this question is `true`:

```
question private: true
```


## Reference template

```json
{
  "name": "TO-BE-REPLACED-WITH-YOUR-PACKAGE-NAME",
  "version": "0.0.1",
  "repository": "github: TO-BE-REPLACED-WITH-YOUR-GITHUB-USERNAME/TO-BE-REPLACED-WITH-YOUR-GITHUB-REPOSITORY-NAME",
  "author": "TO-BE-REPLACED-WITH-YOUR-NAME <TO-BE-REPLACED-WITH-YOUR-EMAIL>",
  "license": "UNLICENSED",
  "private": true
}
```

