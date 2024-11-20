# Task-1: Guide to Access the Encrypted File

Follow the instructions below to access and decrypt the encrypted file.

## Steps:

1. **Download the Key and Encrypted File**
   - Download the key and encrypted file shared with you on Google Drive.

2. **Open Terminal**
   - Open your terminal on your computer.

3. **Navigate to the Downloads Folder**
   - In the terminal, navigate to your Downloads folder using the following command:
     ```bash
     cd Downloads
     ```

4. **Decrypt the Encrypted File**
   - To decrypt the file, use the following command:
     ```bash
     openssl enc -d -aes-256-cbc -in enc_file -out dec_file -pass file:./key.txt
     ```

5. **View the Content of the Decrypted File**
   - Once the file is decrypted, a new file (`dec_file`) will be created. To view its contents, run the following command:
     ```bash
     cat dec_file
     ```

Now, you should be able to see the contents of the decrypted file.
