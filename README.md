# The Azure Stay: High Distribution Costs Problem

## Data Analytics Project Canvas
<img width="1920" height="1080" alt="CP372_Presentation_Final" src="https://github.com/user-attachments/assets/b5320f65-ee26-4cb2-8b8c-e33305900f26" />

## Problem Statement / Background & Pain Points
- สถานการณ์และปัญหาของ Azure Stay:
ปัจจุบัน โรงแรม Azure Stay กำลังเผชิญกับภาวะ "High Distribution Costs" หรือต้นทุนช่องทางการจัดจำหน่ายที่สูงเกินไป แม้โรงแรมจะมีอัตราการเข้าพัก (Occupancy) และรายได้รวม (Gross Revenue) ที่ดูเหมือนจะเติบโตได้ดี แต่เมื่อพิจารณาถึงกำไรสุทธิ (Net Revenue) กลับพบว่าส่วนต่างกำไรนั้นบางลงอย่างมาก

- Pain Point หลัก: โรงแรมพึ่งพาช่องทาง Online Travel Agencies (OTAs เช่น Expedia, Booking.com) ในสัดส่วนที่สูงมาก ซึ่งช่องทางเหล่านี้เรียกเก็บค่าคอมมิชชั่นสูงถึง 15-20% ทำให้โรงแรมสูญเสียรายได้ส่วนที่ควรจะเป็นกำไรไปมหาศาล ปัญหาคือผู้บริหารยังขาดความชัดเจนว่า ตกลงแล้วช่องทางไหนที่ "ทำกำไร (Profitable)" จริงๆ ไม่ใช่แค่ช่องทางที่ "สร้างยอดจอง (Volume)" เพียงอย่างเดียว

## SMART Objectives / Value Propositions
เป้าหมายหลักของการวิเคราะห์ครั้งนี้คือการปรับปรุงโครงสร้างช่องทางการจัดจำหน่าย (Channel Mix) เพื่อเพิ่มกำไรสุทธิ โดยมีเป้าหมายแบบ SMART ดังนี้:
- Specific: ลดสัดส่วนค่าใช้จ่ายในการได้มาซึ่งลูกค้า (Cost of Acquisition: COA%) ในภาพรวมลง โดยการเพิ่มสัดส่วนยอดจองผ่านช่องทาง Direct Web (ไม่ผ่านตัวกลาง)

- Measurable: * เพิ่ม Net RevPAR (รายได้สุทธิต่อห้องพักที่เปิดขาย) ขึ้น 10%

  - ลดสัดส่วน Commission Cost รวมลง 15%

- Achievable: ทำได้จริงผ่านการโยกงบประมาณการตลาดไปกระตุ้นยอดจอง Direct Web และการปรับโควตาห้องพัก (Allotment) ในช่วง High Season

- Relevant: ตอบโจทย์ตรงจุดในการเพิ่มอัตรากำไร (Profitability) ให้กับโรงแรม Azure Stay

- Time-bound: เห็นผลลัพธ์ภายใน 6 เดือน (2 ไตรมาสถัดไป) หลังจากนำ Insights ไปปรับใช้

## Questions / Hypothesis
- Hypothesis 1 (COA Efficiency): * สมมติฐาน: ช่องทาง Direct Web เมื่อรวมกับค่าใช้จ่ายทางการตลาด (Marketing Spend) แล้ว จะยังคงมีต้นทุนการได้มาซึ่งลูกค้า (COA%) ต่ำกว่าค่าคอมมิชชั่นเฉลี่ยของกลุ่ม OTAs อย่างมีนัยสำคัญ
  - วิธีทดสอบ: เปรียบเทียบ (Total Marketing Spend / Gross Rev จาก Direct) เทียบกับ (Total Commission / Gross Rev จาก OTA)
- Hypothesis 2 (Day of Week Behavior): * สมมติฐาน: แพลตฟอร์ม OTAs จะสร้างยอดจองในช่วงวันหยุดสุดสัปดาห์ (ศุกร์-เสาร์) สูงกว่าช่องทาง Direct ซึ่งมักจะได้ลูกค้ากลุ่มองค์กร (Corporate) ในช่วงวันธรรมดา (จันทร์-พฤหัสบดี)
  - วิธีทดสอบ: สร้างกราฟแท่ง (Bar Chart) เทียบ Volume การจอง โดยแบ่งแกน X เป็นวันในสัปดาห์ (Day of Week) และแบ่งสีตาม Channel Type
