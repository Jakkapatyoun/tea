# CLAUDE.md

## โปรเจกต์นี้คืออะไร

**tea** เป็น repository ที่ลงทะเบียนกับ [tea.xyz](https://tea.xyz) package manager  
ไฟล์ `tea` เก็บข้อมูล codeOwner และ quorum สำหรับระบบ package registry ของ tea protocol

## โครงสร้างไฟล์

```
tea/
├── README.md   — คำอธิบาย repository
└── tea         — tea.xyz package config (YAML: version, codeOwners, quorum)
```

## tea config file

ไฟล์ `tea` เป็น YAML format ที่ใช้โดย tea.xyz protocol ประกอบด้วย:

| Field | คำอธิบาย |
|-------|----------|
| `version` | เวอร์ชันของ config schema |
| `codeOwners` | รายการ wallet address ของเจ้าของโค้ด |
| `quorum` | จำนวน approval ขั้นต่ำที่ต้องการ |

## หมายเหตุ

Repository นี้ไม่มีซอร์สโค้ดหลัก ทำหน้าที่เป็น tea protocol registry entry เท่านั้น
