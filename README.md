# Create-SACL-MacOS-LoginWindow

Configure the LoginWindow Service Access Control List (SACL) to only allow a specific user to login

When a Mac is bound to Active Directory you have an option with the MacOS System Preferences to lock the loginwindow to a specific user. By Default any user within the AD bind criteria could login to the computer. This script when called will challenge the user to enter their AD account, it will then lock the login window to only allow that account access to the computer.

This does not prevent local administrators access to the Computer, only Active Directory users.

Written in 10.13 and tested sucessfully on 10.13.1 through 10.13.6 and also on 10.14. 

I leveraged the support of the internet and beased this script on the response of tron_jones on the following link.

https://apple.stackexchange.com/questions/162260/allow-only-specific-ad-users-groups-to-login

Essentially the lgin window like any other service can be linited by Access Control lists. Since it is a Service it is an SACL, thus the name. We are creating a Service Access COntrol List for a specific User.

The associated here is designed to run with "Jamf" Self Service policy, meaning that a user could choose to "Secure their Mac through Self Service and thus enter their AD credental which would be applied to the Login window.
