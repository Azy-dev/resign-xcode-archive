resign-xcode-archive
====================

Bash script to resign xcode archive with new signing identity and provision profile

Parameters passed into a script:
 1. Path to Archive folder
 2. Path to Provision profile
 3. SHA1 fingerprint of certificate you want to sign with. You can find it in certificate details, or run from command-line 
``security find-certificate -c 'iPhone Distribution' -a -Z`` and get SHA-1 hash: value
 4. Certificate name (Common name in certificate details)

Example:
```bash
/path-to-resign/resign-archive '/path-to-archive/My_App 01.01.13, 12.48.xcarchive' ~/Library/MobileDevice/"Provisioning Profiles/F569DD54-6512-4F34-80D8-1AE10FF95EC6.mobileprovision" 086418E906CEE89C2353B6E27FBD9E7439F76316 "iPhone Distribution: My Company (1RFW75TKL3)"
```
