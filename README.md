# -HosxP_PCU-drug-labels-sticker-with-extendel-labels
ฉลากยาผู้ป่วยนอก+ฉลากยาเสริม สำหรับระบบ HIS ของ รพ.สต./pcu (HOSxP PCU)

วิธีติดตั้ง (Google Doc)
https://docs.google.com/document/d/18ZHjOwdj-c8_NF9VUEM3ShNpnv7HCWps99x0c79or1g/edit?usp=sharing 

-----------------------------
ฉลากยาและฉลากยาเสริม สำหรับ HOSxP PCU 
----
จัดทำ ยัสลัน  รพ.ทุ่งยางแดง  จ.ปัตตานี 
วันที่จัดทำ  30 มิ.ย. 2565
--------------------------
ได้ไอเดียและเทคนิคจากคุณ Arm เลยเอามาปรับเป็นสติกเกอร์ยาของ รพ.สต. 
ในเขตอำเภอทุ่งยางแดง ปัตตานี เพื่อให้มีข้อมูลยาและฉลากยาเสริมตามโครงการ RDU

แนวคิด:
- ให้ฉลากยาเสริมออกมาพร้อมกับสติกเกอร์ยา
- สามารถเซ็ตข้อความฉลากยาเสริม ผ่านเมนูทั่วไปของระบบ ไม่จำเป็นต้องทำผ่านฐานข้อมูลโดยตรง

ขนาดสติกเกอร์ที่ใช้ :  8.0 x 5.5  ซ.ม.^2

วิธีติดตั้งไฟล์ 
1. ดาวน์โหลดไฟล์ StickerDetailReport-รพสต.rtm ที่ผู้จัดทำทำขึ้นจาก https://github.com/dhfpatient/-HosxP_PCU-drug-labels-sticker-with-extendel-labels แล้วเปลี่ยนชื่อไฟล์เป็น StickerDetailReport.rtm
2. แทนที่ไฟล์ StickerDetailReport.rtm ในโฟลเดอร์ C:\Program Files (x86)\HOSxP_PCU ด้วยไฟล์ที่ดาวน์โหลดนี้ **อย่าลืมสำรองไฟล์ *.rtm เดิมก่อนแทนที่

วิธีเพิ่มข้อความฉลากยาเสริมของยาแต่ละตัว
ทำได้ 2 วิธีคือ 1. อัปเดตข้อมูลที่ตาราง drug_monograph ฟิลด์ summary_formulary_recommendation ตามรหัสยา icode แต่ต้องใช้ข้อความรูปแบบ Rich Text Format และ 2.อัปเดตข้อมูลจากเมนูฐานข้อมูลยาของระบบ กรณีนี้ขอแนะนำวิธีที่ 2

วิธีเพิ่มข้อความฉลากยาเสริมผ่านเมนูของระบบ
1. จากแทป HOSxP : PCU ไปที่เมนู Tools > System setting
2. ไปที่แทป ยา เลือกรายการยาที่ต้องการเพิ่ม/แก้ไขฉลากยาเสริม แล้วดับเบิลคลิกที่รายการยาเพื่อแก้ไข
3. จะขึ้นข้อมูลยาเพื่อแก้ไข ให้คลิกปุ่ม Monograph ข้างล่างเพื่อแก้ไข
4. คลิกที่แทบ Fomulary Recommendation แล้วเพิ่ม/แก้ไขข้อความตามต้องการ แล้วกดบันทึก จะได้ฉลากยาเสริมที่จะออกมาพร้อมกับฉลากยา

หมายเหตุ จากที่รับทราบข้อมูลจาก รพ.สต. บางที่ แจ้งว่าจะเกิดข้อผิดพลาดกรณีเขียนวิธีใช้ยาเอง (พิมพ์ดอกจัน “*” แล้วแก้วิธีใช้เอง) จะทำให้ฉลากยาที่เหลือพิมพ์วิธีใช้เหมือนกันทุกฉลากตามที่แก้ รวมถึงผู้ป่วยรายอื่นหลังจากนั้นด้วย ซึ่งผู้จัดทำยังไม่ได้ติดตามหาสาเหตุ หากท่านใดสามารถแก้ปัญหาได้ โปรดแจ้งผู้จัดทำ ขอขอบคุณมา ณ ที่นี้

--------------------
อ้างอิง
1. https://www.facebook.com/armdsant/posts/403430256689978/ 
2. http://tiphosxp-pcu.blogspot.com/2018/03/hosxppcu.html 
3. http://mrd-hss.moph.go.th/mrd1_hss/wp-content/uploads/2019/06/extended-label-2.pdf 
