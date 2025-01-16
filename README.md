# Managing-Group-Policy-and-User-Accounts-in-Active-Directory
This repository provides step-by-step instructions for managing Group Policy and user accounts in an Active Directory environment. It includes guidelines for editing policies, adding new users, and resetting passwords



## Editing Group Policy

### View Password Policy
1. Go to **Tools > Group Policy Management**
   - Your domain should be under **Domains > yourdomain**
2. Under your domain, select **Default Domain Policy**
3. Click **OK** when Group Policy Management Console appears
4. Select the **Settings** tab to view Policy details
5. Scroll down to **Computer Configuration** to view password policy


https://github.com/user-attachments/assets/82369297-4f85-4fd1-a2da-00dee1133166


### Edit Policy
1. Right-click **Default Domain Policy**
2. Select **Edit**
3. A Group Policy Management Editor will pop up
   - Select **Computer Configuration > Policies > Windows Settings**
   - Go to **Security Settings > Account Policies**
     - Under **Password Policy**, you can change the length, age, and password history
     - Under **Account Lockout Policy**, you can determine the number of password attempts and their duration


https://github.com/user-attachments/assets/0cc1e375-4e97-4b16-b624-bc3ad204173b


## Adding New User
1. In the Server Manager
   - Go to **Tools > Active Directory Users and Computers**
   - Right-click **Users** folder
   - Select **New > User**
     - Fill in the fields:
       - First name, Last name, User logon name
     - Click **Next**
     - Enter password and leave **User must change password at next logon** checked
     - Click **Next**
     - Lastly, click **Finish**


https://github.com/user-attachments/assets/873a91f7-3e2a-487e-89f0-36aa08df348a


2. Go to Windows 10 Virtual Machine
   - Select **Other user**
   - Enter Credentials
   - You will be prompted to create a new password
   - After entering a new password, you will be granted access


https://github.com/user-attachments/assets/fff318fa-11e9-46e0-bb62-63f2397a99a8


## Resetting Password
1. Go to Windows 10 Virtual Machine
   - Select **Other user**
   - Select User
   - To lock Account ,Enter the wrong password several times


https://github.com/user-attachments/assets/36368e4f-e725-4638-82f2-f05790cd2865



2. In the Server Manager
   - Go to **Tools > Active Directory Users and Computers**
   - Under **Users** folder, select the user
   - Right-click the user
   - Select **Reset Password** and enter new password
   - Leave **User must change password at next logon** checked
   - Select **Unlock the user's account** if the user account is locked
