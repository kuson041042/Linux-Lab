# User and Group Management Lab

1. **Created users: user1, user2**
   - ตรวจสอบโดยใช้คำสั่ง:
     ```bash
     cat /etc/passwd | grep user1
     cat /etc/passwd | grep user2
     ```
   - **ผลลัพธ์**: พบ user1 และ user2 ในไฟล์ `/etc/passwd`

2. **Created group: developers**
   - ตรวจสอบโดยใช้คำสั่ง:
     ```bash
     cat /etc/group | grep developers
     ```
   - **ผลลัพธ์**: พบกลุ่ม developers ในไฟล์ `/etc/group`

3. **Assigned users to groups**
   - ตรวจสอบโดยใช้คำสั่ง:
     ```bash
     groups user1
     groups user2
     ```
   - **ผลลัพธ์**: user1 และ user2 ถูกเพิ่มเข้าไปในกลุ่ม developers

4. **Set permissions on home directories**
   - ตรวจสอบโดยใช้คำสั่ง:
     ```bash
     ls -ld /home/user1
     ls -ld /home/user2
     ```
   - **ผลลัพธ์**: สิทธิ์การเข้าถึงของโฟลเดอร์ถูกตั้งเป็น 700 ให้เฉพาะเจ้าของเท่านั้นที่เข้าถึงได้

