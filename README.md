# Shabad OS Library

Plain vanilla javascript vite project wrapped in electron. Make quadrilateral shapes to dewarp pages.

## Usage

- Clone repo
- `npm i`
- `npm run dev`
- Use "Open Directory" button on the top left to choose a folder containing JPEG images (i.e. files ending in `.jpg` or `.jpeg`).
- Use the file picker on the left side to open an image
- Click on the image to set the 4 points of the quadrilateral (must be in order of Top-Left -> Top-Right -> Bottom-Right -> Bottom-Left)
- Hold-and-drag any 4 points of the quadrilateral to adjust
- Use the "Preview" button at the bottom to get an idea of the transform.
- Once done with images, use "Export" on the top left to create a file
- After exporting, the app will ask if you want to clear the local storage (this will delete all saved information about quadrilaterals and their 4 points)
- You may use the "Import" button top left to use an exported file to get data back

## Dev

- Main files for development are located in `src/renderer/index.html` and it's corresponding js/ts and style files
- Only changes to electron are found in `src/main/index.ts`:

```js
// https://github.com/electron/electron/issues/28422
app.commandLine.appendSwitch('enable-experimental-web-platform-features')
```