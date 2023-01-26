# mathPacket_client
Short code sample: socket programming in C.

Important references:
===========================================================================

1. Client Request format:

Command MATH/Version\n
[Operand1 : X\n]
Operator: Y\n
Operand2: Z\n
Connection: [Close|Keep-Alive]\n\n

===========================================================================

2. Example run and correct, parsed response:

you@linux# mathPacket_client 127.0.0.1 8080 9 / 4 + 1 - 9 x 7

Response Code: 100 OK
Result: -42
Rounded!
No Overflow
X-Server-Version
