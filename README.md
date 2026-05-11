# The Azure Stay: High Distribution Costs Problem

## Data Analytics Project Canvas
<img width="1920" height="1080" alt="CP372_Project_Canvas (1)" src="https://github.com/user-attachments/assets/221e84aa-8f4a-4ee8-a6df-fedf16bbf256" />

## Problem Statement / Background & Pain Point
- Background: เจ้าของโรงแรมอิสระขนาดกลางชื่อ The Azure Stay พบว่ากำไรไม่ได้เพิ่มขึ้นเลย แม้ว่าอัตราการเข้าพักจะอยู่ในระดับที่น่าพึงพอใจก็ตาม ซึ่งจากการที่วิเคราะห์สาเหตุของปัญหาพบว่าปัจจุบันโรงแรมมีการพึ่งพาช่องทาง Online Travel Agencies (OTAs) เช่น Agoda หรือ Booking.com ทำให้ต้องแบกรับค่าคอมมิชมิชั่นในอัตราที่สูง
- Problem Statement: ต้นทุนการจัดจำหน่ายสูง (ความสามารถในการทำกำไรของช่องทาง): คุณขายห้องพักได้ แต่ต้องจ่ายค่าคอมมิชชั่นจำนวนมากให้กับบุคคลที่สาม (OTA เช่น Expedia/Booking.com) คุณจำเป็นต้องระบุว่าช่องทางใดที่ทำกำไรได้จริง ไม่ใช่แค่ช่องทางที่สร้างปริมาณการขายเท่านั้น

## SMART Objectives / Value Propositions
การปรับปรุงโครงสร้างช่องทางการจัดจำหน่าย (Channel Mix) ของโรงแรม The Azure Stay เพื่อเพิ่มความสามารถในการทำกำไร โดยใช้ข้อมูลจากปี 2025 เป็นพื้นฐาน เป้าหมายคือการดำเนินการตามกลยุทธ์ใหม่และเห็นผลลัพธ์ภายใน 2 ไตรมาสข้างหน้า โดยมุ่งเน้นไปที่การลดสัดส่วนการพึ่งพา OTAs ที่มีต้นทุนค่าคอมมิชชันสูง และผลักดันยอดการจองผ่านช่องทางตรง (Direct Web/Walk-in) ให้เติบโตขึ้น 15% เมื่อเทียบกับปีที่ผ่านมา ผ่านการย้ายงบประมาณไปลงทุนในแคมเปญการตลาดดิจิทัลที่ควบคุมต้นทุนได้ดีกว่า ซึ่งแนวทางนี้จะนำไปสู่การลดต้นทุนการจัดหาลูกค้า (Cost of Acquisition, COA) และยกระดับรายได้สุทธิต่อห้องพัก (Net ADR)

โดยมีเป้าหมายแบบ SMART ดังนี้:
- S - Specific (เฉพาะเจาะจง): ลดสัดส่วนปริมาณการจองผ่าน OTA ลง และเพิ่มสัดส่วนการจองผ่านช่องทางตรง (Direct Web/Walk-in) ให้เพิ่มขึ้น 15% พร้อมทั้งยกระดับ Net RevPAR โดยรวม
- M - Measurable (วัดผลได้): ติดตามประสิทธิภาพโดยมุ่งเน้นที่การลด Cost of Acquisition (COA) % ให้น้อยลง และเพิ่ม Net ADR (Average Daily Rate หลังหักค่าคอมมิชชัน) ให้สูงขึ้น
- A - Achievable (ทำได้จริง): สามารถทำได้โดยการนำงบประมาณค่าคอมมิชชันบางส่วนไปเพิ่มเป็น Marketing Spend เพื่อดึงดูดทราฟฟิกเข้าสู่ Direct Web รวมถึงการสร้าง Rate Code แบบพิเศษ เพื่อจูงใจลูกค้าโดยตรง
- R - Relevant (สอดคล้องกับเป้าหมายหลัก): การเพิ่มความสามารถในการทำกำไรของช่องทาง (Channel Profitability) อย่างยั่งยืน โดยใช้วิธีบริหารต้นทุนช่องทางแทนการลดราคาห้องพักจนเสีย Brand Positioning
- T - Time-bound (มีกรอบเวลาชัดเจน): ดำเนินการปรับเปลี่ยนกลยุทธ์ช่องทางการจัดจำหน่ายและตั้งเป้าให้บรรลุผลสำเร็จ (เพิ่มสัดส่วน Direct Web 15% จากการลดการพึ่งพาช่องทาง OTA) ภายใน 6 เดือน (หรือ 2 ไตรมาสข้างหน้า)

