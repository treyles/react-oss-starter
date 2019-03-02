# React OSS Starter

A a boilerplate for publishing React components to NPM

(Based on an [article](https://medium.com/@BrodaNoel/how-to-create-a-react-component-and-publish-it-in-npm-668ad7d363ce) by Noel Broda)

## Getting Started

Update the following fields in `package.json` with your project information:

```
"name": "react-oss-starter",
"version": "0.0.0",
"description": "description",
"repository": {
	"url": "http://github-url.com"
}
```

In the `root` directory, install node modules:

```
yarn
```

Run the build and watch for changes:

```
yarn start
```

Your component to be published will be in the `src` directory

## Test Your Component Locally

### Create a Symlink

The test project lives in the `example` directory. To be able to import your new component into the test project, we need to create a link between the `root` and `example` directories using a symlink. This is a two step process:

In the `root` directory, run:

```
yarn link
```

In the `example` directory, run:

```
yarn link [name of your project]
```

`[name of your project]` corresponds to the `name` field in `package.json` (root)

### Run Test Project

In the `example` directory, install node modules:

```
yarn
```

then run the dev server:

```
yarn start
```

## Publish to NPM

In the `root` directory, run:

```
yarn publish
```

🎉🎉🎉
