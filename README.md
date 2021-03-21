=====================
# Cryptography_Python
=====================

* __Author__ __Lencof__

# Welcome to Lencof/Cryptography_Python

``cryptography`` includes both high level recipes and low level interfaces to common cryptographic algorithms such as symmetric ciphers, 
message digests, and key derivation functions. For example, to encrypt something with ``cryptography``’s high level symmetric encryption recipe:

from cryptography.fernet import Fernet
Put this somewhere safe!
key = Fernet.generate_key()
f = Fernet(key)
token = f.encrypt(b"A really secret message. Not for prying eyes.")
token
b'...'
f.decrypt(token)
b'A really secret message. Not for prying eyes.'
