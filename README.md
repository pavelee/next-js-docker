# Next.js Docker

Run your next.js app in container.

With one command you will have simulesly working DEV and PROD enviorment. It's really usefull to test your app on both enviorments during development.

By default, it is typescript version of Next.js

## How to run?

### fetch repo
```
 git clone https://github.com/pavelee/next-js-docker.git
```
### inside project dir
```
docker-compose up -d
```
### enjoy enviorments
- DEV -> http://localhost:3000
- PROD -> http://localhost:3001

## Rebuild production

Production is optimized and not changing with files editing.
If you would like to refresh production build, you need to rebuild docker image by command:
```
docker-compose up -d --build --force-recreate
```