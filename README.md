# Zerops + Astro - Nodejs

![Header Image](/header.png)

A Nodejs Astro example for Zerops which you can deploy in 2 simple steps.

**Features**

- Astro
- Tailwind

## Instructions to Deploy on Zerops

1. Navigate to the Zerops Dashboard and locate the import project button on the sidebar.

2. Paste the Project Yaml

```yaml
project:
  name: astro

services:
  - hostname: astronode
    type: nodejs@20
    buildFromGit: https://github.com/fxck/zerops-astro-nodejs
    ports:
      - port: 4321
    enableSubdomainAccess: true
    minContainers: 1
```

If you still find yourself stuck in the process join our [Discord community](https://discord.gg/5ptAqtpyvh).
