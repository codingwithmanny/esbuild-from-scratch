# ESbuild From Scratch

## Requirements

- NVM or NodeJS version `14.17.5`
- Yarn version `1.22.10` or NPM version `6.14.6`
- Docker version `20.10.7` (For deployment)

## Local Development

Simply run:

```bash
yarn start; # or npm start;
```

## Build

To build the files into the `dist` folder, run:

```bash
yarn build; # or npm run build;
```

## Docker Deployment

To build the docker image:

```bash
docker build . -t your/image-name:tag
```

To test the build and run:

```bash
docker build . -t esbuild-from-scratch;
docker run -it -d -p 9000:80 --name esbuild esbuild-from-scratch;
```

To remove the test image:

```bash
docker rm -f esbuild;
```
