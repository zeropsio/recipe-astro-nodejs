```yml title="zerops.yml"
zerops:
  - setup: app
    build:
      base: nodejs@20
      buildCommands:
        - pnpm i
        - pnpm run build
      deployFiles:
        - dist
        - package.json
        - node_modules
      cache:
        - node_modules
        - pnpm-lock.yaml
    run:
      base: nodejs@20
      ports:
        - port: 3000
          httpSupport: true
      envVariables:
        PORT: 3000
        HOST: 0.0.0.0
      start: pnpm start
```
