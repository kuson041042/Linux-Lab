# User and Group Management Lab

1. **Created users: user1**
   - Create user:
     ```bash
      sudo adduser user1
     ```
   - ผลลัพธ์: พบ user1 ในไฟล์ `/etc/passwd`
   - ตรวจสอบโดยใช้คำสั่ง:
     ```bash
     cat /etc/passwd | grep user1
     ```
   - ผลลัพธ์: พบ user1 ในไฟล์ `/etc/passwd`


2. **Created group: developers**

   - Create group for user:
     ```bash
     sudo groupadd developers 
     ```
   - ตรวจสอบโดยใช้คำสั่ง:
     ```bash
     cat /etc/group | grep developers
     ```
   - Add user to group:
     ```bash
     sudo usermod -aG developers user1 
     ```
   - Check user in group:
     ```bash
     groups user1
     ```
   - ผลลัพธ์: kusonh@server1:/home$ groups user1 
	user1 : user1 users developers		

3. **Set permissions on home directories**
   - Set permissions:
     ```bash
     sudo chmod 700 /home/user1
     ```
   - ผลลัพธ์: สิทธิ์การเข้าถึงของโฟลเดอร์ถูกตั้งเป็น 700 ให้เฉพาะเจ้าของเท่านั้นที่เข้าถึงได้

   - Check permissions:
     ```bash
     ls -ld /home/user1
     ```
   - ผลลัพธ์: drwx------ 2 user1 user1 4096 May 11 08:27 /home/user1



