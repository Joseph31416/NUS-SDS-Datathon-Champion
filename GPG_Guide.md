
# GPG Installation and Decryption Guide

## For Windows

### Installing GPG:

1. **Download Gpg4win**: Visit [Gpg4win's official website](https://www.gpg4win.org/) and download the latest version.
2. **Run the Installer**: Open the downloaded file and follow the installation instructions. Select the components you wish to install (default selection is usually sufficient for most users).
3. **Complete the Installation**: Proceed with the installation and complete it.

### Decrypting a File:

1. **Download File**: Go to the kaggle link sent in the telgram channel, and download the file. 
2. **Decrypt the File**:
   Click on file to open it. The Kleopatra app (comes installed in default Gpg4win set-up) should open automatically and prompt for passphrase. Enter the passphrase sent in your email.
3. Store the decrypted data file in the `data` folder in your local copy of the template repo.

## For macOS

### Installing GPG:

1. **Download GPG Suite**: Visit [GPGTools website](https://gpgtools.org/) and download GPG Suite for macOS.
2. **Install GPG Suite**: Open the downloaded `.dmg` file and follow the installation instructions.

### Decrypting a File:

1. **Download File**: Go to the kaggle link sent in the telgram channel, and download the file. 
2. **Open Terminal**: You can find it in Applications > Utilities > Terminal.
3. **Navigate to the File's Directory**:
   ```bash
   cd path/to/file/directory
   ```
4. **Decrypt the File**:
   ```bash
   gpg --decrypt catA_train.csv.gpg
   ## OR
   gpg --decrypt catB_train.parquet.gpg
> outputfile
   ```
   Enter the passphrase sent in your email.
5. Store the data in the `data` folder in your local copy of the template repo.

## For Linux

### Installing GPG:

GPG is usually pre-installed on most Linux distributions. If it's not, you can install it using the package manager.

For Ubuntu/Debian-based systems:
```bash
sudo apt-get install gnupg
```

For Fedora/RHEL-based systems:
```bash
sudo yum install gnupg
```

For Arch Linux:
```bash
sudo pacman -S gnupg
```

### Decrypting a File:

1. **Download File**: Go to the kaggle link sent in the telgram channel, and download the file. 
2. **Open Terminal**.
3. **Navigate to the File's Directory**:
   ```bash
   cd path/to/file/directory
   ```
4. **Decrypt the File**:
   ```bash
   gpg --decrypt catA_train.csv.gpg
   ## OR
   gpg --decrypt catB_train.parquet.gpg 
   ```
   Enter the passphrase sent in your email. 
5. Store the data in the `data` folder in your local copy of the template repo.
