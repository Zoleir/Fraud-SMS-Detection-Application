lib
|-- main.dart
|   เป็นไฟล์หน้าหลักโลโก้ และจักการเกี่ยวกับการแจ้งเตือน
|-- style.dart
|   เป็นไฟล์ที่ใช้กำหนดรูปแบบของข้อความ เช่น ฟอนต์ ขนาด สี น้ำหนัก และลักษณะการแสดงผลอื่นๆ
|-- constant.dart
|   เป็นไฟล์ที่กำหนดค่าคงที่ของสี
|-- firebase_options.dart
|   เป็นไฟล์ตั้งค่าโปรเจ็กต์ให้เชื่อมต่อกับ Firebase ไฟล์นี้มีการตั้งค่าและข้อมูลที่จำเป็นสำหรับการเชื่อมต่อและใช้งานบริการต่างๆ ของ Firebase
|-- models
            |-- messages.dart ไฟล์นี้คือการสร้างโมเดลข้อมูลสำหรับจัดการข้อมูลต่างๆ ของข้อความ SMS
            |-- virus.dart ไฟล์นี้คือการสร้างโมเดลข้อมูลสำหรับจัดการข้อมูลที่ได้มาจากการ virustotal
|-- pages
            |-- login.dart ไฟล์นี้เป็นส่วนของหน้า login
            |-- forgotPass.dart ไฟล์นี้เป็นส่วนของหน้า forgot Password
            |-- register.dart ไฟล์นี้เป็นส่วนของหน้า Register
            |-- otpReader.dart ไฟล์นี้เป็นส่วนของหน้ากรอก OTP เพื่อ Register ด้วย Phone number
            |-- homeScreen.dart ไฟล์นี้เป็นส่วนของหน้า homeScreen
            |-- showSMS.dart ไฟล์นี้เป็นส่วนของหน้า แสดงข้อความ SMS ที่ผู้ส่งเคยส่งมา
            |-- showResult.dart ไฟล์นี้เป็นส่วนของหน้า showResult
            |-- showResultFromNoti.dart ไฟล์นี้เป็นส่วนของหน้า showResult ที่มาจากการแจ้งเตือน
            |-- acc.dart ไฟล์นี้เป็นส่วนของหน้า Account
            |-- messageFilter.dart ไฟล์นี้เป็นส่วนของหน้า Message Filter
            |-- setting.dart ไฟล์นี้เป็นส่วนของหน้า Setting
|-- service
            |-- getAPI.dart ไฟล์นี้เป็นส่วนของการเรียกใช้ API 
|-- utils
            |-- auth_methods.dart ไฟล์นี้เป็นส่วนของ Authentication เพื่อจัดการการ Login Logout 
            |-- classify.dart ไฟล์นี้เป็นส่วนของการคำนวนความน่าจะเป็นของข้อความ SMS จากมิจฉาชีพ
|-- widgets
            |-- chip_tag.dart ไฟล์นี้เป็นส่วนของ widget chip_tag
            |-- inputFormField.dart ไฟล์นี้เป็นส่วนของ widget FormField