## Questions / Hypothesis

### Bussiness Questions
1. ช่องทางใด (Booking Channel) มี Net ADR และ Net RevPAR สูงที่สุดและต่ำที่สุดเมื่อเทียบตลอดทั้งปี 2025?
2. Cost of Acquisition (COA) % ของช่องทาง Direct Web คุ้มค่ากว่าการเสียค่าคอมมิชชัน 15-18% ให้ OTA หรือไม่?
3. อัตราการยกเลิก (Cancellation Rate) และ No-Show บนช่องทางที่มีคอมมิชชันสูง (OTA) สูงกว่าช่องทาง Direct หรือไม่?
4. ลูกค้าเก่าที่กลับมาพักซ้ำ (Returning Guests) มีพฤติกรรมการจองอย่างไร? เรายังคงต้องเสียค่าคอมมิชชันให้กับ OTA สำหรับลูกค้ากลุ่มที่รู้จักแบรนด์เราอยู่แล้วหรือไม่?

### Hypotheses
1. ช่องทาง Direct Web ให้อัตรากำไรสุทธิต่อห้อง (Net ADR) สูงที่สุด แม้จะมีการทำโปรโมชัน (Rate Code: RT_PROMO) ลดราคาหน้าเว็บก็ตาม เนื่องจากไม่ต้องเสีย Commission แบบ Percentage
2. ค่าใช้จ่ายด้านการตลาด (Marketing Spend) บน Ads มี ROI (Return on Investment) และช่วยลด COA % ได้ดีกว่าการยอมจ่ายค่าคอมมิชชันแบบ Flat Rate หรือ Percentage ให้กับ OTA
3. ช่องทาง OTA มีอัตรา Cancel/No-Show สูงกว่า ทำให้โรงแรมเสียโอกาส (Opportunity Cost) ในการขายห้องที่ว่างให้ช่องทางที่กำไรสูงกว่า
4. ลูกค้าเก่าส่วนใหญ่ยังคงพึ่งพาช่องทาง OTA ในการจองห้องพัก (High OTA Dependency) ซึ่งทำให้โรงแรมสูญเสียกำไรจากค่าคอมมิชชันโดยไม่จำเป็น (Revenue Leakage)
5. ในช่วง High Demand Dates (Daily OCC มากกว่าหรือเท่ากับ 90 %) สัดส่วนการจองห้องพักส่วนใหญ่ยังคงมาจากช่องทาง OTA

