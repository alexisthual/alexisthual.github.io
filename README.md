# Personal website

## Run dev instance

From the `dev` branch, run the following commands in two separate prompts:

```bash
npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch
```

```bash
yarn start
```

## Deploy to production

Build with `yarn build` and push to `main` branch (which was setup to be deployed using github pages):

```bash
git checkout dev
yarn build
git checkout main
cp -R dist/* .
git push
```
