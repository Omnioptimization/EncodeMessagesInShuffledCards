# EncodeMessagesInShuffledCards
Rearranges a deck of cards to hide a secret message.

Created by:
Dan Burke
2/20/2026


ENCODE FUNCTION
Encodes a secret message into an array by rearranging its elements.

DECODE FUNCTION
Decodes the secret message from the rearranged array.


Inspired by the following article
https://pagedout.institute/
https://pagedout.institute/download/PagedOut_008.pdf
"Bits per deck:
encoding messages
using playing cards"


//
// example use

let charSet = [" ", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z", ".", ",", "?", "!", "'"];

let deck = ["Ah", "Ad", "Ac", "As", "2h", "2d", "2c", "2s", "3h", "3d", "3c", "3s", "4h", "4d", "4c", "4s", "5h", "5d", "5c", "5s", "6h", "6d", "6c", "6s", "7h", "7d", "7c", "7s", "8h", "8d", "8c", "8s", "9h", "9d", "9c", "9s", "10h", "10d", "10c", "10s", "Jh", "Jd", "Jc", "Js", "Qh", "Qd", "Qc", "Qs", "Kh", "Kd", "Kc", "Ks"];

let secretMessage = "secret message decoded, it's just crazy huh?";

let encoded = encodeMessageToDeck(charSet, deck, secretMessage);
console.log(encoded);

let decoded = decodeMessageFromDeck(charSet, encoded, deck);
console.log(decoded);
