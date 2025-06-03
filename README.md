[Русская версия README](README_RU.md)

[![Ask DeepWiki](https://deepwiki.com/badge.svg)](https://deepwiki.com/Sppqq/ed_pro)

# 🛡️ Cipher Pro (Шифратор Pro)

All-in-one client-side security toolkit: AES file/text encryption, image pixel scrambling, and file hashing, right in your browser. Your data stays local, and no files are ever uploaded to any server.

**[Try it Live!](https://ed.sppq.site)**

## Key Features

*   **Secure File Encryption & Decryption:**
    *   Encrypt individual files or entire folders into a single `.zip.aes` archive.
    *   Decrypt `.zip.aes` archives back into a downloadable `.zip` file.
    *   Uses AES-256-CBC with PBKDF2 for key derivation and a random salt/IV.
*   **Text Encryption & Decryption:**
    *   Securely encrypt and decrypt text snippets using AES.
    *   Output format: `HEX(SALT) + HEX(IV) + HEX(CIPHERTEXT)`.
*   **Image Pixel Scrambling:**
    *   Obscure images (.png, .jpg, .webp) by scrambling their pixels based on a password-derived seed.
    *   Restore scrambled images using the same password.
    *   *Note: This is for obfuscation, not cryptographic security.*
*   **File Hashing:**
    *   Generate cryptographic hashes for any file.
    *   Supported algorithms: SHA-256, SHA-512, SHA-1, MD5.
*   **Client-Side Operations:**
    *   **Privacy First:** All processing (encryption, decryption, hashing, scrambling) is done entirely in your web browser.
    *   **No Uploads:** Your files and data never leave your computer.
*   **User-Friendly Interface:**
    *   Intuitive drag & drop for file selection.
    *   Clear tab-based navigation for different modes.
    *   Password strength meter.
    *   Dark/Light theme toggle for user preference.
    *   Progress indicators for lengthy operations.

## Technologies Used

*   HTML5
*   Tailwind CSS
*   JavaScript (ES6+)
*   [CryptoJS](https://github.com/brix/crypto-js): For AES encryption/decryption and hashing algorithms.
*   [JSZip](https://stuk.github.io/jszip/): For creating and reading ZIP archives in the browser.
*   [FileSaver.js](https://github.com/eligrey/FileSaver.js/): For saving generated files.
*   Font Awesome: For icons.

## How to Use

1.  **Access the Tool:**
    *   Open `index.html` directly in your web browser from a local clone.
    *   Or, visit the [Live Demo](#) link.
2.  **Select Operation Mode:**
    *   Navigate using the tabs: "Encryption", "Decryption", "Text", "Pixels", or "Hashing".
3.  **Provide Input:**
    *   **For File Operations:** Drag & drop your file(s)/folder or click to select.
    *   **For Text Operations:** Type or paste your text.
    *   Enter a strong password/key where required.
    *   Select algorithms or specify output filenames as needed.
4.  **Process:**
    *   Click the main action button (e.g., "Encrypt and Download", "Compute Hash").
5.  **Get Output:**
    *   Encrypted/decrypted files will be automatically downloaded.
    *   Text results or hashes will be displayed on the page, with options to copy.

## Privacy & Security

This application is designed with your privacy in mind. **All operations are performed locally in your browser.** No data, files, or passwords are ever transmitted to any server. The code is open-source, allowing you to inspect its functionality.

## Development / Running Locally

1.  Clone the repository:
    ```bash
    git clone https://github.com/Sppqq/ed_pro.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd ed_pro
    ```
3.  Open `index.html` in your preferred web browser.

No build steps or server setup are required for basic usage.

## Contributing

Contributions are welcome! If you have suggestions for improvements, new features, or bug fixes, please feel free to:
1.  Fork the repository.
2.  Create your feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

*   CryptoJS, JSZip, and FileSaver.js authors and contributors for their invaluable libraries.
