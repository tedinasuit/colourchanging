# Colourchanging

This repository contains a simple web application that allows you to control the background color of a webpage and synchronize it with a Hue light connected to a Hue Bridge.

## Files

The repository consists of the following files:

- `index.html`: The main HTML file that contains the web application code.
- `colour-settings.html`: The HTML file for configuring custom color settings.
- `style/style.css`: The CSS file for styling the web application.
- `style/colour-settings.css`: The CSS file for styling the color settings page.

## Usage

1. Open `index.html` in a web browser to view the web application.
2. Use the dropdown menu to select a color or choose "Auto" for automatic color updates.
3. Click the "Colour Settings" link to configure custom color settings.
4. In the color settings page (`colour-settings.html`), choose colors for each hour of the day.
5. Click the "Save" button to store the color settings.
6. The background color of the web application will update according to the selected color or the automatic color settings.
7. The web application will also update the color of the connected Hue light (requires a Hue Bridge and valid configuration).

## Dependencies

The web application relies on the following dependencies:

- [Axios](https://github.com/axios/axios): A promise-based HTTP client for making requests to the Hue API.

## Note

- The IP address of the Hue Bridge, API token, and light ID are hardcoded in the JavaScript code. Modify them according to your Hue Bridge setup.

`index.html`:
```
      let mode = 'auto';
      // The IP of the Hue Bridge I want to connect to
      const hueBridgeIP = '192.168.178.17';
      // The API token of the Hue Bridge
      const username = 'aMzAUrHbPTUJJUuaaDsoLXyYrCIVF6yZDGZRTVHb';
      // The ID of the Hue light I want to control
      const lightId = '4';

```

Feel free to explore the code and customize it as needed!
