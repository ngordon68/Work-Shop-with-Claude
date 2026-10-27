# Work-Shop-with-Claude

# Build Night Setup: Claude and Claude Code

This guide gets your computer ready for BuildNight on October 15th, 5:30 PM–8:30 PM at Tech Town Detroit.

Please finish Parts 1–4 **before** you arrive. Setup problems are much easier to fix at home than in a room of 30 people sharing Wi-Fi.

>We will use this workbook for tonight session [Idea_to_First_Version_Workbook-4.pdf](https://github.com/user-attachments/files/33516019/Idea_to_First_Version_Workbook-4.pdf)

 


---

## What you need

- A laptop running one of these:
  - macOS 13 (Ventura) or newer
  - Windows 10 (version 1809) or newer
  - Ubuntu 20.04+ or Debian 10+
- At least 4 GB of RAM
- A charger (bring it to the workshop)
- An email address you can check during setup

---

## Part 1: Create a Claude account

1. Go to **https://claude.ai**
2. Click **Sign up** and create an account with your email or Google account.
3. Confirm your email if asked.

### Which plan do you need?

| What you want to do | Free plan | Pro plan or higher |
|---|---|---|
| Chat with Claude, ideate, get feedback | Yes | Yes |
| Claude Design (wireframes) |Yes | Yes |
| Claude Code in the terminal | **No** | Yes |

---

## Part 2: Install the Claude app (optional but recommended)

You can use Claude in your web browser at https://claude.ai. The desktop app works the same way and is a little easier to keep open while you work.

1. Go to **https://claude.com/download**
2. Download the version for your computer (Mac or Windows).
3. Open the downloaded file and follow the installer.
4. Open Claude and sign in with the account from Part 1.

[FILL IN: Anything specific you want them to try in the app before the workshop, e.g. "Ask Claude to describe an app idea you've had."]

---

## Part 3: Open your terminal

The terminal is a window where you type commands instead of clicking. You only need it for Claude Code.

### Mac
1. Press **Command + Space** to open Spotlight.
2. Type **Terminal** and press **Enter**.

### Windows
1. Click the **Start** menu.
2. Type **PowerShell** and open **Windows PowerShell**.
3. You'll know you're in PowerShell if the line starts with `PS C:\`.

### Linux
Press **Ctrl + Alt + T**, or search for **Terminal** in your apps.

**Tip for beginners:** To paste into the terminal, use **Command + V** on Mac. On Windows PowerShell, use **Ctrl + V** or right-click.

[FILL IN: Any terminal basics you want them to know, e.g. what `cd` and `ls` do, how to make a project folder.]

---

## Part 4: Install Claude Code

Copy the command for your computer, paste it into your terminal, and press **Enter**.

### Mac, Linux, or WSL
```bash
curl -fsSL https://claude.ai/install.sh | bash
```

### Windows (PowerShell)
```powershell
irm https://claude.ai/install.ps1 | iex
```

### Windows (Command Prompt / CMD)
```batch
curl -fsSL https://claude.ai/install.cmd -o install.cmd && install.cmd && del install.cmd
```

The installer does not show a progress bar while it downloads. Wait until you see your normal prompt again.

**Windows users:** Installing [Git for Windows](https://git-scm.com/downloads/win) is optional but recommended. Claude Code works without it, using PowerShell instead.

### Check that it worked

1. **Close your terminal and open a new one.** This step is required.
2. Type this and press **Enter**:
   ```bash
   claude --version
   ```
3. You should see a version number, something like `2.1.211 (Claude Code)`.

If you see `command not found` or `not recognized`, go to the Troubleshooting section below.

---

## Part 5: Log in and run Claude Code for the first time

1. Make a folder for your workshop project and move into it:

   **Mac / Linux:**
   ```bash
   mkdir build-night
   cd build-night
   ```

   **Windows:**
   ```powershell
   mkdir build-night
   cd build-night
   ```

2. Start Claude Code:
   ```bash
   claude
   ```

3. A browser window will open asking you to log in. Sign in with the account from Part 1 and approve access.
4. Return to the terminal. You should see Claude Code waiting for your message.
5. Try a first message:
   ```
   What files are in this folder?
   ```
6. To exit Claude Code, type `/exit` or press **Ctrl + C** twice.

Official install troubleshooting: https://code.claude.com/docs/en/troubleshoot-install

---

## What we'll do at the workshop

1. **Ideate:** Come up with a new idea, or get critical feedback on one you already have.
2. **Wireframe:** Use Claude Design to generate and compare different wireframes.
3. **Plan:** Turn the wireframe you pick into a build plan.
4. **Build:** Execute that plan in **[FILL IN: default platform/IDE]**.
5. **Demo:** 8:00–8:30 PM, volunteers show what they built.

You'll leave with a wireframe, a written build plan, and the first working version of your project.

---

## Resources

**Official docs**
- Claude Code quickstart: https://code.claude.com/docs/en/quickstart
- Terminal guide for first-timers: https://code.claude.com/docs/en/terminal-guide
- Installation and system requirements: https://code.claude.com/docs/en/setup
- Install troubleshooting: https://code.claude.com/docs/en/troubleshoot-install
- Claude Help Center: https://support.claude.com
- Prompting guide: https://docs.claude.com/en/docs/build-with-claude/prompt-engineering/overview

**Free courses**
- Anthropic Academy: https://anthropic.skilljar.com

**Other tools**
- Git for Windows: https://git-scm.com/downloads/win


---
