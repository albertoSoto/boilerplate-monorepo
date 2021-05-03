# Boilerplate for monorepo arch: NextJS, Lerna + Storybook

Project solving a NextJS scaffold with a shared-component library w/Storybook in a monorepo environment with Lerna

base article: https://buttercms.com/blog/nextjs-storybook-and-lerna-build-a-monorepo-structure

This project solves tiny bugs in the main repo and changes naming convention

Steps: 
- lerna init
- cd packages && yarn create next-app
- lerna create shared-ui

Let’s add microbundle to our components package, The above command will add microbundle as a dev-dependency.
- cd packages/shared-ui && yarn add microbundle -D

We can run the same command in both environment with
- lerna run dev

We can link repos with
- lerna bootstrap


