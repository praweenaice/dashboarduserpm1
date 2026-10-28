# PM1 Smart Executive Dashboard (PMONE-1020)

ระบบติดตามการดำเนินงานตามนโยบายรัฐบาลและข้อสั่งการนายกรัฐมนตรี (PM1) · Smart Executive Dashboard

## ภาพรวมระบบ (Overview)
แดชบอร์ดอัจฉริยะสำหรับติดตามและประเมินผลการดำเนินงานตามนโยบายรัฐบาลและข้อสั่งการนายกรัฐมนตรี ครอบคลุม:
- **5 รัฐบาล**: พล.อ.ประยุทธ์ จันทร์โอชา, เศรษฐา ทวีสิน, แพทองธาร ชินวัตร, อนุทิน ชาญวีรกูล (1), อนุทิน ชาญวีรกูล (2)
- **27 กระทรวงและหน่วยงานหลัก** พร้อมหน่วยงานระดับกรมย่อยกว่า 115 หน่วยงาน
- **ช่วงเวลารายงานผล**: 45 เดือน (กุมภาพันธ์ 2566 – ตุลาคม 2569) รวมกว่า 12,933 ครั้ง จาก 3,116 นโยบาย/ข้อสั่งการ

## ฟีเจอร์หลัก (Key Features)
1. **Dynamic KPI & Executive Insights**: คำนวณยอดการรายงาน, นโยบาย, ค่าเฉลี่ยความถี่ (ครั้ง/นโยบาย), อัตราเฉลี่ยต่อเดือน และ Peak Month อัตโนมัติตามตัวกรอง
2. **Cross-Government Comparison**: Scorecards เปรียบเทียบ 5 รัฐบาล, Head-to-Head 2 รัฐบาล (วิเคราะห์ Delta รายกระทรวง), และตาราง Heatmap Matrix 27 กระทรวง × 5 รัฐบาล
3. **Ministry & Department Drill-Down**: เจาะลึกระดับกระทรวง สัดส่วนกรมในสังกัด และแนวโน้มรายเดือนของแต่ละหน่วยงาน
4. **PMONE-1020 Full Matrix**: ตารางข้อมูลรายเดือนฉบับเต็ม ยุบ/ขยายรายกระทรวง พร้อมระบบสี Heatmap
5. **Future-Proof Data Import**: รองรับการนำเข้าข้อมูลใหม่ (CSV / TSV / JSON / วางข้อความ) ทั้งตารางรวมและตารางรัฐบาลใหม่ พร้อมระบบ Quick Entry และ LocalStorage persistence
6. **Print & Export to PDF Studio**: ระบบพิมพ์และแปลงเป็น PDF สำหรับรายงานผู้บริหารราชการ (@media print รองรับทั้ง A4 Landscape และ Portrait)

## โครงสร้างไฟล์ (Project Structure)
- `index.html`: เว็บแอปพลิเคชัน Single Page Application (Tailwind CSS, SVG Charts Engine, Data Parser, LocalStorage, Print Engine)
- `pmone_1020_raw_data.csv`: ชุดข้อมูลตั้งต้น PMONE-1020 ครบทั้ง 7 ตาราง
- `template_import_new_gov.csv`: เทมเพลตตัวอย่างสำหรับการนำเข้าข้อมูลรัฐบาลใหม่ในอนาคต
- `vercel.json`: การตั้งค่า Static Routing สำหรับ Vercel
