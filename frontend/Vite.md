# Vite

## What is it?
Vite is a toolchain for React apps, similar to CRA (Create React App). It's very closely modeled after CRA but with much faster builds.

### Highlights
- **🐆 Fast!!!**. Implemented in Rust so much faster than JavaScript.
- **Fast Hot Module Replacement**: Hot module replacement happens very quickly!
- **Flexible**. Similar to CRA but modernized.
- **Opensource**. Less profit motive than Next.js which tries to push its wares.
- **Code Splitting**: Code splitting avilable
- **SSR**: Possible to add server-side rendering.

### Comparisons

**Versus CRA**.  CRA is showing its age and not likely to be maintained in the future.

**Versus Next.js**. Next.js has many strange design decisions that I personally dislike (strange routing, over-emphasis on SSR, incompatability with redux). And it's very opinionated. It's also a for-profit endeavor and tends to push its Vercel hosting platform, which I'm not a fan of.

## Getting started
I was able to get started using [this guide](https://vitejs.dev/guide/) and use it in less than 5 minutes!

```bash
yarn create vite
```

First impression: Very impressive speed!

## Gotcha: Environment Variables
Add a `VITE_` prefix (like `REACT_APP_`) to pass environment variables into the application.  `REACT_APP` prefixes will not work!

## GitHub Actions
Template available [here](https://github.com/hywax/github-action-template)!

🎉 That's about all there is to it. It's very similar to CRA--just better! (Or so it seems...)