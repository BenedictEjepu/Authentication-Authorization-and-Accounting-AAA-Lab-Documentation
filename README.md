# Authentication-Authorization-and-Accounting-AAA-Lab-Documentation
This lab demonstrate the fundamental concepts of authentication,Authorization,
and Accounting (AAA) in a linux environment using multiple user accounts.
The exercises focus on user authentication,file and directory permisions, 
access control, and user activity tracking through practical command-line operations.

## Objectives
.Understand the principles of Authentication, Authorization, and accounting (AAA)
.Create and manage multiple user accounts.
.Authenticate users using passwords.
.Explore files and directory ownership.
.Modify permissions using symbolic and numeric methods.
.Verify access control through practical testing.
.Examine user activity and login information using linux accounting commands 

## Lab Environment
.OPerating System: Kali Linux
.Shell: Zsh
.Users: Kali, jeo, jenny

## Authentication
Authentication is the process of verifying a user's identity before getting access to a system.

## Commands used:
.su - joe
.su - jenny
The lab demonstrated successful user authentication through password verification 
and showed that access is denied when incorrect credentials are supplied.

## Authorization
Authorization determines what an authenticated user is permitted to access or modify.
## Commands used:
.ls -ld /home/joe
.ls -ld /home/jenny
.chmod o+r /home/jenny
.chmod o+x /home/jenny
.chmod 705 /home/jenny
The exercises demonstrated how linux uses ownership, groups,and permissions 
to control access to resources.

## Symbolic Permissions
Examples:
.chmod o+r /home/jenny
chmod o-x /home/jenny
chmod g+x /home/joe

## Numeric Permisions
Examples:
.chmod 705 /home/jenny
.chmod 755 /home/joe
.chmod 700 /home/joe
These activities reinforced the relationship between numeric and symbolic permision assignments.

## Accounting
Accounting provides a record of user activities and system usage.
## Commands Explored:
.whoami
.id 
.history
.who
.w
.last
These commands provide information about user identity, 
command history, active sessions, and login activity.

## Key Findings
.Authentication verifies user identity using credentials.
.Authorization controls access based on permissions and ownership.
.Directory access requires execute permissions.
.Read permissions allow directory contents to be viewed.
.Write permissions are required to create or modify files.
.Linux permissions management can be performed using symbolic or numeric notation.
.Accounting mechanisms help monitor and audit user activity.

## Lessons Learned 
This lab provided practical experience with linux user management and access control.
The exercises demonstrated how authentication, authorization, and accounting
work together to secure a system and manage user access.

## Conclusion
The AAA model is a fundamental security framework used in linux and enterprise environments. 
Through practical exercises involving user authentication, permision management,
and activity monitoring, this lab demonstrated how linux enforces access control 
and tracks users interactions with system resources.