## Key Metrics / Attributes
1. Key Metrics 
    - Net ADR : รายได้เฉลี่ยต่อห้องพักที่ขายได้ หลังจากหักลบค่าคอมมิชชันแล้ว
    - Net RevPAR : รายได้เฉลี่ยต่อห้องพักทั้งหมดที่มี (รวมห้องว่าง) หลังจากหักลบค่าคอมมิชชันแล้ว
    - Total Net Room Revenue : รายได้สุทธิรวมทั้งหมดจากค่าห้องพัก หลังจากหักลบค่าคอมมิชชันแล้ว
    - Cost of Acquisition (COA) % : สัดส่วนเปอร์เซ็นต์ของต้นทุนการได้มาซึ่งลูกค้า (ค่าคอมมิชชัน + ค่าการตลาด) เมื่อเทียบกับรายได้รวม
    - Total Acquisition Cost : ต้นทุนรวมทั้งหมดที่เกิดขึ้นเพื่อให้ได้ลูกค้ามา (ผลรวมของค่าคอมมิชชันและค่าใช้จ่ายทางการตลาด)
    - Total Bookings : จำนวนรายการจองห้องพักทั้งหมด
    - Total Rooms Sold : จำนวนห้องพักทั้งหมดที่ถูกขายและเข้าพักจริง
    - % Share of Bookings : สัดส่วนเปอร์เซ็นต์ของจำนวนการจอง (ใช้เพื่อเปรียบเทียบขนาดตลาดของแต่ละช่องทางหรือกลุ่มลูกค้า)
    - Cancellation Rate % : สัดส่วนเปอร์เซ็นต์ของรายการจองที่ถูกยกเลิก (Status = Cancelled)
    - No-Show Rate % : สัดส่วนเปอร์เซ็นต์ของรายการจองที่ลูกค้าไม่มาแสดงตัวในวันเข้าพัก (Status = No-Show)
    - Opportunity Cost : ต้นทุนค่าเสียโอกาส คำนวณจากรายได้ห้องพักรวมที่หายไปจากรายการที่ถูกยกเลิกหรือ No-Show
    - Total Commission Cost : จำนวนเงินค่าคอมมิชชันรวมทั้งหมดที่ต้องจ่ายให้กับช่องทางการจัดจำหน่าย
    - ROI Multiply : อัตราผลตอบแทนจากการลงทุนที่แสดงเป็นตัวคูณ (รายได้รวมคิดเป็นกี่เท่าของต้นทุนการได้มาซึ่งลูกค้า)

2. Key Attributes
    - channel_name : ชื่อของช่องทางการจัดจำหน่าย (เช่น Booking.com, Expedia, Direct Web)
    - channel_type : หมวดหมู่ของช่องทางการจัดจำหน่าย (เช่น OTA, Direct, Wholesale)
    - rate_code_id / rate_name : รหัสและชื่อของแพ็กเกจราคาหรือโปรโมชันที่ลูกค้าเลือกใช้ (เช่น RT_MEMBER, RT_PROMO)
    - check_in_date : วันที่ลูกค้ามีกำหนดการเข้าพัก (ใช้สำหรับจัดกลุ่มข้อมูลรายเดือน รายไตรมาส หรือรายปี)
    - spend_date : วันที่เกิดการจ่ายเงินค่าโฆษณาทางการตลาด (ใช้สำหรับวิเคราะห์ร่วมกับช่วงเวลาที่มีคนเข้าพัก)
    - platform : แพลตฟอร์มหรือช่องทางที่ใช้ยิงโฆษณา (เช่น Google Ads, Facebook)
    - segment_name : ประเภทกลุ่มลูกค้าที่จองเข้ามา (เช่น Leisure, Corporate, Group)
    - room_type_name : รูปแบบหรือประเภทของห้องพัก (เช่น Standard Queen, Suite)
    - status : สถานะปัจจุบันของการจองนั้น ๆ (เช่น Confirmed, Checked-Out, Cancelled, No-Show)
    - Day of Week : วันในสัปดาห์ (ใช้สำหรับวิเคราะห์เปรียบเทียบพฤติกรรมระหว่างวันธรรมดา Weekday และวันหยุดสุดสัปดาห์ Weekend)

