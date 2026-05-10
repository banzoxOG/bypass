# Bypass

A utility tool designed to help you bypass certain restrictions and limitations in your system environment.

## 📋 Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Configuration](#configuration)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

---

## ✨ Features

- Fast and efficient bypass solutions
- Easy-to-use interface
- Minimal system resource consumption
- Secure and reliable performance
- Cross-platform compatibility

---

## 📥 Installation

### Requirements
- Windows 10 or higher
- Administrator privileges
- .NET Framework (or as required by your version)

### Steps

1. **Clone the repository:**
   ```bash
   git clone https://github.com/banzoxOG/bypass.git
   cd bypass
   ```

2. **Download the latest release:**
   - Visit [Releases](https://github.com/banzoxOG/bypass/releases)
   - Download the latest executable or packaged version

3. **Extract files:**
   - Unzip the downloaded file to your preferred location
   - Ensure the main executable has proper permissions

4. **Run the application:**
   - Double-click the executable or run via command line
   - Grant administrative privileges when prompted

---

## 🚀 Usage

### Basic Usage

```bash
bypass.exe [options]
```

### Command Line Options

| Option | Description |
|--------|-------------|
| `-h` or `--help` | Display help message and available options |
| `-v` or `--version` | Show current version |
| `-c` or `--config` | Load custom configuration file |
| `-d` or `--debug` | Enable debug mode for detailed logging |

### Example Commands

```bash
# Run with default settings
bypass.exe

# Run with custom configuration
bypass.exe -c config.ini

# Enable debug mode
bypass.exe -d
```

---

## 📂 How to Use: Drag & Drop Method (Simple Setup)

### 🎯 Easy File Location Method

This is the **simplest way** to use the bypass tool without needing full administrator privileges!

#### Step 1: Open File Location

1. **Locate the file** you want to bypass (the target application or file)
2. **Right-click** on the file
3. **Select "Open file location"** from the context menu
   - This opens the folder containing your file in Windows Explorer

#### Step 2: Drag & Drop the App

1. **Keep the File Explorer window open** with your target file visible
2. **Open another window** or tab showing where you installed `bypass.exe` (steuper.exe)
3. **Drag the bypass app** (`steuper.exe`) **into the File Explorer window** where your target file is located
   - Alternatively, copy `steuper.exe` into the same folder as your target file

#### Step 3: Run the Bypass

1. **In the same folder**, you'll now have both:
   - Your target file/application
   - `steuper.exe` (the bypass tool)

2. **Double-click `steuper.exe`** to run it
   - The tool will automatically detect and process files in the same directory

3. **It will work without needing admin rights!** ✅

---

### 📍 Alternative: Copy Method

If drag-and-drop doesn't work:

1. **Navigate to your target file's folder**
   - Right-click the file → **"Open file location"**

2. **Copy `steuper.exe`** from the bypass installation folder
   - Right-click `steuper.exe` → **Copy**

3. **Paste it** into the target file's folder
   - Right-click in empty space → **Paste**

4. **Double-click the pasted `steuper.exe`** to run
   - Works without admin rights when in the same folder!

---

### ⚙️ Admin Rights Requirements

#### ✅ When You DON'T Need Admin Rights:
- Using the **Drag & Drop method** (same folder)
- Running on files in your **User folder** (Documents, Downloads, Desktop)
- Processing files with **standard permissions**
- Using the bypass in **portable mode**

#### ⚠️ When You MIGHT Need Admin Rights:
- Targeting **system files** in `C:\Windows\System32`
- Modifying **protected registry entries**
- Accessing **Program Files** directory (depending on permissions)
- Running **system-level operations**

#### 💡 Pro Tip: Run Without Admin
To run the bypass **without administrator privileges**:

1. **Right-click `steuper.exe`**
2. **Select "Run as different user"**
3. Choose your standard user account (not admin)
4. Enter your password if prompted

This allows you to process user-level files without full admin access.

---

### 🎬 Step-by-Step Example

**Scenario:** You want to bypass a file called `target.exe` in your Downloads folder

```
1. Open File Explorer
2. Navigate to: C:\Users\YourUsername\Downloads
3. Find: target.exe
4. Right-click target.exe → "Open file location"
5. File location now open in Windows Explorer
6. Drag steuper.exe (from installation folder) → into this Downloads folder
7. Double-click steuper.exe in the Downloads folder
8. Done! ✅ No admin rights required!
```

---

### 📋 Verification Checklist

Before running, make sure:

- [ ] Both `steuper.exe` and target file are in the **same folder**
- [ ] You have **read/write permissions** for that folder
- [ ] The file location is **not a protected system folder**
- [ ] No other instance of `steuper.exe` is running
- [ ] Your antivirus is **not blocking the application**

---

## 🎯 Advanced: Using bypass.bat (Batch Script Method)

### 📜 What is bypass.bat?

The `bypass.bat` file is a batch script that allows you to bypass restrictions using the Windows compatibility layer system. This method is even more powerful and doesn't require admin rights!

### 📝 bypass.bat Content

```batch
cmd /min /C "set __COMPAT_LAYER=yourpcusername && start "" "%1"
```

### 🔧 How to Create and Use bypass.bat

#### Step 1: Create the Batch File

1. **Open Notepad:**
   - Press `Win + R`
   - Type `notepad` and press Enter

2. **Paste this code:**
   ```batch
   cmd /min /C "set __COMPAT_LAYER=yourpcusername && start "" "%1"
   ```

3. **Replace `yourpcusername`:**
   - Replace `yourpcusername` with your actual Windows username
   - Example: `set __COMPAT_LAYER=JohnDoe && start "" "%1"`
   - To find your username: Right-click "This PC" → Properties → see username

4. **Save the file:**
   - Press `Ctrl + S`
   - Name it: `bypass.bat`
   - Choose location: Same folder as your target file
   - **Important:** Select "All Files" as file type, not "Text Document"

#### Step 2: Use the Batch Script

1. **Drag your target file** onto `bypass.bat`
   - The application will launch with compatibility mode enabled

2. **Or right-click the batch file:**
   - Select "Run as administrator" (optional)
   - It will process any target files in the same directory

3. **The magic happens:**
   - `__COMPAT_LAYER` environment variable sets compatibility mode
   - `/min` flag runs the command window minimized (hidden)
   - No admin rights needed! ✅

---

### 🎬 Complete Example with bypass.bat

**Scenario:** You have a file called `app.exe` and want to bypass it

```
1. Create bypass.bat with your username:
   cmd /min /C "set __COMPAT_LAYER=YourUsername && start "" "%1"

2. Save both files in same folder:
   C:\Users\YourUsername\Documents\
   ├── app.exe
   └── bypass.bat

3. Drag app.exe onto bypass.bat
   OR
   Right-click bypass.bat → Run as administrator

4. app.exe launches with bypass enabled! ✅
```

---

### 🔑 How __COMPAT_LAYER Works

The `__COMPAT_LAYER` environment variable enables Windows compatibility modes:

| Mode | Value | Effect |
|------|-------|--------|
| `yourpcusername` | Your PC username | Runs as your user, bypasses certain restrictions |
| Standard | (Default) | Normal execution |
| Custom | Various modes | Can enable specific compatibility features |

**Benefits:**
- ✅ No admin elevation needed
- ✅ Bypasses UAC prompts for lower-level operations
- ✅ Maintains user session context
- ✅ Works with drag-and-drop files
- ✅ Minimized command window (hidden from view)

---

### ⚙️ Finding Your Windows Username

If you don't know your Windows username:

**Method 1 - Command Prompt:**
```bash
echo %USERNAME%
```

**Method 2 - System Properties:**
1. Right-click "This PC" or "My Computer"
2. Select "Properties"
3. Look for "Full computer name" or "User name"

**Method 3 - File Explorer:**
1. Open File Explorer
2. Click on "This PC"
3. In the address bar, you'll see: `C:\Users\YourUsername`

---

### 💡 Tips & Tricks

**Tip 1: Use Both Methods Together**
- Use the **batch script method** for primary bypass
- Keep **steuper.exe** in the folder as backup
- Run whichever one works best for your situation

**Tip 2: Create Multiple Versions**
```batch
rem Version for Admin bypass
cmd /min /C "set __COMPAT_LAYER=ADMIN && start "" "%1"

rem Version for Standard bypass
cmd /min /C "set __COMPAT_LAYER=YourUsername && start "" "%1"
```

**Tip 3: Silent Execution**
To run completely silently (no window at all):
```batch
start "" "%1"
```

**Tip 4: Check Execution Status**
Add this line to see if it worked:
```batch
echo Bypass executed. Press any key to close...
pause
```

---

### 🚨 Troubleshooting bypass.bat

| Problem | Solution |
|---------|----------|
| "File not found" | Make sure batch file is in same folder as target |
| "Invalid username" | Check your Windows username spelling |
| "Still asks for admin" | Use "Run as administrator" on the batch file |
| "Command window stays open" | Remove the `/min` flag temporarily to debug |
| "File won't run" | Verify `.bat` extension (not `.txt`) |

---

---

## ⚙️ Configuration

### Configuration File Structure

Create a `config.ini` file in the application directory:

```ini
[Settings]
EnableLogging=true
LogLevel=INFO
Timeout=30000
RetryAttempts=3

[Advanced]
VerboseMode=false
OutputFormat=default
```

### Environment Variables

- `BYPASS_CONFIG` - Path to custom configuration file
- `BYPASS_DEBUG` - Set to `1` to enable debug mode

---

## 🔧 Troubleshooting

### ❌ Problem: Application Doesn't Work

**Symptom:** The application fails to run or produces errors.

#### Solution

Follow these steps to resolve the issue:

1. **Press `Win + R`** (Windows key + R simultaneously)
   - This opens the Run dialog

2. **Type `gpedit.msc`** in the Run dialog
   - Click **OK** or press **Enter**
   - The Group Policy Editor will open

3. **Navigate to User Configuration:**
   - In the left panel, expand: **User Configuration**
   - Then expand: **Administrative Templates**
   - Click on: **System**

4. **Find "Prevent access to the command prompt":**
   - In the center panel, scroll to find **"Prevent access to the command prompt"**
   - Double-click on this policy

5. **Verify the Configuration:**
   - In the dialog that opens, check the status:
     - **Not Configured** ✅ (Recommended - allows access)
     - **Disabled** ✅ (Allows access)
     - **Enabled** ❌ (Blocks access - this is the problem)

6. **If it's Enabled:**
   - Select **"Not Configured"** or **"Disabled"**
   - Click **Apply**
   - Click **OK**
   - Close Group Policy Editor

7. **Restart your computer** for changes to take effect

#### Additional Troubleshooting Steps

- **Verify Administrator Privileges:**
  ```bash
  whoami /priv
  ```
  Ensure `SeDebugPrivilege` is present

- **Check System Logs:**
  - Open Event Viewer: `eventvwr.msc`
  - Look under **Windows Logs > Application** for errors

- **Disable User Account Control (UAC) temporarily:**
  - Search for "UAC" in Windows search
  - Adjust settings to lowest level
  - Restart and test again

- **Run in Compatibility Mode:**
  - Right-click `bypass.exe`
  - Select **Properties**
  - Go to **Compatibility** tab
  - Try running in compatibility mode for Windows 7 or 8

---

### 🔗 Alternative Solutions

If Group Policy Editor is not available (Windows Home editions):

**Using Registry Editor:**
```bash
regedit.exe
```

Navigate to:
```
HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows\System
```

- Find or create: `DisableCMD`
- Ensure value is set to `0` (disabled) or delete the entry
- Restart your computer

---

### 📱 Common Error Messages

| Error | Cause | Solution |
|-------|-------|----------|
| "Access Denied" | Insufficient permissions | Run as Administrator |
| "Command not found" | CMD blocked by policy | Verify GPEdit settings |
| "File not found" | Missing configuration file | Create default config.ini |
| "Timeout error" | System too slow | Increase timeout in config |

---

## 🛠️ Advanced Configuration

### Debug Mode Output

Enable detailed logging:

```bash
bypass.exe -d > debug.log 2>&1
```

### Performance Tuning

Modify `config.ini` for better performance:

```ini
[Performance]
MaxThreads=4
CacheSize=512
CompressionLevel=9
```

---

## 📚 Documentation

For more detailed information, refer to:
- [Wiki](https://github.com/banzoxOG/bypass/wiki)
- [Issues](https://github.com/banzoxOG/bypass/issues)
- [Discussions](https://github.com/banzoxOG/bypass/discussions)

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/YourFeature`)
3. Commit your changes (`git commit -m 'Add YourFeature'`)
4. Push to the branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

### Code Style

- Follow C# naming conventions
- Add comments for complex logic
- Update README with new features

---

## ⚠️ Disclaimer

This tool is provided as-is for educational and authorized use only. Users are responsible for ensuring compliance with local laws and regulations. Misuse of this tool may violate terms of service or legal agreements.

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**banzoxOG** - GitHub Repository Owner

- GitHub: [@banzoxOG](https://github.com/banzoxOG)
- Repository: [bypass](https://github.com/banzoxOG/bypass)

---

## 🐛 Reporting Issues

Found a bug? Have a suggestion? Please open an [Issue](https://github.com/banzoxOG/bypass/issues) on GitHub with:

- Clear description of the problem
- Steps to reproduce
- Your system information (Windows version, .NET version, etc.)
- Debug output (if applicable)

---

## 📞 Support

For support and questions:
- Check [Existing Issues](https://github.com/banzoxOG/bypass/issues)
- Review [Discussions](https://github.com/banzoxOG/bypass/discussions)
- Open a new issue with your question

---

**Last Updated:** May 2026
**Version:** 1.0.0

---

*For the latest updates and releases, visit the [GitHub Repository](https://github.com/banzoxOG/bypass)*
