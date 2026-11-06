# Network Programming Lab 1

## Author

- Name: [Your name]
- Student ID: 6814951034

## Project folders

This repository contains separate TCP Echo and UDP server examples:

```text
.
|-- tcp_echo_server/
|   |-- Dockerfile.client
|   |-- Dockerfile.server
|   |-- echo_client.py
|   `-- echo_server.py
`-- udp_server_test/
    |-- Dockerfile.client
    |-- Dockerfile.server
    |-- udp_client.py
    `-- udp_server.py
```

- [tcp_echo_server](tcp_echo_server/): TCP Echo client and server
- [udp_server_test](udp_server_test/): UDP client and server

## Test results

### Figure 1: TCP Echo client-server test

![TCP Echo test result](Screenshot%202026-11-06%20100948.png)

### Figure 2: UDP client-server test

![UDP test result](Screenshot%202026-11-06%20101028.png)

## ขั้นตอนที่ 3: จัดเตรียมโฟลเดอร์และส่งงานผ่าน Git Command Line

### จัดโครงสร้างโฟลเดอร์ก่อนใช้คำสั่ง Git

> **คำเตือน:** ห้ามรัน `git init` ในโฟลเดอร์ย่อย ให้จัดไฟล์ทั้งหมดไว้ในโฟลเดอร์หลักก่อน

สร้างโฟลเดอร์หลักเพียงโฟลเดอร์เดียว ตั้งชื่อ `networkPro-lab1-รหัสนักศึกษา` แล้วจัดโครงสร้างดังนี้:

```text
networkPro-lab1-รหัสนักศึกษา/
|-- tcp_echo_server/
|-- udp_server_test/
|-- README.md
`-- .gitignore
```

สร้างไฟล์ `.gitignore` ที่ระดับโฟลเดอร์หลัก และใส่ข้อความต่อไปนี้เพื่อไม่ให้อัปโหลดไฟล์ขยะ:

```gitignore
__pycache__/
*.pyc
.DS_Store
```

เปิด Terminal หรือ Command Prompt ที่โฟลเดอร์หลักนี้ แล้วรันคำสั่งตามลำดับ:

เริ่มต้น Git ในโฟลเดอร์หลัก:

```bash
git init
```

เพิ่มไฟล์ทั้งหมด รวมโฟลเดอร์ย่อย, `README.md` และ `.gitignore`:

```bash
git add .
```

บันทึกการเปลี่ยนแปลง:

```bash
git commit -m "ส่งงาน Lab 1 TCP/UDP Echo Server"
```

ตั้งชื่อ branch หลักเป็น `main`:

```bash
git branch -M main
```

เชื่อมต่อกับ GitHub Repository โดยแทนที่ชื่อผู้ใช้ GitHub และรหัสนักศึกษาให้ตรงกับของตน:

```bash
git remote add origin https://github.com/ชื่อผู้ใช้-GitHub/networkPro-lab1-รหัสนักศึกษา.git
```

อัปโหลดไฟล์ขึ้น GitHub:

```bash
git push -u origin main
```

> **หมายเหตุ:** การสร้าง GitHub Repository แบบว่าง และสร้างไฟล์ในเครื่องก่อน push ช่วยหลีกเลี่ยงปัญหาประวัติ Git ไม่ตรงกัน เช่น `unrelated histories` หรือ `non-fast-forward` ได้
