# The Azure Stay: High Distribution Costs Problem

## Data Analytics Project Canvas

## Problem Statement / Background
ฉันและเพื่อน ๆ เป็นเป็นเจ้าของโรงแรมอิสระขนาดกลางชื่อชื่อ The Azure Stay แม้ว่าที่พักพักจะสวยงาม แต่เราพบว่ากำไรของเราไม่ได้เพิ่มขึ้นตามเลยแม้ว่า อัตราการเข้าพักจะอยู่ในระดับที่น่าพึงพอใจก็ตาม ซึ่งจากการที่เราลองวิคราะห์สาเหตุของปัญหาเราพบว่าปัจจุบันโรงแรงของเรามีการพึ่งพาช่องทาง Online Travel Agencies (OTAs) เช่น Agoda หรือ Booking.com ทำให้ต้องแบกรับค่าคอมมิชมิชั่นในอัตราที่สูง

## SMART Objectives / Value Propositions
เป้าหมายหลักของการวิเคราะห์ครั้งนี้คือการเพิ่มรายได้สุทธิต่อห้องพักที่เปิดขาย (Net RevPAR) ขึ้น 10% และลดสัดส่วนต้นทุนการได้มาซึ่งลูกค้า (Cost of Acquisition: COA %) ลง 5% ภายในระยะเวลา 6 เดือน ผ่านการวิเคราะห์ข้อมูลและปรับลดสัดส่วนยอดจองจากช่องทาง OTA ที่มีค่าคอมมิชชันสูง มาเป็นการเพิ่มยอดจองตรง (Direct Booking)

โดยมีเป้าหมายแบบ SMART ดังนี้:
- Specific: ปรับโครงสร้างสัดส่วนช่องทางการจอง (Channel Mix) ให้เหมาะสม โดยมุ่งเป้าไปที่การลดการพึ่งพาช่องทาง OTA (เช่น Agoda, Booking.com) และกระตุ้นการจองผ่านช่องทางตรง (Direct Web) เพื่อเพิ่มรายได้หลังหักค่าคอมมิชชัน (Net Room Revenue) โดยที่อัตราการเข้าพัก (OCC) ยังคงอยู่ในระดับที่ดี

- Measurable: สามารถชี้วัดความสำเร็จได้จากชุดข้อมูลที่คุณมี โดยติดตามตัวเลข 2 ตัวหลัก:
    - COA % (Cost of Acquisition): ต้องลดลง 5% (วัดจากผลรวมของ Commission Cost + Marketing Spend หารด้วย Total Revenue)

    - Net RevPAR: ต้องเพิ่มขึ้น 10% (วัดจาก Gross Revenue ลบ Commission Cost แล้วหารด้วย Total Rooms Available)

- Achievable: สามารถบรรลุเป้าหมายได้ด้วยการทำ Exploratory Data Analysis (EDA) อย่างละเอียดเพื่อเจาะลึกดูประสิทธิภาพของแต่ละ Channel และ Rate Code เมื่อเราพบช่องทางที่มีต้นทุนสูงแต่ประสิทธิภาพต่ำ เราสามารถโยกงบประมาณส่วนนั้นไปลงทุนใน fact_marketing_spend เพื่อทำแคมเปญดึงดูดลูกค้าให้มาจองตรงได้อย่างมีประสิทธิภาพมากขึ้น

- Relevant: ตอบโจทย์ปัญหาคอขวดของ The Azure Stay อย่างตรงจุด เนื่องจากปัจจุบันโรงแรมไม่มีปัญหาเรื่องการหาลูกค้า (Occupancy เป็นที่น่าพึงพอใจ) แต่มีปัญหาเรื่องต้นทุนช่องทาง การโฟกัสที่ค่า Net ADR และ Net RevPAR จึงเป็นการแก้ปัญหาเพื่อดึง "กำไรสุทธิ" กลับเข้าสู่ธุรกิจอย่างแท้จริง

- Time-bound: กำหนดระยะเวลาในการปรับเปลี่ยนกลยุทธ์และประเมินผลภายใน 6 เดือน โดยสามารถแบ่งการติดตามผลจาก Dashboard เป็นรายเดือน เพื่อดูแนวโน้มการเปลี่ยนแปลงของ Channel Mix อย่างใกล้ชิด

