# Honey-Sessions
A tool for spoofing user sessions in active directory

description taken from spooks' blog post: https://blog.spookysec.net/DnD-Deceiving-BH/

Little to no setup is required, though there are a few constraints:

The user must be an Administrator on the Workstation
The user must be a domain user (unless you specify a SID)

If you have trust issues, the source code is provided as-is. You may feel comfortable substituting in your own NTUSER.DAT file as well. Currently, this is placed directly in the source code as a base64 encoded string. 

![image](https://user-images.githubusercontent.com/91209755/187058827-b80ccc5b-1989-48e3-901f-d87d638798c9.png)
![image](https://user-images.githubusercontent.com/91209755/187058892-9186baae-c6df-4ee9-a4f0-b9147dfda6e2.png)

make sure you disable the Firewall or make a firewall exception. By default, the Remote Registry service is filtered and you may not be able to see your session!
