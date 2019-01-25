# Rail-Fence-Cipher-Java
Introduction 
The railfence cipher is a very simple, easy to crack cipher. It is a transposition cipher that follows a simple rule for mixing up the characters in the plaintext to form the ciphertext. The railfence cipher offers essentially no communication security, and it will be shown that it can be easily broken even by hand.

Although weak on its own, it can be combined with other ciphers, such as a substitution cipher, the combination of which is more difficult to break than either cipher on it's own.

Many websites claim that the rail-fence cipher is a simpler "write down the columns, read along the rows" cipher. This is equivalent to using an un-keyed columnar transposition cipher.


Example 
The key for the railfence cipher is just the number of rails. To encrypt a piece of text, e.g.

defend the east wall of the castle

We write it out in a special way on a number of rails (the key here is 3)

d . . . n . . . e . . . t . . . l . . . h . . . s . . .
. e . e . d . h . e . s . w . l . o . t . e . a . t . e
. . f . . . t . . . a . . . a . . . f . . . c . . . l .
The ciphertext is read off along the rows:  dnetlhseedheswloteateftaafcl

ENCRYPTION:
In the rail fence cipher, the plain-text is written downwards and diagonally on successive rails of an imaginary fence.
When we reach the bottom rail, we traverse upwards moving diagonally, after reaching the top rail, the direction is changed again. Thus the alphabets of the message are written in a zig-zag manner.
After each alphabet has been written, the individual rows are are combined to obtain the cipher-text.

DECRYPTION:
The number of columns in rail fence cipher remains equal to the length of plain-text message. And the key corresponds to the number of rails.
Hence, rail matrix can be constructed accordingly. Once we’ve got the matrix we can figure-out the spots where texts should be placed (using the same way of moving diagonally up and down alternatively ).
Then, we fill the cipher-text row wise. After filling it, we traverse the matrix in zig-zag manner to obtain the original text.
