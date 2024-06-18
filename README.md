# Zerops x Astro - SSR on Node.js 

![astro](https://github.com/zeropsio/recipe-shared-assets/blob/main/covers/cover-astro.png)

Astro is a server-first JavaScript web framework that supports every major UI framework, it's optimized for building fast, content-driven websites. [Zerops](https://zerops.io) makes deploying and running Astro sites, both server side rendered and static, a breeze. This recipe showcases the SSR version, see [zeropsio/recipe-astro-static](https://github.com/zeropsio/recipe-astro-static) for the static version.

<br/>

## Deploy on Zerops

You can either click the deploy button to deploy directly on Zerops, or manually copy the [import yaml](https://github.com/zeropsio/recipe-astro-nodejs/blob/main/zerops-project-import.yml) to the import dialog in the Zerops app.

<a href="https://app.zerops.io/recipe/astro-nodejs">
    <img width="250" alt="Deploy on Zerops" src="https://github.com/zeropsio/recipe-shared-assets/blob/main/deploy-button/deploy-button.png">
</a>

<br/>
<br/>

## Recipe features
- SSR version of **Astro 4.1** running on a load balanced **Zerops Node.js** service.

<br/>

## Production vs. development
This recipe is ready for production as is, and will scale horizontally in case of high traffic surges. If you want to achieve the highest baseline reliability and resiliace, start with at least two containers (add `minContainers: 2` in recipe YAML in the `app` service section, or change the minimum containers in "Automatic Scaling
configuration" section of service detail).

<br/>

## Changes made over the default installation
If you want to modify your own app running Astro to efficiently run on Zerops, these are the general steps we took:

- If you haven't already, add `@astrojs/node` package and implement it in your [astro.config.mjs](https://github.com/zeropsio/recipe-astro-nodejs/blob/main/astro.config.mjs#L15-L17)
- Add [zerops.yml](https://github.com/zeropsio/recipe-astro-nodejs/blob/main/zerops.yml) to your repository

<br/>
<br/>

Need help setting your project up? Join [Zerops Discord community](https://discord.com/invite/WDvCZ54).
