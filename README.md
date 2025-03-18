# DynamicArchive

DynamicArchive is designed to archive folders into compressed files with encryption features, as well as extract encrypted compressed files. This tool aims to simplify archive management while adding a layer of security through [symmetric encryption](https://ricaldocs.github.io/posts/gnu-privacy-guard/#asymmetric--symmetric). 🔒✨

## 📁 Supported Formats
- [Tar](https://id.wikipedia.org/wiki/Tar_(komputasi))
- [ZIP](https://id.wikipedia.org/wiki/ZIP_(format_berkas))
- [7-Zip](https://id.wikipedia.org/wiki/7-Zip)
- gz

## ✨ Features

1. Archive folders into encrypted files using [GnuPG](https://ricaldocs.github.io/posts/gnu-privacy-guard/). 📦🔒
2. Extract encrypted files. 📥🔒

## 🌟 Prerequisites

- Bash or Zsh

## 🚀 Usage

To run this tool, simply execute the following commands in your terminal:

```bash
git clone https://github.com/ricalnet/DynamicArchive.git && cd DynamicArchive
```

```bash
sudo ./requirements.sh
```

```bash
./dynamic_archive.sh
```

## 📋 Menu Options
Follow the on-screen instructions to choose your method of use. 

```
==================================================================
      DynamicArchive          
      https://github.com/ricalnet/DynamicArchive
==================================================================

========== TAR =========
1) Archive 📦🔒
2) Extract 📥🔒
========================

========== ZIP =========
3) Archive 📦🔒
4) Extract 📥🔒
========================

========== 7z ==========
5) Archive 📦🔒
6) Extract 📥🔒
========================

========== GZ ==========
7) Archive 📦🔒
8) Extract 📥🔒
========================

==================================================================
Enter your choice (1, 2, 3, 4, 5, 6, 7, or 8): 1
Enter the path of the folder you want to archive: /home/user/folder
```

### To Archive a Folder into an Encrypted File:
- Enter the path of the folder you want to archive (e.g., `/home/user/backup`).
- Enter the desired output file name (e.g., `backup.tar`).
- The script will create the file and encrypt it using [GnuPG](https://ricaldocs.github.io/posts/gnu-privacy-guard/), resulting in an output of `backup.tar.gpg`. 🎉

### To Extract an Encrypted File:
- Enter the name of the encrypted file (e.g., `backup.tar.gpg`).
- The script will decrypt and extract the file for you. 🔓

> **Note:** DynamicArchive will validate the output file name to ensure that only alphanumeric characters, dots, underscores, and hyphens are allowed. 

## 📜 License
This project is open-source and available under the [MIT License](https://github.com/ricalnet/DynamicArchive/blob/main/LICENSE.md).