## Data Dictionary
### Table 1: `fact_bookings`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| booking_id | Unique identifier for the reservation | Nominal | e.g., RES-10023 |
| guest_id | Unique identifier for the guest | Nominal | e.g., G-5021 |
| channel_id | Links to dim_channels | Nominal | e.g., CH_01 |
| room_type_id | Foreign key linking to the Room Type dimension | Nominal | e.g., RT_01 |
| rate_code_id | Links to dim_rate_codes | Nominal | e.g., RT_CORP |
| segment_id | Foreign key linking to the Customer Segment dimension | Nominal | e.g., CORP |
| booking_date | The date the reservation was made | Interval (Date) | <= check_in_date (e.g., 2024-01-15) |
| check_in_date | The scheduled arrival date | Interval (Date) | >= booking_date (e.g., 2024-02-01) |
| check_out_date | The scheduled departure date (Stay calculation strictly excludes this date) | Interval (Date) | > check_in_date (e.g., 2024-02-03) |
| gross_room_revenue | Total revenue paid by the guest (before commission) | Ratio (Continuous) | >= 0.00 (e.g., 500.00) |
| commission_amount | The calculated cost paid to the channel for this specific booking | Ratio (Continuous) | >= 0.00 (e.g., 75.00) |
| net_room_revenue | gross_room_revenue - commission_amount | Ratio (Continuous) | >= 0.00 (e.g., 425.00) |
| status | Status of booking | Nominal | 'Confirmed', 'Cancelled', 'Checked-Out', 'No-Show' |
| adults_count | Number of adults | Ratio (Discrete) | >= 1 (e.g., 2) |
| children_count | Number of children | Ratio (Discrete) | >= 0 (e.g., 1) |
| number_of_rooms | Number of rooms booked in this specific reservation | Ratio (Discrete) | >= 1 (e.g., 1) |
| ancillary_revenue | Revenue generated from extras (e.g., Spa, F&B) to calculate true Cost of Acquisition | Ratio (Continuous) | >= 0.00 (e.g., 150.00) |

---

### Table 2: `dim_channels`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| channel_id | Unique ID | Nominal | e.g., CH_01 |
| channel_name | Name | Nominal | e.g., 'Booking.com', 'Expedia' |
| channel_type | Category for cost analysis | Nominal | 'OTA', 'Direct', 'Wholesale' |
| commission_model | Type of cost structure | Nominal | 'Percentage', 'Flat Fee', 'Net Rate' |
| default_commission_rate | The standard % fee | Ratio (Continuous) | 0.00 to 1.00 (e.g., 0.15) |
| contract_owner | The internal sales manager responsible for this relationship | Nominal | e.g., 'John Doe' |
| default_flat_fee_amount | The standard flat fee amount charged per booking (for Flat Fee model) | Ratio (Continuous) | >= 0.00 (e.g., 5.00) |

---

### Table 3: `dim_rate_codes`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| rate_code_id | Unique ID | Nominal | e.g., RT_CORP |
| rate_name | Name of the rate | Nominal | e.g., 'Corporate Flat Rate' |
| description | Description of inclusions | Nominal | e.g., 'Includes Breakfast & Wifi' |
| is_commissionable | If False, the channel usually takes its cut before sending you the money | Nominal (Binary) | True, False |

---

### Table 4: `fact_marketing_spend`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| spend_id | Unique ID | Nominal | e.g., SP_001 |
| channel_id | Links to dim_channels (specifically the Direct Website channel) | Nominal | e.g., CH_DIRECT |
| spend_date | The date the money was spent | Interval (Date) | <= Current Date (e.g., 2024-01-01) |
| platform | Where the ad ran | Nominal (Binary) | e.g., 'Google Ads', 'Facebook' |
| cost_amount | The amount spent | Ratio (Continuous) | >= 0.00 (e.g., 500.00) |
| clicks | Number of clicks generated | Ratio (Discrete) | >= 0 (e.g., 1500) |

---

### Table 5: `dim_guests`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| guest_id | Unique ID | Nominal | e.g., G-5021 |
| full_name | Full name of guest | Nominal | e.g., 'Jane Smith' |
| nationality | Nationality of the guest | Nominal | e.g., 'TH', 'US', 'UK' |
| guest_type | Guest type classification | Nominal | 'New Guest', 'Returning Guest' |

---

