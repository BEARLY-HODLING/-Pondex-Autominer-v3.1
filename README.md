# -Pondex-Autominer-v3.1

Below is a detailed `README.md` file with installation instructions for both the **Pond0x Miner Automation** script (version 3.1) and the **Pond0x Status Injector** script (version 2.4). These instructions are designed to be clear and user-friendly for new users, helping them install the scripts, set up their environment, and start mining on Pond0x safely and efficiently. The README includes prerequisites, step-by-step guidance, troubleshooting tips, and important notes for multiple users.

---

# Pond0x Miner Automation and Status Injector Scripts

Welcome to the Pond0x Miner Automation and Status Injector scripts! These scripts work together to automate mining on [pond0x.com](https://www.pond0x.com) and provide real-time status updates, enhancing your mining experience. This README provides step-by-step instructions for installing and using both scripts, along with important safety and usage notes.

## Overview
- **Pond0x Miner Automation (v3.1)**: Automates the mining process on pond0x.com, handling mining starts, claims, errors, and restarts. It uses a status injector for real-time updates.
- **Pond0x Status Injector (v2.4)**: Injects mining status updates into a status mini window, sending data back to the miner script for monitoring.

Together, these scripts streamline mining, ensure reliability, and provide visibility into your mining progress.

## Prerequisites
Before installing and using these scripts, ensure you have the following:

- **Browser**: Google Chrome, Mozilla Firefox, or another browser that supports Tampermonkey (a user script manager).
- **Tampermonkey Extension**: Install Tampermonkey from the [Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) or [Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/).
- **Phantom Wallet**: Install and configure the Phantom wallet extension ([Chrome](https://chrome.google.com/webstore/detail/phantom/bfnaelmomeimhlpmgjnjophhpkkoljpa) / [Firefox](https://addons.mozilla.org/en-US/firefox/addon/phantom/)) for signing transactions on Pond0x.
- **Pond0x Account**: Create and log in to an account on [pond0x.com](https://www.pond0x.com).
- **Internet Connection**: A stable connection to access pond0x.com and related services.

## Installation Instructions

### Step 1: Install Tampermonkey
1. Open your browser and navigate to the Tampermonkey extension page:
   - For Chrome: [Tampermonkey on Chrome Web Store](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo)
   - For Firefox: [Tampermonkey on Firefox Add-ons](https://addons.mozilla.org/en-US/firefox/addon/tampermonkey/)
2. Click "Add to Chrome" or "Add to Firefox" and follow the prompts to install the extension.
3. After installation, you’ll see the Tampermonkey icon in your browser toolbar.

### Step 2: Install the Pond0x Status Injector Script
1. Copy the entire **Pond0x Status Injector** script (provided below) into a text editor.
2. Open Tampermonkey in your browser:
   - Click the Tampermonkey icon in your toolbar and select "Dashboard."
3. Click the "+ New User Script" or "Create a new script" button.
4. Paste the following script into the editor:


5. Click "File" > "Save" (or the equivalent in Tampermonkey’s interface) to install the script.
6. Ensure the script is enabled (it should automatically run on the specified `@match` URLs, like `https://cary0x.github.io/status-mini*`).

### Step 3: Install the Pond0x Miner Automation Script
1. Copy the entire **Pond0x Miner Automation** script (version 3.1, provided below) into a text editor.
2. Open Tampermonkey’s Dashboard again (as in Step 2).
3. Click the "+ New User Script" or "Create a new script" button.
4. Paste the following script into the editor:
5. Click "File" > "Save" (or the equivalent in Tampermonkey’s interface) to install the script.
6. Ensure the script is enabled (it should automatically run on `https://www.pond0x.com/*`).

### Step 4: Set Up Phantom Wallet
1. Install the Phantom wallet extension in your browser (see Prerequisites for links).
2. Create or import a wallet in Phantom, and ensure it’s connected to your Pond0x account.
3. Visit [pond0x.com](https://www.pond0x.com) and log in with your Phantom wallet to verify connectivity.

### Step 5: Start Mining
1. Open your browser and navigate to [https://www.pond0x.com/mining](https://www.pond0x.com/mining).
2. Ensure both scripts are enabled in Tampermonkey (check the Tampermonkey dashboard).
3. Keep the tab open and active. The Miner Automation script will automatically start mining, display a claim history box, and use the Status Injector to monitor progress.
4. Use a tab-keeper extension (e.g., "Keep Awake" or "Tab Reloader") to ensure the tab stays active, especially for daily resets at 23:59.

## Important Notes
- **Terms of Service**: Ensure you comply with [pond0x.com](https://www.pond0x.com)’s terms of service regarding automation. Using these scripts may violate their policies, potentially risking account suspension. Use at your own risk.
- **Safety**: The scripts modify Phantom wallet behavior and store data locally. Only install from trusted sources, and use a separate browser profile for each user to avoid data conflicts.
- **Logging**: The Miner Automation script includes verbose logging by default (`logVerbose = true`). For simpler logs, edit the script in Tampermonkey and set `logVerbose = false` before saving.
- **Multiple Users**: Each user should install the scripts in their own browser or Tampermonkey instance to prevent data overlap. The scripts use unique identifiers for storage, but separate profiles are recommended.
- **Troubleshooting**:
  - If mining doesn’t start, check the console (F12 or right-click > Inspect > Console) for errors (e.g., Phantom wallet not detected, popup blockers).
  - Ensure no content blockers or ad blockers interfere with `cary0x.github.io` or `pond0x.com`.
  - If the claim history box doesn’t appear, verify the LCD container is loaded on the page and no JavaScript errors occur.

## Troubleshooting Tips
- **Phantom Wallet Issues**: If you see `[Pond0x-Miner] - Phantom wallet not detected...`, install or configure the Phantom wallet extension and refresh the page.
- **Popup Blockers**: If the status mini popup fails, disable popup blockers for `cary0x.github.io` or allow popups in Tampermonkey settings.
- **Page Reloads**: If the script doesn’t restart after errors or claims, check `reloadReason` in the logs and ensure the page isn’t blocked from reloading.
- **Performance**: If the browser lags, reduce log verbosity (`logVerbose = false`) or use a tab-keeper to prevent tab sleep.

## Support
For issues or questions, contact [your support channel or email here]. Please include your browser, Tampermonkey version, and console logs for faster assistance.

## License
These scripts are provided as-is for personal use. No warranty is provided, and users are responsible for compliance with pond0x.com’s terms and local laws.

---
