---
layout: page
title:  File Sharing System
description: Secure file sharing system with user authentication, file operations, and access control.
img: assets/img/filesharing.jpg
importance: 1
category: School Projects
related_publications: false
---

This [project](https://sp24.cs161.org/proj2/) focuses on designing and implementing a secure file sharing system that ensures the confidentiality, integrity, and availability of files, even in the presence of malicious adversaries. Written entirely in `Go`, the system supports various functionalities, including user authentication, file operations, and file sharing with access control mechanisms.

### Project Details

### Users and User Authentication
This section includes the creation of new users and user login functionalities.

- **InitUser**: This function creates a new user with a unique username and password. It returns an error if the username already exists or if the username is empty.
- **GetUser**: This function allows an existing user to log in using their username and password. It returns an error if the credentials are incorrect or if the user does not exist.

### File Operations
This section includes methods for managing file storage and retrieval.

- **User.StoreFile**: Creates a new file or overwrites an existing file with new contents in the user's namespace.
- **User.LoadFile**: Retrieves the contents of a specified file in the user's namespace.
- **User.AppendToFile**: Appends additional content to an existing file efficiently, ensuring minimal bandwidth usage.

### Sharing and Revocation
This section covers functionalities for sharing files with other users and revoking access.

- **User.CreateInvitation**: Generates an invitation UUID for sharing a file with another user.
- **User.AcceptInvitation**: Allows a user to accept an invitation and gain access to a shared file using a chosen filename.
- **User.RevokeAccess**: Enables the owner of a file to revoke access from a user and all users that the target user has shared the file with.

### Security and Design Considerations
The system is designed with a focus on security and efficiency:
- **User Authentication**: Ensures secure login and prevents unauthorized access.
- **Stateless Design**: Supports multiple devices for each user without relying on local memory for persistent data.
- **Efficient File Operations**: Maintains bandwidth efficiency, especially during file append operations.
- **Access Control**: Enforces strict access control to prevent unauthorized access and tampering.

### Address
For more details on this project, visit: [CS161 Project](https://sp24.cs161.org/proj2/)
