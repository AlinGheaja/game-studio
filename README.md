# Game Studio v7



Game Studio is a tool for creation \`js-dos bundles\`

## Development

```
yarn start
```

## Web deployment

```
cd build && PUBLIC_URL=/studio NODE_ENV=production yarn build && aws s3 --endpoint-url=https://storage.yandexcloud.net sync . s3://dos.zone/studio --delete --acl public-read && cd ..
```
