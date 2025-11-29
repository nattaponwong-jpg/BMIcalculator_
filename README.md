# BMIcalculator_
BMIcalculator for   CS436
BMIcalculator for CS436 ฟังก์ชันหลักการเลือกเพศ: กำหนดเพศ (ชาย/หญิง) เพื่อการคำนวณและแปลผลที่อาจแตกต่างกันการป้อนข้อมูล: บันทึกน้ำหนัก, ส่วนสูง, และอายุ โดยใช้ตัวเลือกระบบ Spinner/Sliderการคำนวณ BMI: ประมวลผล BMI ตามสูตรมาตรฐานแสดงผลลัพธ์: แสดงค่า BMI, การแปลผล (Normal/Overweight), และช่วงน้ำหนักที่เหมาะสม

วิธีการติดตั้งและรันโปรเจกต์

ข้อกำหนดเบื้องต้นติดตั้ง Flutter SDK และตั้งค่า Environment Pathติดตั้ง IDE ที่รองรับ Flutter (เช่น VS Code หรือ Android Studio)มีอุปกรณ์จำลอง (Emulator) หรืออุปกรณ์จริงที่พร้อมใช้งาน
การติดตั้ง (Clone the Repository)Bash# ในกรณีที่โค้ดอยู่ใน GitHub git clone [URL_GITHUB_REPOSITORY_ของท่าน] cd bmi_calculator_app
การดึง Dependencyเปิด Terminal ในโฟลเดอร์โปรเจกต์และรันคำสั่งเพื่อดาวน์โหลดแพ็กเกจที่จำเป็น:Bashflutter pub get
วิธีรันแอปพลิเคชันตรวจสอบว่ามี Emulator หรืออุปกรณ์เชื่อมต่ออยู่ จากนั้นรันคำสั่ง:Bashflutter run
โครงสร้างโค้ด (Code Structure) lib/main.dartจุดเริ่มต้นของแอปพลิเคชัน, กำหนด Theme และ Routing lib/models/เก็บ Class โมเดลข้อมูลที่ใช้ในการส่งผ่านข้อมูลระหว่างหน้าจอ lib/screens/หน้าจอหลักทั้งหมดของแอปพลิเคชัน (Gender Selection, Input Data, Result) lib/utils/เก็บ BMICalculator Class ซึ่งเป็นส่วนของ Business Logic lib/widgets/UI Components ที่สามารถนำกลับมาใช้ใหม่ได้ (เช่น ปุ่ม, Card Layout)
