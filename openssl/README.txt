How to build Openssl
=====================

We need to build this library only for windows.

Instructions

- Download openssl-1.0.0d (http://www.openssl.org/source/)
- Decompress it openssl-XXX.tar.gz

WIN

cd openssl-1.0.0d
perl configure VC-WIN32 no-asm
ms\do_ms
nmake -f ms\ntdll.mak



###add those env variables
### %CD% should be expanded here
OPEN_SSL_HOME = %CD%\openssl-1.0.0d
include=%OPEN_SSL_HOME%\inc32
lib=%OPEN_SSL_HOME%\out32
path=%OPEN_SSL_HOME%\out32