## Questions / Hypothesis

### Bussiness Question
1. ต้นทุนที่แท้จริงของการจองตรง (Direct Web) คุ้มค่ากว่า OTA จริงหรือไม่?
2. โปรโมชัน (Rate Code) แบบใดที่เมื่อขายผ่าน OTA แล้วทำให้โรงแรมสูญเสียกำไร (Net ADR) มากที่สุด? 
3. พฤติกรรมการพึ่งพา OTA ที่มีค่าคอมมิชชันสูง มักเกิดขึ้นในวันใดของสัปดาห์ (Day of Week) มากที่สุด? 
4. อัตราการยกเลิกการจอง (Cancellation Rate) ของ OTA สร้างต้นทุนแฝงและตัดโอกาสการทำกำไรไปเท่าไรเมื่อเทียบกับ Direct Web? 
5. ช่องทาง (Channel) ใดที่มีประสิทธิภาพสูงสุด (High Net RevPAR, Low COA%) และควรได้รับการอัดฉีดงบการตลาดเพิ่ม? 

### Hypothesis
1. ต้นทุนการได้มาซึ่งลูกค้า (COA%) ของช่องทาง Direct Web อยู่ในระดับต่ำกว่า 10% โดยต่ำกว่าค่าเฉลี่ยคอมมิชชันของช่องทาง OTA (15-20%) อย่างมีนัยสำคัญ 
2. ยอดจองที่ใช้ Rate Code กลุ่ม "Promotion/Discount" ผ่านช่องทาง OTA ประเภท Percentage Model จะมีค่า Net ADR ต่ำกว่ายอดจองที่ใช้ Rate Code เดียวกันบน Direct Web อย่างน้อย 15-20% 
3. ยอดจองในวันหยุดสุดสัปดาห์ (ศุกร์ ถึง เสาร์) กว่า 60% มาจากช่องทาง OTA ทำให้แม้ภาพรวมโรงแรมจะมี Gross RevPAR สูงในวันหยุด แต่ Net RevPAR กลับถูกหักล้างจนไม่ทัน Gross RevPAR 
4. ช่องทาง OTA มีสัดส่วนยอดจองสถานะ 'Cancelled' สูงกว่า Direct Web มากกว่า 10% ทำให้เกิดการสูญเสียโอกาส (Lost Net Revenue) ที่ประเมินค่าได้ 
5. การเพิ่มงบประมาณในตาราง fact_marketing_spend มีความสัมพันธ์เชิงบวก กับจำนวนยอดจองตรง (Direct Web) ภายใน 7 วัน และรายได้ Net Revenue ที่ได้กลับมา มีมูลค่าสูงกว่าค่าโฆษณาที่จ่ายไป (ROI > 100%)

## Key Metrics / Attributes
1. Key Metrics 
    - Net Room Revenue: รายได้สุทธิหลังหักค่าคอมมิชชัน
    - COA % (Cost of Acquisition): ต้นทุนรวมในการหาลูกค้า (Commission + Marketing Spend) หารด้วยรายได้รวม
    - Net ADR & Net RevPAR: ราคาเฉลี่ยและรายได้ต่อห้องที่เปิดขาย "แบบสุทธิ" (หักต้นทุนแล้ว)
    - Cancellation Rate: เปอร์เซ็นต์อัตรายกเลิกการจอง
    - Marketing ROI: ความคุ้มค่าของเงินโฆษณาที่ยิงไปเพื่อดึงยอดจองตรง

2. Key Attributes
    - Channel Type: กลุ่มช่องทางการจอง (OTA, Direct Web)
    - Rate Code: ประเภทโปรโมชันหรือราคา (ใช้หาตัวที่ทำให้ขาดทุน)
    - Day of Week: วันที่เข้าพัก (จันทร์-อาทิตย์ เพื่อดูพฤติกรรม OTA ช่วงวันหยุด)
    - Status: สถานะการจอง (Confirmed, Cancelled, Checked-Out)
    - Commission Model: รูปแบบการหักเงินของ OTA (Percentage, Flat Fee)