### Table 6: `dim_segments`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| segment_id | Unique ID | Nominal | e.g., CORP, FIT, GRP |
| segment_name | Customer group name | Nominal | 'Corporate', 'Leisure', 'Group', 'Wholesaler' |
| segment_category | Main category | Nominal | 'B2B', 'B2C' |
| description | Details of the terms and conditions for this customer group | Nominal | e.g., 'Special corporate rate for partnered companies' |

---

### Table 7: `dim_room_types`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| room_type_id | Unique ID | Nominal | e.g., RT_01 |
| room_type_name | Room type name | Nominal | 'Standard', 'Deluxe', 'Suite' |
| base_capacity | Standard number of people staying | Ratio (Discrete) | >= 1 (e.g., 2) |
| total_inventory_count | The total physical number of rooms available for this specific room type | Ratio (Discrete) | >= 1 (e.g., 50) |

---

### Table 8: `dim_date`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| date | Specific calendar date | Interval (Date) | e.g., 2024-02-01 |
| is_holiday | Indicates if the date is a public holiday | Nominal (Binary) | True, False |

---

### Table 9: `fact_daily_inventory`
| Attribute | Description | Data Type | Valid Range / Example |
| :--- | :--- | :--- | :--- |
| date | Calendar date linking to dim_date (PK part 1) | Interval (Date) | e.g., 2024-02-01 |
| room_type_id | Links to dim_room_types (PK part 2) | Nominal | e.g., RT_01 |
| available_rooms | Number of rooms available for sale on this date | Ratio (Discrete) | >= 0 and <= total_inventory_count (e.g., 48) |
| out_of_order_rooms | Number of rooms blocked for maintenance | Ratio (Discrete) | >= 0 and <= total_inventory_count (e.g., 2) |

## Analysis/Model
* Cost of Acquisition (COA) Modeling: สร้างโมเดลคำนวณต้นทุนการได้มาซึ่งลูกค้า โดยนำค่า Commission (OTA) มาเปรียบเทียบกับ Marketing Spend (Google Ads/Facebook) ที่ลงไปกับช่องทาง Direct Web เพื่อหาว่าแบบไหนคุ้มค่า (ROI) กว่ากัน
* Guest Loyalty & Channel Market Share (การวิเคราะห์สัดส่วนการตลาดตามประเภทลูกค้า): วิเคราะห์พฤติกรรมของลูกค้า (Guest Type: New Guest vs. Returning Guest) จากตาราง dim_guests ว่ามีการเลือกใช้ช่องทางการจอง (Channel Type) แบบใด โดยคำนวณออกมาเป็น % Market Share ของจำนวน Booking ทั้งหมด
* Demand Pacing & Daily OCC Curve (การวิเคราะห์ความหนาแน่นของความต้องการพักอาศัย): จำแนกช่วงเวลาออกเป็น Regular Demand และ High Demand โดยพิจารณาจาก Daily Occupancy (OCC) ที่เกิดขึ้นจริงในแต่ละวัน (Stay Date) และนำมาแยกสัดส่วนตาม Channel Type เพื่อดูว่าในวันที่ความต้องการสูง ห้องพักถูกกินสัดส่วนโดยช่องทางใด

## Findings and Insight
### Dashboard (Overview)
<img width="1600" height="900" alt="Dashboard" src="https://github.com/user-attachments/assets/0040b46c-15bb-4a78-90c9-302f75885232" />

### Net ADR & Net RevPAR vs. Booking Channels
<img width="1305" height="858" alt="Hypothesis1 1" src="https://github.com/user-attachments/assets/71e37ac9-6523-4934-bad1-c9ff05b826ed" />
<br>

