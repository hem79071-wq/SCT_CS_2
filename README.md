🔐 Image Encryption and Decryption Tool
Cyber Security Internship – Task 02
1. Project Overview
This project demonstrates a simple image encryption and decryption technique using pixel manipulation.
The main goal is to secure image data by converting it into an unreadable format and then restoring it back using a secret key.
The project is implemented using Python and executed on Google Colab, making it accessible and easy to use without any local setup.
2. Objective of the Project
The objectives of this project are:
To understand how digital images are stored as pixel values
To apply basic cryptographic logic on image data
To demonstrate encryption and decryption using the same key
To gain hands-on experience in Cyber Security fundamentals
3. Technology and Tools Used
Python – Programming language
Google Colab – Cloud-based coding environment
NumPy – For numerical operations on pixel arrays
Pillow (PIL) – For image processing
4. Image Encryption Concept
An image is made up of pixels, and each pixel has RGB values ranging from 0 to 255.
In this project, encryption is done using the XOR (Exclusive OR) operation.
🔹 Encryption Formula
Copy code

Encrypted Pixel = Original Pixel XOR Secret Key
🔹 Example
If a pixel value is 120 and the secret key is 123:
Copy code

120 XOR 123 = Encrypted Value
This encrypted value looks random and makes the image unreadable.
5. Image Decryption Concept
Decryption is the reverse process of encryption.
The same XOR operation with the same secret key is applied to retrieve the original image.
🔹 Decryption Formula
Copy code

Decrypted Pixel = Encrypted Pixel XOR Secret Key
🔹 Example
Copy code

(120 XOR 123) XOR 123 = 120
Thus, the original pixel value is restored.
6. Working of the Project (Step-by-Step)
Step 1: Image Upload
The user uploads an image file (.jpg or .jpeg) into Google Colab.
Step 2: Convert Image to Array
The image is converted into a NumPy array so that pixel values can be accessed and modified.
Step 3: Apply Encryption
Each pixel value is encrypted using the XOR operation with a secret key.
Step 4: Save Encrypted Image
The encrypted pixel array is converted back into an image and saved as encrypted.png.
Step 5: Apply Decryption
The encrypted image is decrypted using the same secret key.
Step 6: Save Decrypted Image
The decrypted image is saved as decrypted.png, which matches the original image.
7. Input and Output Description
🔹 Input
Original image file (e.g., images.jpeg)
Secret key (integer value)
🔹 Output
Encrypted Image (encrypted.png) – Appears distorted and unreadable
Decrypted Image (decrypted.png) – Restored original image
8. Security Perspective
The encryption ensures data confidentiality
Without the correct secret key, decryption is not possible
Demonstrates the concept of symmetric key cryptography
Highlights the importance of key secrecy in cyber security
9. Applications of the Project
Secure image transmission
Digital watermarking
Basic learning model for cryptography
Cyber Security education and training
Protecting sensitive image data
10. Limitations of the Project
Uses a single static key
Not suitable for real-world high-security systems
No key management or authentication
Designed for educational purposes only
11. Conclusion
This project successfully demonstrates a simple yet effective image encryption and decryption technique using pixel manipulation and XOR operation.
It provides a strong foundation for understanding how encryption works at the data level and helps beginners explore core concepts of Cyber Security.
