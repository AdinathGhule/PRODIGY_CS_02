# Image Encryption Tool

This project presents a straightforward image encryption and decryption tool built using Python's tkinter for the graphical user interface and PIL (Pillow) for image manipulation.

## Overview
The Image Encryption Tool enables users to secure their images through encryption and subsequently decrypt them using a specified encryption key. The encryption process modifies each pixel of the image through a mathematical operation, while decryption reverses this to restore the original image.

## Features
- **Select Image**: Allows users to choose an image file (supports .png, .jpg, .jpeg formats).
- **Encryption Key**: Users provide an integer key for encryption and decryption.
- **Encrypt Image**: Encrypts the chosen image and saves the encrypted version.
- **Decrypt Image**: Decrypts the encrypted image to recover and save the original image.

## How It Works
The tool utilizes tkinter for the interface. Once an image is selected and an encryption key is provided:

- **Encrypt**: Adds the key value to each pixel's RGB values modulo 256.
- **Decrypt**: Subtracts the key value from each pixel's RGB values modulo 256.

## Requirements
- Python 3.x
- tkinter (usually included in standard Python installations)
- Pillow (PIL) library: `pip install pillow`

## How to Run
1. **Clone the Repository**:
   ```sh
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Install Dependencies**:
   ```sh
   pip install pillow
   ```

3. **Run the Program**:
   ```sh
   python pixel.py
   ```

4. **Using the Program**:
   - Click **Select Image** to choose an image file.
   - Enter an integer **Encryption Key**.
   - Click **Encrypt** to encrypt the selected image.
   - Click **Decrypt** to decrypt the previously encrypted image.

## Project Structure
**File**: `pixel.py`  
This file contains the core implementation of the Image Encryption Tool using tkinter for the GUI and PIL for image processing.

### Functions
- `select_image()`: Opens a file dialog to select an image file.
- `encrypt_image()`: Encrypts the selected image using the specified key.
- `decrypt_image()`: Decrypts the previously encrypted image using the same key.

### GUI Components
- `button_select_image`: Button to select an image file.
- `entry_key`: Entry field for the encryption key.
- `button_encrypt`: Button to initiate the encryption process.
- `button_decrypt`: Button to initiate the decryption process.
- `label_image`: Displays the selected and decrypted images.

## Contributions
Contributions are welcome! If you have suggestions, discover bugs, or want to add features, please open an issue or a pull request on GitHub.

Thank you for using the Image Encryption Tool! Enjoy encrypting and decrypting your images securely.

## How to Add this README.md to Your Repository
### Create the README.md File
1. Open your text editor or IDE.
2. Create a new file named `README.md`.
3. Copy and paste the content above into the README.md file.
4. Save the file in the same directory as your `pixel.py` file.

### Upload the README.md File to GitHub
**Using the GitHub web interface**:
1. Navigate to your repository on GitHub.
2. Click on "Add file" > "Create new file".
3. Name the file `README.md`.
4. Paste the content from the above template into the editor.
5. Scroll down and click "Commit new file" to add it to the repository.

**Using Git commands**:
1. In your terminal, run the following commands:
   ```sh
   git add README.md
   git commit -m "Added detailed README.md file for Image Encryption Tool"
   git push origin master
   ```