> ช่องทาง Walk-in และ Direct Web เป็นช่องทางที่ไม่มีตัวกลางคอยหักค่าคอมมิชชัน ทำให้โรงแรมเก็บกำไรสุทธิต่อคืน (NetADR) ได้เต็มเม็ดเต็มหน่วยที่ 119.77 และ 121.58 ดอลลาร์ ในขณะที่ Expedia มี Net ADR ต่ำที่สุดเพียง 104.20 ดอลลาร์เพราะโมเดลของ OTA เจ้านี้มีการเก็บค่าคอมมิชชันสูงถึง 18% ที่ลดทอนความสามารถในการทำกำไรสุทธิต่อคืนของโรงแรมอย่างมีนัยสำคัญ

### Distribution Channel Performance: Daily Net Room Revenue Volume vs. Net ADR
<img width="1627" height="841" alt="Hypothesis1 2" src="https://github.com/user-attachments/assets/45baa4b9-dba7-446e-9fd6-ac0467ba8809" />

### Distribution Channel Performance: Gross Room Revenue Volume vs. Net RevPAR
<img width="1627" height="841" alt="Hypothesis1 3" src="https://github.com/user-attachments/assets/a9e32792-b335-452f-8c74-e945837ced3c" />
<br>

> ถึงแม้ Booking.com จะกำไรสุทธิต่อคืน (Net ADR) เพียง 108.77 ดอลลาร์ แต่ด้วยปริมาณการขายที่ทำยอดไปถึง 9,468 ห้อง ทำให้สามารถขับเคลื่อน Net RevPAR หรือรายได้รวมเมื่อเทียบกับความจุโรงแรมออกมาได้สูงที่สุดที่ 31.75 ดอลลาร์ต่อห้อง ในทางกลับกัน Corporate GDS แม้จะมีกำไรต่อคืนดีมาก แต่ฐานลูกค้ายังแคบและจำนวนคืนเข้าพักน้อย ทำให้ทำ Net RevPAR ได้ต่ำที่สุดเพียง 7.35 ดอลลาร์ต่อห้อง

> ช่องทาง Walk-in สร้างสถิติที่ดูเหมือนจะขัดแย้งกันเอง (Paradox) โดยเป็นช่องทางที่สร้าง Net ADR ได้สูงที่สุดเป็นอันดับ 1 ที่ 121.58 ดอลลาร์ แต่ในขณะเดียวกันกลับมีปริมาณคืนเข้าพัก (Total Rooms Sold) ต่ำเกือบที่สุดที่ 1,647 คืน (สูงกว่า Corporate GDS เพียงช่องทางเดียว) และดึงค่า Net RevPAR ลงไปจมอยู่ท้ายตารางที่ 7.79 ดอลลาร์

### Net ADR Distribution by Channel Type and Rate Category
<img width="1367" height="841" alt="Hypothesis1 4" src="https://github.com/user-attachments/assets/3cfce410-3755-4ddc-a11c-5a091369b6d0" />
<br>

> การยอมเสีย Margin เพื่อลดราคาให้ลูกค้า 10% หน้าเว็บไซต์ตัวเอง ได้ NetADR ที่ 119.77 ดอลลาร์ ซึ่งน้อยกว่าการฝืนขายราคาเต็มบน OTA แล้วถูกหักค่าคอมมิชชัน 15-18% แม้จะเป็น ราคาเต็มไม่ผ่าน Promotion ก็ตาม บน Booking.com ได้ Net ADR เพียง 111.73 ดอลลาร์

> The Double-Hit Margin Compression: สาเหตุที่การนำโปรโมชันไปลงบน OTA เป็นเรื่องอันตรายต่อกำไร เพราะโรงแรมจะโดนผลกระทบ 2 ชั้น คือ 1) ฐานราคาถูกกดให้ต่ำลงจากส่วนลด 10% และ 2) ถูก OTA คิดเปอร์เซ็นต์คอมมิชชันทับลงไปอีก ทำให้ Net ADR ของ Agoda และ Expedia ร่วงลงไปเหลือเพียง 96-98 ดอลลาร์ (หายไปกว่า 20 ดอลลาร์ต่อคืน เมื่อเทียบกับ Direct Web)

