This repo is extracted from monorepo > api-client auto generated package.

Reason for extraction is that we're moving to polyrepo setup and gql so continue having a working client for the time being, we'll need this as a seperate repo.

If you need to modify any endpoints:

1. modify the controllers in monorepo > api package
2. run yarn build && yarn generate in api directory
3. copy monorepo/packagess/api-client/src to ./src
4. run yarn build at root of this repo
5. merge changes to main
6. run yarn install on your client to get latest changes
