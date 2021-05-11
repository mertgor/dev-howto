# SSH and GPG how to 

* [How to Generate SSH Key document by GitHub](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

* [How to Generate GPG Key document by Github](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-gpg-key)

* [GPG Signed Commit document by GitHub](https://docs.github.com/en/github/authenticating-to-github/signing-commits)

## Some tips for your GPG key

* You may learn your Key ID by running this command : 
  * `gpg --list-secret-keys --keyid-format LONG`

* You may export your secret key to external hard disk by running this command :
  * `gpg --output secret.key --export-secret-keys yourkeyfingerprint`
* You may export your revocation certificate by running this command : 
 `gpg --output revoke.asc --gen-revoke mykey`

* Then export your public key by running this command :
  * `gpg --armor --export keyid > publickey.asc`

4. Then publish to PGP Global Directory , import key , trust and sign
