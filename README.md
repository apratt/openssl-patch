# openssl-patch for the installation of Ruby 1.9.3 with rbenv

Because of OpenSSL incompatibility in Debian (7.5 and above), Ruby might fail to compile without patching it first:

Apply with:

cat openssl.patch | rbenv install -v --patch 1.9.3-p551
