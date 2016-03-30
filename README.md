# Modem: Secrets

> Encrypted passwords, key files, and more for internal use

This repository contains various encrypted files with credentials for accessing the accounts and servers that are responsible for the technical aspects of Modem. Files are transparently encrypted using [git-crypt](https://github.com/AGWA/git-crypt) and can only be decrypted using the `radio-modem/secrets.key` file found in Google Drive. This allows us to keep credentials secure and versioned whilst still keeping everything out in the open which, luckily, is entirely free. We're a university radio after all; free is good!
