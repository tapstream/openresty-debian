# openresty-debian
Builds a deb package for OpenResty 1.9.3.1 w/ ssl-cert-by-lua branch of lua-nginx-module

##Notes

* All files go in the standard debian nginx locations
* Includes init, logrotate, and post/pre install/remove scripts from the official nginx package.
* Builds for Ubuntu Trusty by default.
* LuaJIT upgraded to 2.1 Beta 1 from 2.1 Alpha
* Includes a bundled copy of LuaRocks 2.2.2
* Statically linked against OpenSSL 1.0.2d, PCRE 8.3.7, ZLib 1.2.8
* Uses the ssl-cert-by-lua branch of lua-nginx-module


##Usage

Run ```./build``` from the project root. When it completes you'll have a deb in ```./artifacts```.
Note that you'll need to have a functional docker installation.
