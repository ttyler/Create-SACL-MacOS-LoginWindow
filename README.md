# Create-SACL-MacOS-LoginWindow

Configure the LoginWindow Service Access Control List (SACL) to only allow a specific user to login

When a Mac is bound to Active Directory you have an option with the MacOS System Preferences to lock the loginwindow to a specific user. By Default any user within the AD bind criteria could login to the computer. This script when called will challenge the user to enter their AD account, it will then lock the login window to only allow that account access to the computer.

This does not prevent local administrators access to the Computer, only Active Directory users.

Written in 10.13 and tested sucessfully on 10.13.1 through 10.13.6 and also on 10.14. 
