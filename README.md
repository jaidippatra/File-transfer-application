Project: Encrypted File Transfer Application (Sender/Receiver)
Overview
This project provides a secure file transfer system between two computers using AES encryption. It includes two separate Python applications:

File Sender (sender_gui.py): Allows users to send files to a recipient over a network.
File Receiver (receiver_gui.py): Enables users to receive encrypted files sent from the sender.
Both applications are built using PyQt5 for the GUI, AES encryption for file security, and socket programming for network communication.

Features
Secure Transmission: Files are encrypted using AES encryption before being sent over the network.
User-Friendly Interface: Both sender and receiver apps feature simple, intuitive GUIs.
Real-time Progress: The applications display progress bars to monitor file sending/receiving processes.
File Descriptions
1. sender_gui.py (File Sender)
Purpose: This script allows users to select a file and send it to a receiver.
Main Components:
File Selection: Users can select the file they want to send using a file dialog.
Send Button: Starts the transmission of the selected file.
Progress Bar: Displays the progress of the file being sent.
Speed Display: Shows the speed of the file transfer.
2. receiver_gui.py (File Receiver)
Purpose: This script enables users to receive files that are sent to them over the network.
Main Components:
Folder Selection: Users choose the folder where the received file will be stored.
Start Button: Starts listening for incoming files.
Progress Bar: Displays the progress of the file being received.
Decryption: The received file is decrypted and saved in the specified folder.
Dependencies
PyQt5: For the graphical user interface.
PyCryptodome: For AES encryption.
Python 3.x: Ensure that you have Python 3 installed on your system.
Socket Programming: To enable network communication between sender and receiver.

Usage
Start the Receiver: First, launch the receiver app on the machine that will receive the file.
Select Destination Folder: Use the receiver GUI to select where the incoming file should be saved.
Start the Sender: Launch the sender app on the machine that will send the file.
Select File: Use the sender GUI to select the file you want to send.
Send the File: Click the "Send" button, and the transfer will begin.
The receiver will automatically decrypt and save the file once the transfer completes.
Security Considerations
This system uses AES encryption, which ensures that the file's contents are encrypted before transfer, providing confidentiality during transmission.
Future Improvements
Add support for multiple file types.
Implement a more sophisticated encryption key exchange protocol.
Add error handling for network disconnections.
License
This project is licensed under the MIT License.

