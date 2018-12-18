# Recovery Phrase and Wallet Backup

The normal process of creating a City Hub wallet, involves writing down the Recovery Phrase. This is a 12-word sentence, and an optional Extension Word.

It is very important that you keep a backup of both the **Recovery Phrase** and the **Extension Word**. You cannot restore your wallet in the future, if you forget your **Extension Word**. You can leave the Extension Word empty.

At the end of wallet creation, you enter your personal password. This is validated and entered twice. The password is used to safely store your private key on your computer.

If you restore your wallet in the future on a different (or same) computer, you can select a different password.

## Wallet Backup

Note: Before you take backup of wallet, and before your restore a wallet backup, you should exit City Hub (or City Chain daemon).

If you loose your Recovery Phrase, or did not take a backup when creating your wallet, you can still take a backup of your wallet file. This wallet file can be moved to a different computer.

Remember that this file is only as secure as your password. If you use a very simple password, your wallet file is not very safe if anyone gain physical access to your computer and/or your wallet file.

If you have very few characters in your password, your wallet file can easily be exposed with brute-force attack.

Wallet files for the City Chain main network is located in the AppData folder on your computer. This is different on Windows, Linux and Mac. 

**TODO**: Add examples for Linux and Mac.

```
%APPDATA%\CityChain\city\CityMain\
```

If the path above is opened in Windows Explorer, you should automatically navigate to a path similar to the example below:

```
C:\Users\YourName\AppData\Roaming\CityChain\city\CityMain\
```

Located in this folder, you will see a few files.

All files named SOMETHING.wallet.json, are your wallet files.

Example:

```
main.wallet.json
```

This is the file that is important to take backup of, if you do not have your Recovery Phrase and Extension Word.

To recover your wallet file on a different computer, simply copy the wallet file to the same location on your other computer. Exit City Hub before restore the wallet file.

## Encrypted Disks

We suggest you always rely on encrypted disk storage, if available for your computer. Using encrypted disks, ensures that nobody in the future which recycles your computer, or steals your computer, can read old files that was written on your disk.

It is also possible to encrypt USB harddrives connected to your computer. These can be good option for backup of various files in a secure manner.
