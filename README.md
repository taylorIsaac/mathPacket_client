# mathPacket_client
Short code sample: socket programming in C.

Important references:
===========================================================================

1. Client Request format:

Command MATH/Version
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
![example_run](https://user-images.githubusercontent.com/103297296/214791073-ffc5d6b1-3477-4280-8ce2-00033fc73f18.png)
