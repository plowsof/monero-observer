---
layout: post
category: story
title: Guide to verifying, running and updating the official Monero CLI wallet on Linux
description: "Step by step guide to verifying, running and updating the official Monero CLI wallet on Linux."
tags: guides
image: 
---

## Motivation

- Why Linux/CLI

Linux is the most empowering OS for users. The CLI is the most empowering wallet for users. Transitioning from GUIs to the command line doesn't have to be complicated.

- Why Verify/Update

Most users skip software verification. Blindly installing software is not secure and can lead to loss of funds and privacy. Running up-to-date verified software means less bugs, new features and more peace of mind.

## Assumptions

- you want to run (install) / update the official Monero CLI wallet 
- you are on a Linux machine (ie. Debian)

## Step 1: Verify software (important)

Before downloading and running the latest Monero CLI binaries from Github[^1] or Getmonero.org[^2], we need to first determine if the software is safe to use.

Open up a terminal.

### Step 1.1: Verify and import signing key

Fetch *binaryFate*'s signing key[^3] from Github:

`wget -O binaryfate.asc https://raw.githubusercontent.com/monero-project/monero/master/utils/gpg_keys/binaryfate.asc`

Display the key's fingerprint:

`gpg --keyid-format long --with-fingerprint binaryfate.asc`

The output should look like this:

```
pub   rsa4096/F0AF4D462A0BDF92 2019-12-12 [SCEA]
      Key fingerprint = 81AC 591F E9C4 B65C 5806  AFC3 F0AF 4D46 2A0B DF92
uid                           binaryFate <binaryfate@getmonero.org>
```

Proceed to the next step **only if the key fingerprint matches exactly** with the above (81AC 591F E9C4 B65C 5806  AFC3 F0AF 4D46 2A0B DF92).

**Do not proceed if the key fingerprint does not match exactly** with the above. Delete the file and try downloading it again.

Import the key:

`gpg --import binaryfate.asc`

Output should contain the following if this is the first time you have imported this key:

```
gpg: Total number processed: 1
gpg:               imported: 1
```

### Step 1.2: Download and verify hashes file

Download the signed hashes file from Getmonero.org:

`wget -O hashes.txt https://www.getmonero.org/downloads/hashes.txt`

Verify the signature of the file:

`gpg --verify hashes.txt`

If the file is authentic (file is signed with binaryFate's key), output should be:

```
gpg:                using RSA key 81AC591FE9C4B65C5806AFC3F0AF4D462A0BDF92
gpg: Good signature from "binaryFate <binaryfate@getmonero.org>" [unknown]
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: 81AC 591F E9C4 B65C 5806  AFC3 F0AF 4D46 2A0B DF92
```

Only proceed if you see **Good signature** in your output.

If you see **BAD signature**, delete the `hashes.txt` file and download it again.

### Step 1.3: Download and verify binaries

Download the CLI binary. Do **not** extract the archive yet.

`wget -O monero-linux-x64-v0.17.3.0.tar.bz2 http://dlmonerotqz47bjuthtko2k7ik2ths4w2rmboddyxw4tz4adebsmijid.onion/cli/linux64`

Display the `SHA256` hash of your download:

`shasum -a 256 monero-linux-x64-v0.17.3.0.tar.bz2`

The output should **match** the hash for your binary in the `hashes.txt`[^4] file:

`ac18ce3d1189410a5c175984827d5d601974733303411f6142296d647f6582ce  monero-linux-x64-v0.17.3.0.tar.bz2`

#### Notes

- If the latest version is not v0.17.3.0, substitute that above.

- If you have downloaded a different binary, substitute that above.

If hashes match, proceed.

**If hashes do not match, stop**. Delete the binary and try downloading it again.

## Step 2: Extract binaries

Extract the binaries to a new directory of your liking:

`tar -xvf monero-linux-x64-v0.17.3.0.tar.bz2 -C /home/user/monero`

#### Notes

- Substitute the directory `/home/user/monero` to your preferred destination folder.

- Substitute `monero-linux-x64-v0.17.3.0.tar.bz2` with your own binary.

## Step 3: Updating wallets

To update to the latest version (ie. from v0.17.2.3 to v0.17.3.0), just copy over the wallet files (ie. `mywallet` and `mywallet.keys`) from the old folder (containing v0.17.2.3) to the new folder (containing v0.17.3.0).

Start the wallet. A blockchain resync is not needed.

## Feedback & Questions

If you have any issues following this guide, let me know. I will try to help you if I can. You can also get in touch with the Monero community on Matrix/IRC[^5] and Stackexchange[^6].

Feedback is always appreciated @ [/about](/about).

**-3RA**

---

[^1]: https://github.com/monero-project/monero/releases/tag/latest
[^2]: https://getmonero.org/downloads
[^3]: https://raw.githubusercontent.com/monero-project/monero/master/utils/gpg_keys/binaryfate.asc
[^4]: https://getmonero.org/downloads/hashes.txt
[^5]: https://getmonero.org/community/workgroups/
[^6]: https://monero.stackexchange.com
