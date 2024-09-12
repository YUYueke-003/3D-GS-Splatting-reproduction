# 3D-GS-Splatting-reproduction
Here explained my process of doing reproduction of 3d gaussian splatting on remote server with linux platform via ssh connection. I will write this readme.md in details, hope it can help with your attempts!

I connect to the remote server via SSH pubkey. In case you're like me who know nothing about remote server connection …… Let's start from the SSH connection. 

#### 1. Establish the SSH connection to the remote server. ####
Find your ssh pubkey or generate one. See the link [here](https://www.freecodecamp.org/chinese/news/ssh-keygen-how-to-generate-an-ssh-public-key-for-rsa-login/). 
Several things need to be noticed: When you generate your keys, only using ```ssh-keygen``` might give you several kinds of results, including "ssh-rsa", "ssh-ed22519".etc. There might be servers not working well with some kind of pubkeys(such as our lab's), so better determine the type when generate the key using ```-t rsa``` to specifically determine the type to be id_rsa ones. Also, to convenient yourself, remember to type in the place which stores your keys might not be the path you expected!!! For example, my keys were located in ```C:\SPB_Data\.ssh\id_rsa``` not as expected in ```D:\admin\username\.ssh\id_rsa```. 
