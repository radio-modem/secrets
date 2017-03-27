# Modem: Secrets

> Encrypted passwords, key files, and more for internal use

This repository contains various encrypted files with credentials for accessing the accounts and servers that are responsible for the technical aspects of Modem. Files are transparently encrypted using [git-crypt](https://github.com/AGWA/git-crypt) and can only be decrypted using the [`radio-modem/secrets.key`](https://drive.google.com/open?id=0B_EA-Me3eCqGVUdYWm1FTElxR28) file found in Google Drive. This allows us to keep credentials secure and versioned whilst still keeping everything out in the open which, luckily, is entirely free. We're a university radio after all; free is good!

## Requirements

* [git-crypt](https://github.com/AGWA/git-crypt)

For the folks on macOS:

```console
$ brew install git-crypt
```

## Running

Grab the secret key from Google Drive and do:

```console
$ git-crypt unlock <path/to/secret.key>
```

That's it! All the files ending in `.enc` can now be read as plain text and will automatically be encrypted when committed to git.

---

Copyright &copy; 2016-2017 Modem. All rights reserved.