## Data Dictionary
### Table 1: `fact_bookings` 
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| booking_id | รหัสการจองของลูกค้า (Unique ID / PK) | String | BKG_00001, BKG_00002 |
| booking_date | วันและเวลาที่ลูกค้าทำการกดจอง | Datetime | 2025-01-15 14:30:00 |
| check_in_date | วันและเวลาที่ลูกค้าเช็คอินเข้าพัก | Datetime | 2025-02-01 15:00:00 |
| check_out_date | วันและเวลาที่ลูกค้าเช็คเอาท์ | Datetime | 2025-02-03 11:30:00 |
| channel_id | รหัสช่องทางการจอง (FK ไปยัง dim_channels) | String | CH_01, CH_02, CH_03 |
| rate_code_id | รหัสแพ็กเกจราคา (FK ไปยัง dim_rate_codes) | String | RC_PROMO, RC_RACK |
| gross_room_revenue| รายได้รวมค่าห้องพักที่ลูกค้าจ่าย (ก่อนหักคอมมิชชัน) | Float | ค่าที่มากกว่าหรือเท่ากับ 0 เช่น 5400.00, 3600.00, 0.0 |
| commission_amount| จำนวนเงินค่าคอมมิชชันที่โรงแรมต้องจ่ายให้ช่องทาง | Float | ค่าที่มากกว่าหรือเท่ากับ 0 เช่น 972.00, 50.00, 0.0 |
| net_room_revenue | รายได้ค่าห้องพักสุทธิที่โรงแรมได้รับ (Gross - Commission) | Float | ค่าที่มากกว่าหรือเท่ากับ 0 เช่น 4428.00, 3550.00, 0.0 |
| status | สถานะปัจจุบันของการจอง | String | Checked-Out, Cancelled, Confirmed |

---

### Table 2: `dim_channels`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| channel_id | รหัสอ้างอิงช่องทางการจอง (Unique ID / PK) | String | CH_01, CH_02, CH_03 |
| channel_name | ชื่อของช่องทางการจอง | String | Booking.com, Agoda, Direct Web |
| channel_type | หมวดหมู่ของช่องทางเพื่อใช้จัดกลุ่มวิเคราะห์ | String | OTA, Direct, Corporate |
| commission_model | รูปแบบการคิดต้นทุน/ค่าคอมมิชชันของช่องทางนั้น ๆ | String | Percentage, Flat Fee, Net Rate, None |
| default_commission_rate | อัตราค่าคอมมิชชันมาตรฐาน | Float | 0.0 - 1.0 / 0.18, 0.15, 0.0 |
| contract_owner | ชื่อพนักงานฝ่ายขายที่เป็นผู้ดูแลสัญญาช่องทางนี้ | String | Sales_A, Sales_B |

---

### Table 3: `dim_rate_codes` 
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| rate_code_id | รหัสอ้างอิงประเภทราคา (Unique ID / PK) | String | RC_RACK, RC_PROMO, RC_CORP |
| rate_name | ชื่อเรียกของแพ็กเกจราคา | String | Standard Rack Rate, Promotional Discount |
| is_commissionable| เงื่อนไขระบุว่าราคานี้ต้องนำไปคำนวณหักค่าคอมมิชชันหรือไม่ | Boolean | True, False |

---

### Table 4: `fact_marketing_spend`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| spend_id | รหัสอ้างอิงรายการใช้จ่าย (Unique ID / PK) | String | SP_0001, SP_0002 |
| spend_date | วันที่ลงบันทึกค่าใช้จ่าย (ตัดรอบ 23:59:59 ของทุกวัน) | Datetime | 2025-01-01 23:59:59 |
| channel_id | รหัสช่องทางที่ทำการโปรโมต (FK ไปยัง dim_channels) | String | CH_03 |
| platform | แพลตฟอร์มที่ใช้ยิงโฆษณาออนไลน์ | String | Google Ads, Facebook |
| cost_amount | จำนวนเงินค่าโฆษณาที่จ่ายไปในวันนั้น (บาท) | Float | ค่าที่มากกว่าหรือเท่ากับ 0 เช่น 1540.25, 850.50 |
| clicks | จำนวนคลิกที่ได้รับกลับมาจากโฆษณา | Integer | ค่าที่มากกว่าหรือเท่ากับ 0 เช่น 120, 45 |

