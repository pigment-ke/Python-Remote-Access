
# Command and Control (C2) Server
This Python script serves as a Command and Control (C2) server for managing multiple target machines over a network. It allows the operator to execute various commands on the target machines, upload and download files, capture screenshots, and interact with the targets in real-time.

## Features
**Multiple Target Management**: The server can handle connections from multiple target machines simultaneously.
**Command Execution**: Execute commands on individual target machines or send commands to all connected targets.
**File Upload/Download**: Upload files to target machines or download files from them.
**Screenshot Capture**: Capture screenshots from the target machines.
**Webcam Capture**: Capture images from the webcam of the target machines.
**Persistent Backdoor**: Create persistence in the Windows registry to ensure the backdoor runs on system startup.
**Keylogger**: Start, stop, and dump keystrokes from the target machines.
**Help Manuals**: Provides built-in help manuals for both the server and the target communication.
**Heartbeat Mechanism**: Allows the server to periodically check the status of connected target machines.
**Graceful Exit**: Offers a graceful exit option, allowing the operator to close all connections and terminate the server.

## Usage
**Installation**: Ensure Python 3 is installed on your system. Additionally, install the required dependencies using pip install -r requirements.txt.

**Server Setup**: Run server.py on your machine. It will listen for incoming connections from target machines.

**Target Connection**: Execute client.py on the target machines, specifying the IP address and port of the server.

**Control Targets**: Once the targets are connected, the server operator can use various commands to manage them. Use the help command to view available options.

**Interact with Target**s: Send commands to individual targets or all connected targets, upload/download files, capture screenshots, etc.

**Exit**: To gracefully exit the server, use the exit command. This will close all connections and stop the server.

## Security Considerations
Encryption: Implement encryption for communication between the server and targets to secure sensitive data transmission.
Authentication: Implement authentication mechanisms to ensure that only authorized users can access the server.
Firewall Rules: Configure firewall rules to restrict access to the C2 server from unauthorized sources.
Regular Updates: Keep the server script updated with security patches and bug fixes to mitigate potential vulnerabilities.
Logging: Implement logging mechanisms to record all actions performed on the server for auditing and forensic purposes.

# Disclaimer
This script is intended for educational and research purposes only. Misuse of this tool for illegal activities is strictly prohibited. The author assumes no responsibility for any misuse or damage caused by using this script. Use it responsibly and ethically.
