# Development has moved to [shabados/shabados](https://github.com/shabados/shabados)

This repo has been archived in favor of the above monorepo.

<details>
<summary>Archived README</summary>

# Shabad OS Library

Make quadrilateral shapes to dewarp pages. ([Check out the Shabad OS Library User Guide](https://www.shabados.com/support/guide/library/welcome/))

## Dev

- Main files for development are located in `src/renderer/index.html` and it's corresponding js/ts and style files
- Only changes to electron are found in `src/main/index.ts`:

```js
// https://github.com/electron/electron/issues/28422
app.commandLine.appendSwitch("enable-experimental-web-platform-features");
```

</details>
