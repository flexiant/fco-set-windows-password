Installing cloudbase-init in Windows
====================================

As mentioned, cloudbase-init can be installed in Windows alongside custom scripts. Here is how to install cloudbase-init with a Python script to set the password for the Administrator user.

CloudBase state their software works with 2003,2008,2012 (R1/R2). It is possible the Python script needs to be modified for different versions of Windows.

Note: This will only set the password for the Administrator user

1. First download the MSI installer from the following URL:  
   [http://repo.flexiant.com/images/public/tools/CloudbaseInitSetup_Beta_x64.msi]

2. Then, run the installer and accept all default options.

3. Once installed you may choose to enable sysprep so GUUIDs are regenerated.

4. Lastly, save the SetWindowsPassword.py script to the following location:  
   `C:\Program Files (x86)\Cloudbase Solutions\Cloudbase-init\LocalScripts\`

The machine can then be shutdown and used to create an Image. Within FCO you use Create Image from Disk. Ensure you set the Default Username to 'Administrator' and Generate Password is enabled.

Docs for this can be found here: [http://docs.flexiant.com/display/DOCS/Creating+an+Image]
