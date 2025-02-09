# LinuxAdminToolGUI (University final project for the time being, hopefully will expand more in the future)
Project Overview 
This project is a graphical user interface (GUI) tool designed to simplify user and group management, filesystem permissions, network settings, system monitoring, and firewall configuration in Linux environments. It provides an intuitive way for junior and senior system administrators to manage administrative tasks efficiently, without relying heavily on the command-line interface (CLI).

The tool is particularly beneficial for environments where senior admins oversee junior admins, ensuring structured access control, reducing misconfigurations, and improving workflow efficiency.

Key Features
1. User and Group Management
Create, modify, and delete users and groups.
Assign users to groups and configure group memberships.
Ensure that junior admins have limited access while senior admins have full control.
2. Filesystem Permission Management
Manage file and directory permissions (read, write, execute).
Configure ownership and Access Control Lists (ACLs).
Prevent unauthorized modifications by restricting junior admin privileges.
3. Audit and Logging
Record all administrative actions for accountability.
Enable log rotation and auditing for compliance.
Provide an interface for reviewing system logs.
4. Service and System Monitoring
Monitor system resources (CPU, memory, disk usage).
Manage running services (start, stop, restart).
View real-time system performance using built-in Linux utilities.
5. Network and Firewall Management
Configure network settings such as IP addresses and routes.
Monitor network activity and test connectivity.
Manage firewall rules and security policies.
6. Secure Privilege Handling
Uses sudo and polkit to manage elevated privileges securely.
Separates junior and senior admin tasks to prevent unauthorized access.
Implements session timeouts and authentication policies.
7. Role-Based Access Control (RBAC)
Senior Admins: Full control over user management, permissions, logs, and system settings.
Junior Admins: Limited control (e.g., adding users but not deleting them).
Ensures principle of least privilege (PoLP) for security.
8. GUI Interface for Accessibility
Developed using Python (Tkinter or PyQt).
Provides an intuitive and user-friendly dashboard.
Offers tooltips and documentation for usability.
Technology Stack
Programming Language: Python
GUI Framework: Tkinter / PyQt
Backend Commands: Linux CLI utilities (useradd, chmod, firewalld, systemctl, logrotate, etc.)
Security & Privilege Management: sudo, polkit
Logging & Monitoring: journalctl, auditd, df, top, ping
Version Control: Git / GitHub
How It Works
Login System:

Users log in with admin credentials.
The system grants access based on role (junior or senior admin).
Dashboard:

Displays system status, active users, file permissions, and network configurations.
Provides quick-access buttons for essential tasks.
Performing Administrative Tasks:

Users can add, modify, or delete users/groups.
File permissions and ownerships can be adjusted.
Logs can be reviewed for system activity.
Security Measures:

Unauthorized access attempts are logged.
Privileged actions require sudo authentication.
Role-based restrictions ensure safe administration.
Error Handling & Logging:

Displays errors with meaningful messages.
Logs all admin actions for troubleshooting.

Why This Tool?
Bridges the gap between junior and senior admins.
Simplifies complex tasks without requiring CLI knowledge.
Enhances security through structured role management.
Reduces misconfigurations and improves workflow efficiency.
Conclusion
This project aims to modernize Linux system administration by providing a powerful yet easy-to-use GUI tool that ensures security, efficiency, and role-based management. By integrating user, group, permission, and system monitoring functionalities in a single interface, it enhances administrative workflows while maintaining strict security measures.


