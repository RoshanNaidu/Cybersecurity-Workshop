# Cybersecurity-Workshop
The CyberSecurity workshop organized by the Linux Club (Cybersec101) provided me with hands-on experience with various tools and techniques in the field of cybersecurity. This Repo contains a detailed account of what I learned and achieved during the workshop.

# Topics:

## Exploring the JWT Toolkit
We began by exploring the powerful JWT toolkit, which is essential for handling JSON Web Tokens (JWTs) effectively. This toolkit allows for the creation, modification, and validation of JWTs, which are widely used for secure authentication.
![Screenshot 2024-07-08 at 7 15 07 PM](https://github.com/user-attachments/assets/3f073af2-3b65-4d6b-ace7-f5422f10700d)


## JWT.io Deep Dive
At JWT.io, I learned about the core components of JSON Web Tokens, including:
### Header: Contains metadata such as the signing algorithm (alg) and token type (typ).
### Payload: Contains the token's claims, such as subject (sub), name (name), and issued at (iat).
### Signature: Ensures the token's integrity and authenticity.
![Screenshot 2024-07-08 at 1 49 10 AM](https://github.com/user-attachments/assets/72e8fc49-91cb-4035-9f54-03090d92c45f)


## Magic Bytes
We explored the concept of Magic Bytes, which are unique sequences of bytes used to identify file formats. Understanding Magic Bytes is crucial for file format exploitation and forensics.

## PortSwigger and Burp Suite
Gained hands-on experience with Burp Suite from PortSwigger, a leading tool for web vulnerability scanning and penetration testing. Burp Suite is essential for identifying and exploiting web application vulnerabilities.

## Gobuster
Learned about Gobuster, a tool used for brute-forcing URIs (directories and files) in websites and DNS subdomains. Gobuster is a powerful tool for discovering hidden resources on a web server.

## HS256 and RSA
Delved into the HS256 (HMAC with SHA-256) and RSA algorithms, which are widely used for secure token signing and verification. Understanding these algorithms is crucial for implementing secure authentication mechanisms.

## Understanding JWT and JSON Web Tokens (JWS and JWE)
Explored the differences between JSON Web Signature (JWS) and JSON Web Encryption (JWE). JWS provides integrity and authenticity, while JWE ensures confidentiality through encryption.

## SQL Injections
Learned the intricacies of SQL injections and how to protect against them. Practiced bypassing admin logins using SQL injections with SQLmap, a powerful tool for automating SQL injection exploitation.

## robots.txt
Discussed the role of robots.txt files in web security and how they can be exploited if not properly configured. Robots.txt files can inadvertently expose sensitive information if misconfigured.

## Encoding, Encryption, Hashing, and Obfuscation
Explored various methods of data protection, including:

### Encoding: Transforming data into a different format (e.g., Base64).
### Encryption: Securing data using algorithms (e.g., AES, RSA).
### Hashing: Generating a fixed-size hash value from data (e.g., SHA-256).
### Obfuscation: Making code or data harder to understand to prevent reverse engineering.

## Symmetric and Asymmetric Encryption
Compared the symmetric encryption (same key for encryption and decryption) and asymmetric encryption (public and private keys). Both methods are indeed essential for secure communications.

## Base64, XOR, and UTF
Explored various encoding schemes such as Base64, XOR, and UTF, and their applications in cybersecurity. These schemes are widely used for data representation and transmission.

## Cyber Chef
Utilized Cyber Chef, a web-based tool for encryption, encoding, and data analysis. Cyber Chef simplifies complex cybersecurity tasks through a user-friendly interface.
![Screenshot 2024-07-08 at 1 52 44 AM](https://github.com/user-attachments/assets/762d2f2f-684f-4b2e-8b97-084967d673cf)


## Public and Private Keys
Discussed the importance of public and private keys in encryption and secure communications. Public keys are used for encryption, while private keys are used for decryption.

## Argon2
Learned about Argon2, a memory-intensive key derivation function designed to resist brute-force attacks. Argon2 is considered one of the most secure password-hashing algorithms.

## CrackStation
Explored CrackStation, an online tool for cracking passwords using precomputed hash tables. CrackStation is useful for understanding the vulnerabilities of weak password hashes.

## Salting
Discussed the importance of salting in password hashing to prevent rainbow table attacks. Salting adds random data to passwords before hashing to ensure unique hash values.

## Edit JWT Online (setting algorithm to none)
Online editor for a JWT token to use the "none" algorithm by Gavin Johnson-Lynn. Just need to edit the header and the payload and get the encoded output with a "none" algorithm signature.

## picoCTF Challenges
Successfully cleared three hacking tasks in picoCTF and retrieved the flag:

### Accessing Disallowed Sites: Used a robots.txt file to gain access to a disallowed site.
- Accessed the disallowed site by getting the address from robots.txt.
- Captured the flag.
![Screenshot 2024-07-10 at 2 13 12 PM](https://github.com/user-attachments/assets/d32cc24b-c5f9-4dbb-8c06-34e5373d4d6d)
![Screenshot 2024-07-10 at 2 16 50 PM 1](https://github.com/user-attachments/assets/c43079e5-b1cc-48fc-8f1c-441ae1558b0c)
![Screenshot 2024-07-10 at 2 17 32 PM](https://github.com/user-attachments/assets/bd603071-b7db-4d00-9af5-664556c41821)
![Screenshot 2024-07-10 at 2 19 44 PM](https://github.com/user-attachments/assets/8f146b71-c3db-4666-aeb4-27ddfb9c691c)

### Cracking a Password via SQL Injection: Demonstrated how SQL injection can be used to bypass authentication mechanisms.
- Used SQL queries to make an illusion for the website.
- The website thought that the query was complete with ';' but in reality, it was not.
- Injected queries as such that they can break through the filters applied on the website.
- After Round 5, checked the other .php file for the flag.
![Screenshot 2024-07-14 at 4 58 00 PM](https://github.com/user-attachments/assets/b50a7dd3-80ea-40c9-9ff8-ba12d004b28b)
![Screenshot 2024-07-14 at 5 02 11 PM](https://github.com/user-attachments/assets/8781d34d-b9a0-4b8a-9983-0fbaa51dc5d1)
![Screenshot 2024-07-14 at 5 02 12 PM](https://github.com/user-attachments/assets/749e05ac-bfaf-455f-94b2-2f2e496e7131)
![Screenshot 2024-07-14 at 5 10 42 PM](https://github.com/user-attachments/assets/35ad66d1-45d6-4800-b457-e538a79a765b)
![Screenshot 2024-07-14 at 5 11 32 PM](https://github.com/user-attachments/assets/ccb204d7-2475-40a5-a9a6-b17ea241e95d)


### Manipulating JSON Web Tokens: Used the JWT toolkit and JWT.io to manipulate and exploit JWTs.
- Can be done either using the JWT toolkit OR Edit JWT Online
- Retrieved JWT token from Cookies present in the Application part of the Inspection page.
- Used the JWT token to see what it means with JWT.io.
- Manipulated the JWT token with Edit JWT Online.
- Logged in as Admin and captured the flag.
![Screenshot 2024-07-14 at 7 05 29 PM](https://github.com/user-attachments/assets/5982c821-9085-4959-a69d-660f6800ce78)
<img width="1439" alt="Screenshot 2024-07-14 at 7 12 20 PM" src="https://github.com/user-attachments/assets/899b760d-743c-4925-a5ad-bf67e4d2b32a">
![Screenshot 2024-07-14 at 7 16 43 PM](https://github.com/user-attachments/assets/b0b8fe90-94d8-4315-aa61-22a2029fe78d)
![Screenshot 2024-07-14 at 7 17 42 PM](https://github.com/user-attachments/assets/9a8fb8bb-f603-4ea4-bee8-24d42e65e93c)
![Screenshot 2024-07-14 at 7 26 28 PM](https://github.com/user-attachments/assets/9f5043e4-8965-4028-a917-98f7e3b8dfa9)
![Screenshot 2024-07-14 at 7 28 55 PM](https://github.com/user-attachments/assets/97a2c5c2-115f-4f6a-b2aa-bb48c678f0b3)


# Contact
Feel free to reach out to me on [LinkedIn](https://in.linkedin.com/in/roshan-naidu-aka-adonis)!
