# HTML, CSS, JS for Web-developers (Coursera)

## Github Pages

- Select `Deploy from branch` option with the branch as `main` and folder as `root(/)`
- URL format is "https://`username`.github.io/`reponame`/"

## http-server (Recommended)

Syntax: `http-server [path] [options]`

Use via `npx` to use it on-demand

```sh
npx http-server ./src -c-1
```

Refer their [README](https://github.com/http-party/http-server#available-options) for using the options

## Browser Sync (NOT Recommended)

- Install globally via `npm`:

  ```sh
  npm install -g browser-sync
  ```

- Start watching files:

  ```sh
  browser-sync start --server --files "*.html" "*.css"
  ```
