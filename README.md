# Linear Issue Opener Alfred Workflow

This Alfred workflow allows you to quickly open Linear issues in either the desktop app or web browser, streamlining your project management workflow.

## Features

- Open Linear issues directly from Alfred
- Supports both desktop app and web browser fallback
- Automatically adds default project prefix to issue numbers
- Uses clipboard content if no argument is provided

## Setup

1. Install the workflow in Alfred
2. Configure the following workflow variables:
   - `ORGANIZATION`: Your Linear organization name (e.g., "acne")
   - `DEFAULT_PROJECT`: Your default project prefix (e.g., "PROJ")

## Usage

Use the keyword `li` followed by an issue identifier:

- `li PROJ-1000`: Opens issue PROJ-1000
- `li 1000`: Opens issue PROJ-1000 (assuming PROJ is your default project)
- `li`: Opens the issue ID from your clipboard

## Behavior

1. The workflow first attempts to open the issue in the Linear desktop app
2. If the desktop app fails to open the issue, it falls back to opening in the default web browser
3. If no issue ID is provided and the clipboard is empty, a notification is displayed

## Troubleshooting

- Ensure the Linear desktop app is installed and running
- Check that your `ORGANIZATION`, `DEFAULT_PROJECT` variables are correctly set
- Review Alfred's debug console for any error messages

## Customization

You can modify the script to change the default behavior, such as:
- Altering the keyword
- Changing the fallback behavior
- Adding support for multiple organizations or projects

## Contributing

If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project's repository.

## License

This workflow is released under the MIT License. See the LICENSE file for more details.
