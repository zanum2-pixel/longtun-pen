# ลงทุนเป็น

เว็บแอป PWA ภาษาไทยสำหรับเรียนรู้พื้นฐานการอ่านกราฟหุ้นและ Forex มีบทเรียน แบบทดสอบ กราฟจำลอง และเครื่องมือคำนวณเพื่อการศึกษา ไม่มีข้อมูลราคาตลาดจริงและไม่มีสัญญาณซื้อขาย

## เผยแพร่ด้วย GitHub Pages

1. สร้าง repository และอัปโหลดไฟล์ในโฟลเดอร์นี้ โดยใช้ branch `main`
2. เปิด **Settings → Pages** แล้วเลือก **GitHub Actions** เป็นแหล่งเผยแพร่
3. รอ workflow ชื่อ **Publish static PWA to GitHub Pages** ทำงานสำเร็จ จากนั้นใช้ URL ที่แสดงในหน้า Pages

Workflow จะนำ `index.html`, `manifest.webmanifest`, `sw.js` และ `icon.svg` ขึ้นเว็บไซต์โดยตรง ไม่ต้องติดตั้งแพ็กเกจหรือ build ก่อน

เมื่อได้ URL HTTPS แล้ว เปิดบนมือถือเพื่อเพิ่มไปยังหน้าจอหลัก: Android ใช้ Chrome; iPhone ใช้ Safari แล้วเลือก **เพิ่มไปยังหน้าจอโฮม**

## ไฟล์หลัก

- `index.html` — เนื้อหา แอป และเครื่องมือ
- `manifest.webmanifest` — ชื่อและการตั้งค่า PWA
- `sw.js` — cache สำหรับเปิดใช้งานแบบออฟไลน์
- `.github/workflows/pages.yml` — workflow เผยแพร่ GitHub Pages

เนื้อหาเป็นความรู้ทั่วไปและตัวอย่างจำลอง ไม่ใช่คำแนะนำการลงทุน
