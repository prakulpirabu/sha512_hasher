# sha512_hasher
from hashlib import sha512

file_name = input("> ")
with open(file_name, "rb") as f:
    my_hash = sha512(f.read())
    print(my_hash.hexdigest())