### Cost of Acquisition (COA%) Analysis by Booking Channel
<img width="1367" height="858" alt="Hypothesis2 1" src="https://github.com/user-attachments/assets/ea91e15b-c8c9-4912-b82f-51890a426474" />
<br>

> การใช้จ่ายงบการตลาดไปกับโฆษณา (Google Ads / Facebook) เพื่อดึงคนเข้า Direct Web ใช้เงินเพียง ~19,470 ดอลลาร์ แต่สร้างยอดขายได้เกือบ 7 ดอลลาร์ คิดเป็นต้นทุน (COA) เพียง 2.82% ในขณะที่การได้ยอดขายจาก Expedia ต้องเสีย COA ถึง 18%

### Cancellation and No-Show Volume: OTA vs. Direct
<img width="1366" height="858" alt="Hypothesis3 1" src="https://github.com/user-attachments/assets/057ab9b1-f11e-4ae5-a77b-85f93c010b46" />
<br>

> ช่องทาง OTA มียอดจองที่สูญเปล่า (Cancelled และ No-Show) รวมสูงถึง 1,160 รายการ ซึ่งมากกว่าช่องทาง Direct กว่า 2.6 เท่า

### Net Opportunity Loss by Channel
<img width="1366" height="841" alt="Hypothesis3 2" src="https://github.com/user-attachments/assets/42858fc2-9bb8-4e77-8afb-fe7bb11f8079" />
<br>

> ค่าเสียโอกาสสุทธิ (Net Opportunity Loss) ที่ทำให้รายได้โรงแรมสูญเสียรายได้จากการยกเลิกนั้น กระจุกตัวอยู่ที่ช่องทาง Booking.com (-3,864 $) เป็นหลัก ในขณะที่ OTA อื่น ๆ อย่าง Agoda และ Expedia โรงแรมยังสามารถนำห้องไปรีเซลเพื่อดึงรายได้กลับมาได้

### Loss Rooms Night vs. Revenue Recovery by Channel
<img width="1367" height="841" alt="Hypothesis3 3" src="https://github.com/user-attachments/assets/098efc54-89f3-492c-92db-f5a979e89ee3" />
<br>

> แม้ Expedia จะมียอดการยกเลิกถึง (1,930 ห้อง-คืน) แต่ Direct Web คือช่องทางที่คุ้มค่ากว่า เพราะสร้างรายได้กู้คืนได้ใกล้เคียงกัน แม้จะมีปริมาณห้องที่สูญเสียไปน้อยกว่าถึง 295 ห้อง-คืนก็ตาม

### Booking Share (%) by Guest Type and Channel
<img width="1367" height="841" alt="Hypothesis4" src="https://github.com/user-attachments/assets/55ce20bf-378c-4f6f-91ce-6025e7223df2" />
<br>

> สัดส่วนการจองผ่าน OTA แทบจะไม่ต่างกันเลย ระหว่างลูกค้าใหม่ (70.05%) และลูกค้าเก่า (70.55%) ซึ่งสะท้อนให้เห็นว่าแม้ลูกค้าจะเคยมาพักและรู้จักโรงแรมของเราแล้ว แต่พวกเขาก็ยังเลือกที่จะกลับไปจองผ่านช่องทาง OTA เหมือนเดิม แทนที่จะเปลี่ยนมาจองตรงกับทางโรงแรม (Direct)

> โดยปกติแล้ว ลูกค้าเก่า (Returning Guest) ควรจะมีสัดส่วนการจองตรง (Direct) ที่สูงกว่าลูกค้าใหม่ เนื่องจากมีความเชื่อมั่นในแบรนด์ของเราแล้ว แต่จากกราฟจะเห็นว่าสัดส่วนการจองตรงของลูกค้าเก่า (24.51%) กลับน้อยกว่า ลูกค้าใหม่ (24.87%) แม้จะเพียงเล็กน้อย แต่สิ่งนี้ก็ชี้ให้เห็นว่าโรงแรมยังคงขาดกลยุทธ์การทำ Retention Marketing

