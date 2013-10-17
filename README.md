resign-xcode-archive
====================

Bash script to resign xcode archive with new signing identity and provision profile

Parameters passed into a script:
1. Path to Archive folder.
2. Path to Provision profile.
3. SHA1 fingerprint of certificate you want to sign with. You can find it in certificate details, or run from command-line 
``security find-certificate -c 'iPhone Distribution' -a -Z`` and get SHA-1 hash: value.
4. Certificate name (Common name in certificate details).
