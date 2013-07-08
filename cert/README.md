# cant_wait ~ Gem Signature verification
[![Gem Version](https://badge.fury.io/rb/cant_wait.png)](https://badge.fury.io/rb/cant_wait)


All the versions of **cant_wait** released from rubygems.org have been digitally signed.

To verify that the gem has not been tampered with, I am providing here the self-signed certificate used, which includes the public key.

Therefore, you have now two pieces of information from two different sources:

- The signed gem from [rubygems.org](http://rubygems.org/gems/cant_wait)
- The certificate from [github.com's](https://github.com/CarlosCD/cant_wait) repository

Unfortunately this mechanism is not perfect, but I believe it is better than no security at all, until the Ruby community and RuybyGems.org agrees in something better.


## Cryptographic signature verification

To verify the gem's signature:

1. First install the certificate public_cert.pem downloaded from the cert folder of Github's repository (master branch):

        gem cert -a public_cert.pem

2. Then Download the last version of the gem (or a version you intend to use) from rubygems.org.  The file would look something like:

        cant_wait-X.Y.Z.gem

   Where <tt>X.Y.Z</tt> is the gem's version.

3. Next the gem can be installed with the high security option, which checks that the gem is signed and the signature matches an installed certificate:

        gem install cant_wait-X.Y.Z.gem -P HighSecurity

If the certificate or the gem has been tampered with, the gem command (RubyGems) should refuse to install it.


July 2013
