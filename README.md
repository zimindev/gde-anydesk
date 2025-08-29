## 🖥️ AnyDesk Setup Guide

### ✅ What is AnyDesk?

**AnyDesk** is a fast, lightweight, and secure remote desktop application. It allows you to connect to remote computers, provide support, or access your own machines from anywhere. AnyDesk supports multiple platforms including Linux, Windows, macOS, Android, and iOS.

---

### 🖥️ Step 1: Install AnyDesk

#### Arch Linux (using yay):

```bash
yay -S anydesk-bin
````

This will download and install the latest AnyDesk binary from the AUR.

#### Debian/Ubuntu:

1. Add the AnyDesk repository:

```bash
wget -qO - https://keys.anydesk.com/repos/DEB-GPG-KEY | sudo apt-key add -
echo "deb http://deb.anydesk.com/ all main" | sudo tee /etc/apt/sources.list.d/anydesk.list
```

2. Update and install:

```bash
sudo apt update
sudo apt install anydesk
```

#### Fedora:

```bash
sudo dnf config-manager --add-repo https://rpm.anydesk.com/fedora/anydesk.repo
sudo dnf install anydesk
```

#### Windows:

Download the installer from the [official website](https://anydesk.com/en/downloads/windows) and run the `.exe` file.

#### macOS:

Download the `.dmg` from [AnyDesk macOS](https://anydesk.com/en/downloads/mac-os) and drag it to your Applications folder.

---

### ⚙️ Step 2: Launch AnyDesk

Open AnyDesk from your applications menu or run:

```bash
anydesk
```

On first launch, AnyDesk will generate your **AnyDesk Address**, which you can share to allow remote connections.

---

### 🔧 Step 3: Configure Permissions (Linux)

On Linux, ensure AnyDesk has the required permissions for:

* Screen recording/sharing
* Clipboard access
* Audio transmission (optional)

For example, on GNOME or KDE, you may need to grant permissions via system settings.

---

### 🛡️ Step 4: Security Tips

* Always verify the AnyDesk ID before granting access.
* Enable **Interactive Access** for better control.
* Use strong passwords for unattended access.
* Keep AnyDesk updated to the latest version for security patches.

---

### 🚀 Step 5: Optional: Start AnyDesk at Boot

#### Systemd (Linux):

```bash
sudo systemctl enable anydesk.service
sudo systemctl start anydesk.service
```

This ensures AnyDesk runs in the background and is ready for remote connections after system startup.

---

### 📚 Additional Resources

* Official Website: [https://anydesk.com](https://anydesk.com)
* Arch Wiki: [AnyDesk](https://wiki.archlinux.org/title/AnyDesk)
* Man page: `man anydesk`

```
