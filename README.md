# Zerops x Astro - Nodejs

![Header Image](header.png)

A Node.js Astro app deployment example for [Zerops](https://zerops.io) - a developer first cloud platform.

## Deploy to Zerops

1. [Create an account](https://app.zerops.io/registration) and locate the "Import project" button in the top left menu.
2. Copy & paste the YAML setup below and confirm

```yaml
project:
  name: zerops-astro

services:
  - hostname: astronode
    type: nodejs@20
    buildFromGit: https://github.com/zeropsio/recipe-astro-nodejs
    ports:
      - port: 4321
        httpSupport: true
    enableSubdomainAccess: true
    minContainers: 1
```

Join [Zerops Discord community](https://discord.com/invite/WDvCZ54).
