# Xoodoo-fork
https://ecc2017.cs.ru.nl/slides/ecc2017-daemen.pdf

Xoodoo is a cryptographic permutation function designed by the Keccak team

Xoodoo is a cryptographic permutation function designed by the Keccak team along with Seth Hoffert and Johan De Meulder. 
It was described by Joan Daemen at the 2017 Workshop on Elliptic Curve Cryptography in a talk: 
Innovations in permutation-based crypto 

The design is very similar to the Keccak permutation function, but obviously draws inspiration from 
the design of Gimli that also uses a 384-bit state, and works efficiently on many platforms. 

The C code shown here is derived from a python implementation. The Keccak team have posted their own implementations here
with further documentation in the Xoodoo cookbook.

Xoodoo with 12 rounds and a 384-bit state is much more compact than Keccak with 22 rounds and an 800-bit state. 
Presumably Keccak is more secure, but cannot be vectorized and perform as well as Xoodoo or Gimli. 
Sources:
https://github.com/odzhan/tinycrypt/tree/master/permutation/xoodoo

Xoodoo is used in Xoodyak
https://keccak.team/xoodyak.html
