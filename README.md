# AutozSignup

AutozSignup is an advanced Tampermonkey script designed to automate the process of filling out signup forms and managing temporary email addresses for anonymous registrations.

## Features

- **Automatic Form Filling**: Intelligently detects and fills out signup forms with randomly generated data.
- **Temporary Email Generation**: Creates and manages a temporary email address for each session.
- **Email Checking**: Allows users to check the temporary email inbox for verification messages.
- **Activation Link Detection**: Automatically detects account activation links in received emails.
- **React Compatibility**: Works with both traditional websites and modern React-based applications.
- **Persistent Storage**: Saves the temporary email address using IndexedDB for use across page reloads.
- **Dynamic Content Support**: Continuously monitors for new form fields added to the page.

## Installation

1. Make sure you have the Tampermonkey browser extension installed. If not, you can get it from [the official Tampermonkey website](https://www.tampermonkey.net/).
2. Click on the Tampermonkey icon in your browser and select "Create a new script".
3. Delete any existing code in the editor.
4. Copy and paste the entire AutozSignup script into the Tampermonkey editor.
5. Click "File" > "Save" or use the keyboard shortcut Ctrl+S (Cmd+S on Mac) to save the script.

## Usage

1. Navigate to any webpage where you want to use the automated signup.
2. You'll see two buttons in the bottom-right corner of the page:
   - **Try Anonymous**: Fills out forms and generates a temporary email (if not already generated).
   - **Check Email**: Checks for and displays any received messages in the temporary email inbox.
3. Click "Try Anonymous" to automatically fill out any signup forms on the page.
4. If you receive a verification email, click "Check Email" to view it.
5. If an activation link is detected in the email, an "Activate Account" button will appear, allowing you to open the link in a new tab.

## Important Notes

- This script is intended for educational and testing purposes only. Always respect website terms of service and legal considerations.
- The script uses the 1secmail.com API for temporary email services. Be aware of their usage policies and limitations.
- While efforts have been made to ensure compatibility with various websites, including React-based ones, some sites may have additional protections that prevent automated form filling.
- The script generates random user data. Do not use it to create accounts with false information on services you intend to use legitimately.
- Be cautious when using this script, as automated account creation may be against the terms of service of many websites.

## Customization

You can customize the script by modifying the following sections:

- `generateRandomData()`: Adjust the pool of random names, or add more fields as needed.
- `fieldMap` in `fillFormFields()`: Modify or add new field detection patterns.
- `tempMailService`: Change the temporary email service if desired (requires adjusting the API calls accordingly).

## Troubleshooting

- If the buttons disappear on some websites, they should reappear within 5 seconds. If they don't, try refreshing the page.
- If form filling doesn't work on a particular website, check the browser console for any error messages.
- For persistent issues or feature requests, please open an issue in the project repository.

## Disclaimer

This script is provided as-is, without any warranties or guarantees. Users are responsible for ensuring they comply with all relevant laws and website policies when using this script.

## Contributing

Contributions to improve AutozSignup are welcome! Please feel free to submit pull requests or open issues to suggest improvements or report bugs.

## License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).