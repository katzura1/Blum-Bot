# Blum-Bot Autoclaim Script

This script automates the process of claiming rewards or points in the Blum App. It uses the Telegram development console to retrieve the necessary tokens and then interacts with the Blum App to perform the autoclaim function.

## Step-by-Step Instructions

1. **Open the Telegram Developer Console**
   - Open Telegram and navigate to the developer console to inspect network requests and extract necessary tokens.

2. **Open the Blum App**
   - Access the Blum App on your device to initiate the process of retrieving tokens.

3. **Obtain Authorization Token**
   - In the Telegram console, find the HTTP request header with the `Authorization` field.
   - Extract the token that follows the "Bearer " prefix. This is your `auth_token`.

4. **Obtain Refresh Token**
   - In the Telegram console, locate the endpoint `/refresh` in the network tab.
   - Find the payload data and extract the refresh token. This is your `ref_token`.

5. **Edit the Script**
   - Open the script file `blum.py`.
   - Replace `auth_token` with the extracted Bearer Token from step 3.
   - Replace `ref_token` with the extracted payload refresh token from step 4.

6. **Run the Script**
   - Ensure you have Python installed on your system.
   - Open a terminal or command prompt in the directory where `blum.py` is located.
   - Run the script using the following command:
     ```bash
     python blum.py
     ```

## Troubleshooting

- **Error with Tokens:** Double-check the extracted tokens for any typos or missing characters.
- **Python Not Found:** Ensure Python is installed and correctly added to your system's PATH.
- **Script Issues:** If the script does not work as expected, check the error messages for clues and confirm all steps were followed correctly.

## Disclaimer

This script is intended for educational purposes and personal use only. Please ensure you have permission to use any tools or applications involved. Misuse or unauthorized access to services or applications may violate terms of service or the law. Use this script responsibly and at your
