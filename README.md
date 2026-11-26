# 🌊 Warin-UBU Smart Disaster Relief & Flood Logistics Platform
### แพลตฟอร์มบริหารจัดการภัยพิบัติและศูนย์พักพิงอัจฉริยะวารินชำราบ - ม.อุบลฯ
> **Warin-UBU Smart Disaster Relief & Flood Logistics Platform with Predictive Analytics**  
> *รายวิชา 1145 204 โครงงานสำหรับนักศึกษาปีสอง (Sophomore Project) ภาคการศึกษาปลาย ชั้นปีที่ 2*  
> *สาขาวิชาวิทยาการข้อมูลและนวัตกรรมซอฟต์แวร์ คณะวิทยาศาสตร์ มหาวิทยาลัยอุบลราชธานี*

---

[![Agile Scrum](https://img.shields.io/badge/Methodology-Agile%20Scrum-blue.svg)](https://github.com/Chongdet/warin-ubu-smart-flood)
[![AUN-QA](https://img.shields.io/badge/Standard-AUN--QA%20Compliant-success.svg)](https://github.com/Chongdet/warin-ubu-smart-flood)
[![Story Points](https://img.shields.io/badge/Total%20Story%20Points-85-orange.svg)](https://github.com/Chongdet/warin-ubu-smart-flood)
[![License](https://img.shields.io/badge/License-Academic%20Use-lightgrey.svg)](https://github.com/Chongdet/warin-ubu-smart-flood)

---

## 📌 บทสรุปโครงงาน (Project Overview)
อำเภอวารินชำราบและพื้นที่โดยรอบมหาวิทยาลัยอุบลราชธานี จังหวัดอุบลราชธานี ประสบวิกฤตอุทกภัยซ้ำซากเป็นประจำทุกปี ส่งผลกระทบต่อทั้งชุมชนริมแม่น้ำมูล หอพักนักศึกษา และสถานประกอบการ จากการลงพื้นที่สำรวจและวิจัยเชิงลึกผ่านแบบสอบถามผู้ประสบภัยจริงจำนวน **68 คน (N=68)** โครงงานนี้จึงมุ่งแก้ปัญหาหลัก 3 ประการ:
1. **การขาดระบบเตือนภัยล่วงหน้ารายพิกัดตัวบ้าน (Micro-Location Warning Gap):** พยากรณ์ระดับน้ำล่วงหน้า 24–48 ชม. เชื่อมโยงสถานีต้นน้ำ M.182 (อ.ท่าตูม) M.2 (อ.ราษีไศล) และ M.7 ร่วมกับระดับความสูงพื้นบ้าน 3 รูปแบบมาตรฐาน (ความคลาดเคลื่อน ≤ ±15 ซม.)
2. **วิกฤตการอพยพของสัตว์เลี้ยง (Pet Evacuation & Shelter Dilemma):** ค้นหาศูนย์พักพิงที่เปิดรับสัตว์เลี้ยง และเครือข่ายโรงแรม/หอพักช่วยเหลือสังคมในอัตราพิเศษ
3. **วิกฤตสิ่งของบริจาคไม่ตรงกับความต้องการจริง (Relief Supply Mismatch):** ระบบกระจายของบรรเทาทุกข์เฉพาะกลุ่ม (อาหารฮาลาล เจ นมผงเด็ก อาหารสัตว์เลี้ยง) พร้อมกระดาน Dynamic Live Wishlist และระบบคลังสิ่งของบรรเทาทุกข์แบบ Zero Negative Stock

---

## 👥 สมาชิกในทีม Scrum (Agile Scrum Team)
* **รหัสวิชา:** 1145 204 โครงงานสำหรับนักศึกษาปีสอง (Sophomore Project) ภาคการศึกษาปลาย ชั้นปีที่ 2
* **อาจารย์ที่ปรึกษาโครงงาน:** **อาจารย์ ดร.ทศพร อเลิร์ป (Dr. Tossaporn Alherbe, Ph.D. Southampton)**

| ลำดับ | รหัสนักศึกษา | ชื่อ-สกุล | วิชาเอก | บทบาทหน้าที่หลักในทีม (Agile Role) |
| :---: | :---: | :--- | :---: | :--- |
| **1** | 68114540214 | **นายทรงเดช จำปาเทศ (แม็ก)** | **วิทยาการข้อมูล (DS)** | **Scrum Master & Data Scientist**<br>รับผิดชอบการบริหารกระบวนการ Agile Scrum วิจัยความต้องการผู้ใช้ สถิติ N=68 คน พัฒนาโมเดลพยากรณ์น้ำ M.7 ร่วมกับสถานีต้นน้ำ M.182 / M.2 และควบคุมความมั่นคงปลอดภัยข้อมูล PDPA |
| **2** | 68114540489 | **นายยศสรัล ถิระบุต (ป๊อป)** | **วิทยาการข้อมูล (DS)** | **Product Owner & Data Engineer**<br>รับผิดชอบการวิจัยสถิติ N=68 คน ออกแบบฐานข้อมูล 3NF ท่อส่งข้อมูล Data Pipeline เชื่อมโยงโทรมาตรต้นน้ำ RESTful API (Node.js) และระบบคลัง Zero Negative Stock |
| **3** | 68114540399 | **นางสาวปัญญาพร มูลดับ (ฝ้าย)** | **นวัตกรรมซอฟต์แวร์ (SI)** | **Frontend Developer & UI/UX Designer**<br>รับผิดชอบการออกแบบ Responsive UI ด้วย Design Thinking พัฒนาระบบส่วนหน้าด้วย React.js เชื่อมต่อแผนที่สารสนเทศภูมิศาสตร์ GIS Map หมุด SOS และระบบ Fast-pass QR Code |

---

## 🎯 วัตถุประสงค์ตามหลัก SMART & AUN-QA Standard (Measurable 100%)
* **วิศวกรรมซอฟต์แวร์ (Web Architecture):** API Response Time เฉลี่ยไม่เกิน 2.0 วินาที และส่งมอบ MVP 1.0 ภายในสัปดาห์ที่ 8
* **ระบบสารสนเทศภูมิศาสตร์ (GIS Map Service):** Render แสดงผลหน้าต่างแผนที่ GIS และสลับเลเยอร์ระดับน้ำได้ภายในเวลา < 2.0 วินาที
* **วิทยาการข้อมูลและ AI (Water Forecasting):** อัตราความคลาดเคลื่อนของการคาดการณ์ระดับน้ำเฉลี่ยไม่เกิน ±15 เซนติเมตร เทียบกับ M.7
* **ระบบเตือนภัยรายหลัง (House-Level Alert):** ประมวลผลคำนวณส่วนต่างระดับน้ำและแจ้งเตือนภัยเสร็จสิ้นภายใน < 3.0 วินาที
* **การจัดการโลจิสติกส์ (Triage & Supplies):** ป้องกันการตัดสต็อกสิ่งของบริจาคติดลบ (Zero Negative Stock) 100% ภายใต้สภาวะ Race Condition
* **การประเมินผลผู้ใช้ (Usability & Impact):** ผ่านการทดสอบจากผู้ใช้งานจริง ≥ 15 คน ด้วยคะแนน SUS ≥ 75 คะแนน

---

## 📊 Agile Kanban Board & Backlog
โครงการนี้บริหารจัดการการส่งมอบงานด้วย **Agile Scrum (16 สัปดาห์)** โดยแบ่งเป็น 4 Sprints รวม **85 Story Points**:
* 📋 **[คลิกเพื่อเข้าสู่ GitHub Project Kanban Board](https://github.com/Chongdet/warin-ubu-smart-flood/projects)**
* **Sprint 0 (W1–3):** Foundation & Setup (Inception Phase)
* **Sprint 1 (W4–7):** Core Architecture, GIS & Shelter UI (14 Points - MVP 1.0)
* **Sprint 2 (W8–11):** Hydrology Model, GPS SOS & Triage (46 Points - MVP 2.0)
* **Sprint 3 (W12–16):** Final Integration, Usability Testing & Pitching (25 Points)

---

## 📂 เอกสารโครงการฉบับทางการ (Official Deliverables)
เอกสารการดำเนินงานช่วง Inception Phase ฉบับสมบูรณ์จัดเก็บไว้ในโฟลเดอร์ [`docs/`](./docs/):
* 📄 **[ดาวน์โหลดเอกสาร Final PDF สำหรับส่งอาจารย์](./docs/เอกสารนำเสนอหัวข้อโครงงาน%20_%20แพลตฟอร์มบริหารจัดการภัยพิบัติและศูนย์พักพิงอัจฉริยะ.pdf)** *(ไฟล์หลักของโครงงาน)*
* 📝 **[เอกสารนำเสนอหัวข้อโครงงานฉบับสมบูรณ์ (Markdown)](./docs/เอกสารนำเสนอหัวข้อโครงงาน_Final.md)**