- Hypothesis 3 (Rate Code Cannibalization): * สมมติฐาน: การขายราคาโปรโมชั่น (Promo) ผ่านช่องทาง OTAs ให้ค่า Net ADR (รายได้เฉลี่ยต่อห้องหลังหักคอมมิชชั่น) ที่ต่ำที่สุด และอาจต่ำกว่าจุดคุ้มทุน เมื่อเทียบกับการขายเรทปกติ (Rack Rate) ผ่านช่องทาง Direct
  - วิธีทดสอบ: หาค่าเฉลี่ย Net ADR โดยจัดกลุ่ม (Group by) ตาม Rate Code และ Booking Channel

## Key Metrics / Attributes
ตัวชี้วัดที่เราจะใช้เป็นเข็มทิศในการวิเคราะห์ ได้แก่:
- Gross Room Revenue: รายได้ก่อนหักค่าใช้จ่าย (ใช้วัด Volume)

- Net ADR: รายได้เฉลี่ยต่อห้องที่ขายได้ หลังหักคอมมิชชั่น (ใช้วัดคุณภาพของราคา)

- Commission Cost: จำนวนเงินที่จ่ายให้ 3rd party จริง

- Cost of Acquisition (COA) %: ประสิทธิภาพของช่องทาง (คอมมิชชั่น + งบการตลาด) / รายได้รวม (ยิ่งต่ำยิ่งดี)

- Net RevPAR: รายได้สุทธิต่อห้องว่างทั้งหมด (ตัวชี้วัดความสำเร็จสูงสุด)

## Data Dictionary
### Table 1: fact_bookings

| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| **booking_id** | รหัสการจอง (Primary Key) | String | BKG-10001 ถึง BKG-99999 |
| **booking_date** | วันและเวลาที่ลูกค้าทำการจอง | Datetime | 2024-10-15 08:30:00 (ต้องเกิดก่อนเช็คอิน) |
| **check_in_date** | วันและเวลาที่ลูกค้าเข้าพัก | Datetime | 2024-11-01 14:00:00 |
| **channel_id** | รหัสช่องทางการจอง (Foreign Key) | String | CH_01 ถึง CH_05 |
| **rate_code_id** | รหัสประเภทราคา (Foreign Key) | String | RT_RACK, RT_PROMO, ฯลฯ |
| **gross_room_revenue** | รายได้ก่อนหักคอมมิชชั่น | Float | 1,500.00 - 15,000.00 |
| **commission_amount** | จำนวนเงินค่าคอมมิชชั่นที่คำนวณแล้ว | Float | 0.00 - 3,000.00 |
| **net_room_revenue** | รายได้สุทธิ (Gross - Commission) | Float | 1,500.00 - 12,000.00 |
| **status** | สถานะการจอง | String | Confirmed, Cancelled, Checked-Out |

### Table 2: dim_channels
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| **channel_id** | รหัสช่องทาง (Primary Key) | String | CH_01, CH_02 |
| **channel_name** | ชื่อแพลตฟอร์ม / ช่องทาง | String | Booking.com, Direct Web, Expedia |
| **channel_type** | หมวดหมู่ช่องทาง | String | OTA, Direct, Wholesale |
| **commission_model** | รูปแบบการคิดค่าใช้จ่าย | String | Percentage, Flat Fee, Net Rate |
| **default_commission_rate** | อัตราค่าคอมมิชชั่นมาตรฐาน (%) | Float | 0.00 - 0.20 (เช่น 0.15 คือ 15%) |
| **contract_owner** | ชื่อผู้ดูแลสัญญา | String | John Doe, Jane Smith |

### Table 3: dim_rate_codes
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| **rate_code_id** | รหัสแพ็คเกจราคา (Primary Key) | String | RT_RACK, RT_CORP, RT_PROMO |
| **rate_name** | ชื่อเรียกแพ็คเกจราคา | String | Rack Rate, Corporate, Promotion |
| **is_commissionable** | สามารถคิดคอมมิชชั่นจากราคานี้ได้หรือไม่ | Boolean | True, False |

### Table 4: fact_marketing_spend
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| **spend_id** | รหัสการจ่ายเงินค่าโฆษณา (Primary Key) | String | SPD-001 ถึง SPD-999 |
| **spend_date** | วันและเวลาที่บันทึกค่าใช้จ่าย | Datetime | 2025-01-05 23:59:59 |
| **channel_id** | รหัสช่องทางที่โฆษณาสนับสนุน (Foreign Key) | String | CH_03 (ส่วนใหญ่คือ Direct Web) |
| **platform** | แพลตฟอร์มที่ลงโฆษณา | String | Google Ads, Meta Ads |
| **cost_amount** | จำนวนเงินที่จ่ายไป (USD หรือ THB) | Float | 50.00 - 5,000.00 |
| **clicks** | จำนวนคลิกที่ได้จากโฆษณา | Integer | 100 - 10,000 |

