# Solarized Dark Patched for Windows Terminal

Using the built-in solarized dark color scheme, I would notice that options and arguments for commands would be invisible since they were rendered with the background color. This color scheme fixes that. See below screenshot where  you can clearly see the `-m` when committing.

![Screenshot of color scheme in Windows Terminal](screenshot.png)


## Installation Instructions for Custom Color Scheme in Windows Terminal

Follow these steps to install and use this custom color scheme in your Windows Terminal:

### 1. Locate the `settings.json` File
The `settings.json` file contains all your Windows Terminal settings including color schemes. You can find the defulat locations at [[Link text Here](https://learn.microsoft.com/)](https://learn.microsoft.com/en-us/windows/terminal/install#settings-json-file). A typical location for this file is at:

```plaintext
%LOCALAPPDATA%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\LocalState\settings.json
```

To quickly open this location:
- Press `Win + R` on your keyboard.
- Type or paste the above file path and press Enter.

### 2. Edit the `settings.json` File
Open the `settings.json` file using a text editor such as Notepad or Visual Studio Code.

### 3. Add the Custom Color Scheme
Within the `settings.json` file, locate the `"schemes": [ … ]` section. This section lists all custom color schemes. Follow these steps to add the new scheme:

- Scroll to the `"schemes"` array.
- Add the JSON snippet of the custom color scheme to the end of this array.
- Ensure proper JSON formatting:
  - Add a comma `,` at the end of the previous color scheme entry if it's not the last item in the list.
  - The color scheme JSON should look like this:

    ```json
    {
        "name": "Solarized Dark Patched",
        "cursorColor": "#657b83",
        "background": "#002b36",
        // Other color settings...
    }
    ```

### 4. Apply the Custom Color Scheme
After adding the custom color scheme to the `settings.json` file, apply it by following these steps:

- Open Windows Terminal.
- Access "Settings" via the dropdown menu or use the shortcut `Ctrl + ,`.
- In the "Profiles" tab, select your desired profile (e.g., PowerShell, Command Prompt).
- Find the "Color scheme" dropdown under the "Appearance" section.
- Select the name of your newly added custom color scheme.
- Save the changes.

### 5. Troubleshooting
If the new color scheme does not appear correctly, check for syntax errors in the JSON snippet. Common errors include missing brackets, commas, or incorrect string formats.

### 6. Restart Windows Terminal
After saving your settings, restart Windows Terminal to see the new color scheme in action.
