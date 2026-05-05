# RSA

Aim: To perform encryption and decryption using RSA (Rivert-Shamir-Adleman) Algorithm.
Course Outcome: To build cryptosystems by applying asymmetric key cryptographic
algorithms.
Theory:
RSA(Rivest-Shamir-Adleman) Algorithm is an asymmetric or public-key cryptography
algorithm which means it works on two different keys: Public Key and Private Key. The Public
Key is used for encryption and is known to everyone, while the Private Key is used for
decryption and must be kept secret by the receiver. RSA Algorithm is named after Ron Rivest,
Adi Shamir and Leonard Adleman, who published the algorithm in 1977.
Procedure:
1. Select Two Prime Numbers
Choose two distinct prime numbers p and q.
2. Compute the Modulus (n)
Multiply the two prime numbers:
3. Calculate Euler’s Totient Function (φ(n))
ϕ(n)=(p−1)(q−1)\phi(n) = (p - 1)(q - 1)ϕ(n)=(p−1)(q−1) ϕ(n)=(17−1)(11−1)\phi(n) =
(17 - 1)(11 - 1)ϕ(n)=(17−1)(11−1) ϕ(n)=16×10=160\phi(n) = 16 \times 10 =
160ϕ(n)=16×10=160
4. Choose the Public Key Exponent (e)
Select a number e such that:
○ 1&lt;e&lt;ϕ(n)1 &lt; e &lt; \phi(n)1&lt;e&lt;ϕ(n)
○ gcd(e, ϕ(n)\phi(n)ϕ(n)) = 1
5. Choose:
e=7 &amp; Verify:
gcd(7, 160) = 1 → Condition satisfied
Public Key = (7, 187)
6. Determine the Private Key Exponent (d)
d×e≡1(modϕ(n))
🔒 2. Encryption Formula

If message = M

C=M
e
modn

Where:

C = ciphertext
🔓 3. Decryption Formula
M=C
d
modn
187C=887mod187 C=11C = 11C=11
Ciphertext obtained = 11
9. (Optional) Verify by Decryption
Use the decryption formula:
M=Cdmod  nM = C^d \mod nM=Cdmodn M=1123mod  187M = 11^{23} \mod
187M=1123mod187 M=88M = 88M=88
