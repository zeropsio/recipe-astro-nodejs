```yml
project:
   name: astro

  services:
   - hostname: astronode
    type: nodejs@20
    buildFromGit: https://github.com/fxck/zerops-astro-nodejs
    ports:
      - port: 4321
        httpSupport: true
    enableSubdomainAccess: true
    minContainers: 1
```
