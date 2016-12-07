# WinCom
Secure Windows Multi-Threaded Asynchronous Socket Library

# Brief Info
This library will wrap around what would be standard socket connections in windows (winsock) and add a more modern, secure structure.
## Notice 
This library was developed in just a few days, and isn't meant to be implemented as-is in any serious environment (especially an enterprise one). It's mainly proof-of-concept code.

# Notable Features
1. Support for multiple user defined callback routines. 
2. Theoretically could be used to support quite a few clients (especially if you modify the client/server initial connection protocols)
3. Made with performance, stability, security, and scalability in mind
4. Custom exception handling
5. Infrastructure scalability factors mostly accounted for
6. Implementation of Microsoft's Schannel API provides a secure channel via SSL/TLS protocol(s)
7. Schannel implementation includes data singing and verification routines built into the default connection/data handlers
8. Includes support for the general Microsoft CryptoAPI with a few included examples:
  * Public/Private key cryptography sessions (RSA-2048bit, perfect forward secrecy)
  * Data encryption using a strong block cipher with derived keys (AES-256bit)
  
  Other examples include:
  * Basic chatroom application (GUI built in C#)
  * Extension of the chatroom application, now utilizing Microsoft Schannel API (SSL/TLS with data verification) and supporting FTP between users.
  * Secure server/client data storage application (using RSA-2048bit public/private keys to transfer client data encrypted with a AES-256bit derived key)
  
 # General Design
 
 # Implementation
 
