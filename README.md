This project is to aggregate issues in any open source projects that still use obsolete and deprecated SHA1 and weaker algorithms. These include removal of:

* SHA2-224 (not strong enough in 2030+)
* SHA1-128 (obsolete, prohibited in 2030+)
* DES
* DSA
* MD5 (should be dead)
* MD4
* MD2
* WHIRLPOOL
* RIPEMD160

Depending on usecases one should upgrade to any modern alternatives.

* For cryptographic hash function capability upgrade to [SHA2-256](https://en.wikipedia.org/wiki/Template:Comparison_of_SHA_functions)
* For non-cryptographic fast hash function upgrade to [xxhash](https://xxhash.com/)
* For key derivation function use [Argon2](https://en.wikipedia.org/wiki/Argon2)
* For password hashing use [Yescrypt](https://www.openwall.com/yescrypt/)

If you want to sponsor me working on this more, please consider dontating at https://github.com/sponsors/xnox

Source code created to port software away from SHA1 is generally released under permissive license, or not even copyrightable due to being trivial in its nature, or actually simply deleting existing code.
