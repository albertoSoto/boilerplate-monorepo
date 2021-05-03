# sandbox-monorepo

source: https://buttercms.com/blog/nextjs-storybook-and-lerna-build-a-monorepo-structure

Steps: 
- lerna init
- cd packages && yarn create next-app
- lerna create shared-ui

Let’s add microbundle to our components package, The above command will add microbundle as a dev-dependency.
- cd packages/components && yarn add microbundle -D

We can run the same command in both environment with
- lerna run dev