### Market Share (%) by Channel Type vs. Demand Type
<img width="1367" height="858" alt="Hypothesis5 1" src="https://github.com/user-attachments/assets/c0febf8c-bb1f-4f19-9132-7d878b547992" />
<br>

> โรงแรมมีวันที่ขายดีมาก (Daily OCC มากกว่าหรือเท่ากับ 90%) สูงถึง 214 วันในหนึ่งปี แต่ในวันเหล่านั้น โรงแรมก็ยังปล่อยให้ OTA เข้ามาแย่งสัดส่วนห้องไปถึง 70.69% โดยยอม Net ADR แค่ 106.73 ดอลลาร์ ทั้ง ๆ ที่ถ้าขายผ่านช่องทาง Direct จะได้กำไรสูงถึง 120.12 ดอลลาร์

> "ขายดี แต่ขาดทุนกำไร" (Leaving Money on the Table): ในวัน High Demand (เช่น เทศกาล คอนเสิร์ต หรือวันหยุดยาว) เป็นวันที่ "ยังไงห้องก็ขายหมดอยู่แล้ว" การปล่อยห้องให้ OTA ขายในวันเหล่านี้ คือการเสียค่าคอมมิชชันฟรีๆ โดยไม่จำเป็น (Cannibalization)

## Recommendations
ACTION 1 (H1 & H2)
* ต้นทุน COA ที่ 2.82% ของการยิงแอดถือว่า "ถูกมาก" เมื่อเทียบกับค่า Commission ของช่องทาง OTA ดังนั้นโรงแรมควรเพิ่มงบการโฆษณาบน Google Ads หรือ Facebook Ads โดยเน้นไปที่แคมเปญ "Brand Search" (คนที่ค้นหาชื่อโรงแรม) เพื่อลดจำนวนลูกค้ากลุ่มที่นิยมจองผ่านลิงก์ของ OTA ที่นิยมซื้อ Ads ดักชื่อโรงแรมเราไว้

* เราสามารถ "ลดราคาการจองผ่านหน้าเว็บของเราเอง (Direct Web) ให้ถูกกว่าช่องทาง OTA" ได้ (เช่น ลด 12 ถึง 15%) การทำแบบนี้จะส่งผลให้ลูกค้ารู้สึกคุ้มค่าและตัดสินใจจองตรงในทันที ส่วนโรงแรมก็ยังมี Net ADR ที่สูงกว่า หรืออย่างน้อยก็เทียบเท่ากับการขายผ่านช่องทาง OTA

ACTION 2 (H3)
* Automated Post-Stay CRM: ทันทีที่ลูกค้า Checked-Out ระบบต้องส่ง Email หรือ SMS ขอบคุณ พร้อมแนบ "Secret Promo Code" สำหรับการจองครั้งถัดไปผ่าน Direct Web เท่านั้น
* Front Desk Conversion: อบรมพนักงานต้อนรับ (Front Office) ว่าในขั้นตอน Check-out ให้เชิญชวนลูกค้าสมัคร Line OA / Member ของโรงแรม แลกกับสิทธิพิเศษ ซึ่งเป็น Touchpoint สุดท้ายที่สำคัญในการแย่งชิงลูกค้ามาจาก OTA

ACTION 3 (H4)
* เริ่มทำ Allotment Cut-off: ให้ทีม Revenue Manager มอนิเตอร์ยอดจองล่วงหน้า (On-the-books) วันไหนที่ยอดทะลุ 70-80% ให้ทำการ "ปิดการขายบน OTA (Close Out)" ทันที เพื่อเก็บห้อง 20% สุดท้ายไว้ขายบนเว็บโรงแรมเองหรือรับ Walk-in ในราคาเต็ม

## Contributors
* Pacharadanai Kurakanok (66102010145)
* Sirayuth Chotithammaporn (66102010153)
* Yanapatt Pankaseam (66102010236)
