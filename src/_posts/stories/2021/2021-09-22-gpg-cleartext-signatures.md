---
layout: post
category: story
title: Digitally signing contact information with GPG
description: Digitally signing contact information with GPG
tags: guides
image: 
---

## Motivation

By signing a file containing your non-confidential contact info (ie. email, social handles, XMR addresses), you are essentially allowing people to verify that the public details haven't been tampered with and they come from you.

## Assumptions

- `gnupg`[^1] is installed on your system
- you already own a keypair[^2]

## Signing

We're going with a clear text type of signature in this guide.

Fire up a terminal and type in:

- `nano contact.txt`
*(creates the file and opens it in a text editor)*

Enter your contact details that you want to publish on your site. Save and exit the editor.

- `gpg --clear-sign -o contact-signed.txt contact.txt`
*(signs the file with your main public key)*

Enter your key password when prompted. 

*Note: you can also use a different keypair to sign the file by using the `--local-user` flag.*

You should now have a `contact-signed.txt` file in the same directory.

- `cat contact-signed.txt`
*(lists file contents, signed)*

This should output something like this, only with your own content:

```
-----BEGIN PGP SIGNED MESSAGE-----
Hash: SHA512

Email: escapethe3ra@ctemplar.com
Key Fingerprint: BCE1 5F74 D181 1282 4899  608A FD10 3120 DC7B CC36
Reddit: escapethe3ra
Matrix: escapethe3ra@matrix.org
-----BEGIN PGP SIGNATURE-----

iQKuBAEBCgCYFiEEvOFfdNGBEoJImWCK/RAxINx7zDYFAmFLogNfFIAAAAAALgAo
aXNzdWVyLWZwckBub3RhdGlvbnMub3BlbnBncC5maWZ0aGhvcnNlbWFuLm5ldEJD
RTE1Rjc0RDE4MTEyODI0ODk5NjA4QUZEMTAzMTIwREM3QkNDMzYaHGVzY2FwZXRo
ZTNyYUBjdGVtcGxhci5jb20ACgkQ/RAxINx7zDb6Xw//dSR6MRxxjSJO5agmvSSt
RGkduH/KXRRfvsWFZh5ETgSUmnCeg2GoXKUPE4ZGCHHk3ZsMsB89F529WOeT8+5H
ELG507/WPVh0MFdbLfctCt/IBNyBItbQ4P8UR6l6KLLEu35AkCIRq5E6G/XCwkKK
JEXFodCvGHA6SyMOtT2MHnlvmQzvuhFQVys7SMnPmsyZlayXa88M+Q3kKO5mwoMi
keT+mqbTEM/x80cxrd81/r2VT/aMM4fpuZSGzY70p7JCypBCDpLgjdFFhGztwiHa
SF6h2mMmYn8JInrr5LByunK9PLPXjx0F6f0/ym4Wts/IBDOEA+g5pwWElITVSYWt
BXjQL/pTGlKGl3YT5GTlxZgW/9zqaifQquFMWaZ36IZ/e/IWNcVTBbk1OZKhBiHP
7rbvAon3/z53mdUFB7EhDo3yScRvnhqUFvvDxXMw0ck4P7NcBowFFPDbrVDRFUhs
//kbQSG1siKVrqJ0U6rOCounjZXfEJbMsMvp4d1ERO92gHrrHcWfbwOrLc3DFK/i
cD7i8LsqKH4KWI6FsVddr9XsNmH9BUoI3fLN1a5CQsFJs2nTFPH80zq2Cb8sZMg6
WVb/iPk2PqsbGdvl+nXsBVRefmdNOjFCzDduWUggBocnqqplDbMo3DIdVWcAxDNr
SMvCKV9o+/vZ4SbRe3oeo+8=
=etlF
-----END PGP SIGNATURE-----
```

Now you can publish the file online. Don't forget to also include your public key that you used to sign this file. That way people can use it to verify your contact details.

## Verifying

You can exercise by trying to verify my information. This way you can see how the process works for the other party.

If you don't already have my public key, download it. Then verify the fingerprint and import it.

*Note: on Whonix you can replace `wget` with `scurl` for better security.[^3]*

- `wget https://monero.observer/3RA_pubkey.asc`
*(downloads my public key to your machine)*

- `gpg --show-keys 3RA_pubkey.asc`
*(list the key's fingerprint)*

The output should match this fingerprint:

> BCE15F74D18112824899608AFD103120DC7BCC36

If it doesn't, don't import it. Delete and try again or contact me.

- `gpg --import 3RA_pubkey.asc`
*(imports the key)*

Download the file containing my signed contact info:

- `wget https://monero.observer/contact-signed.txt`
*(downloads my signed contact info to your machine)*

- `gpg --verify contact-signed.txt`
*(verifies if the file contains the original content)*

```
gpg: Signature made Wed 22 Sep 2021 09:37:07 PM UTC
gpg:                using RSA key BCE15F74D18112824899608AFD103120DC7BCC36
gpg:                issuer "escapethe3ra@ctemplar.com"
gpg: Good signature from "escapethe3RA <escapethe3ra@ctemplar.com>" [unknown]
```

You can ignore this warning:

```
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: BCE1 5F74 D181 1282 4899  608A FD10 3120 DC7B CC36
```

The most important part of the output is this:

```
gpg: Good signature from "escapethe3RA <escapethe3ra@ctemplar.com>"
```

That's what you want to see. 

If you see `BAD signature` then the file is probably corrupted, not original, or there was a mistake somewhere in the steps above. You can delete it and try again.

If all went well, you can try and change something inside my `contact-signed.txt` file, save it and verify it again. It should fail, even if all you've modified is 1 single character.

## Notes

- signing a file does not automatically encrypt its contents
- this is not the only way to digitally sign[^4] a file; the manual suggests using detached signatures over cleartext[^5]
- `gpg --verify` does not check for any modifications outside of the cleartext signature or the header lines directly following the dash marker line
- GPG usage might not fit your threat model

## Feedback

After getting lots of PGP-related questions, I decided it might be helpful to start making some guides, and see if people find them useful. 

There's also a second guide[^2] available. Let me know if you want to see more. 

Feedback is always welcome!

**-3RA**

---

[^1]: https://www.gnupg.org/download/
[^2]: [/gpg-generate-full-keypair](/gpg-generate-full-keypair)
[^3]: http://www.dds6qkxpwdeubwucdiaord2xgbbeyds25rbsgr73tbfpqpt4a6vjwsyd.onion/wiki/Secure_Downloads
[^4]: https://www.gnupg.org/gph/en/manual/x135.html
[^5]: https://www.gnupg.org/documentation/manuals/gnupg/Operational-GPG-Commands.html
