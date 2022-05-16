---
layout: post
category: story
title: Generating full GPG keypairs
description: Generate your full keypair using GPG
tags: guides
image: 
---

## Motivation

Keypairs (public key + private key) essentially act as identities. Having your own keypair enables you to digitally sign, encrypt and decrypt files and messages.

## Assumptions

- `gnupg`[^1] is installed on your system

## Create new keypair

In your terminal:

- `gpg --full-generate-key`
*(generates a new GPG keypair)*

Follow the prompts:

1. **(1) RSA AND RSA** (type of key)
2. **4096** (keysize in bits)
3. **2y** (expiry date)
4. **y** (confirmation)

Choose whatever you want, but I suggest you get a 4096-bit RSA/RSA key.

You can skip *Comment* field and enter an email address to be associated with your keypair.

Enter a strong passphrase to protect your secret key. This is important, do not skip this step. In case someone steals your secret key, this passphrase is the only thing that protects that file. Securely store the passphrase.

After a few seconds (sometimes 1-2 minutes), the keypair should be generated. 

GPG should've also created a revocation certificate for this keypair:

> gpg: revocation certificate stored as '/home/user/.gnupg/openpgp-revocs.d/01234567890.rev'

You will need that certificate to tell others to ignore the keypair, if it ever gets lost or compromised.
It might be a good idea to store that separately.

## Export public key

- `gpg -k`
*(lists all keypairs in your keyring)*

Find your key's ID, fingerprint or email address. You can use any of those to specify from which keypair to export.

I will use my email as an example:

- `gpg --export -a escapethe3ra@ctemplar.com > 3RA_pubkey.asc`
*(exports the public key for the user with that email address to the file named 3RA_pubkey.asc)*

*Note: use your own email, key id or fingerprint; and feel free to change the file name above.*

That's all. Now share your public key file with anyone you wish to communicate with.

Keep safe:

- secret key file
- secret key passphrase
- revocation certificate

## Going deeper

There are other things you can do for extra security but the complexity grows with each step. Maybe I will touch on some of those topics in future guides.

I suggest you take a look at subkeys[^2] or explore my cleartext digital signatures guide[^3].

---

[^1]: https://www.gnupg.org/download/
[^2]: https://wiki.debian.org/Subkeys
[^3]: [/gpg-cleartext-signatures](/gpg-cleartext-signatures)
