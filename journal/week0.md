# Week 0 — Billing and Architecture
https://lucid.app/lucidchart/f5212836-a1fe-4f0d-9595-7f705513ed9b/edit?viewport_loc=-83%2C400%2C2120%2C1123%2C0_0&invitationId=inv_09699e43-b1e0-4296-986b-f36064fc8010

Created billing Alert.
Firstly, go to the billing section, checked the receive pdf invoice by email, receive free tier usage alerts(entered  target email address) Receive billing alert check boxes. Secondly, cliked on the manage billing alert. Verified the region(North Virgina) Click Billing alarm and create a billing alarm. fill out the alarm name in the select metric section and enter a maximum amount for which you will recieve email alert once expenditure gets to that amount. Click next at the bottom right. on the configure actions page select in alarm, create a new topic then reconfirm target email and click next to finish the billing alarm creation

ADDING MULTI-FACTOR AUTHENTICATION on the root user
login to AWS console as root and search for IAM(Identity Access Management) click on 'add MFA to root user" this takes you to security credentials, cretae a name for the MFA and select one of the three MFA device provided and click next, follow the prompt to finish

Setting an MFA for the root account adds another layer of secuirity to your AWS account. Anyone accessing the root account will have to go through additional level of authentication before thay can have access.


Create an AU
Adds segregation and organizes and manages security policies
Search AWS organization, and be sure to be a privileged user
1. Create an organization
2. Create an organizational unit
3. Create service control policies 
4. test to see if policies and restrictions are working as desired

Creating IAM Credentials
Go to users, click add user, fill user name, enable console access and click add user to group, check to create an IAM user, add your password method choice, check user must change password and click next, select the group if existing otherwise create a new gruop, add a name and check the admin rigths box(if you want to give admin right--not recommended), or select the user role and create the user group.

USE Cloudshell
On the AWS account click cloudshell to use the aws commandline interface


Generate credentials
Login to password generator of your choice. It is better to create a secure password, the longer the better, then goto users, IAM, user, account settings. Be sure you are logged in as root user. on the security credentials click, click custome password then type your new password and apply.

AWS CLI ON UBUNTU
I used the curl commmand "curl https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip
unzip awscliv2.zip
sudo ./aws/instrall
