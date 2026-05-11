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
<img width="640" height="360" alt="CPP_Channel Profitability Analysis" src="https://github.com/user-attachments/assets/f1bb0cb6-fcd1-417f-80d2-55e6cbfa73d8" />

* ผลลัพธ์ชี้ให้เห็นว่าโรงแรมมีวันที่ขายดีมาก (Occ > 90%) สูงถึง 214 วันในหนึ่งปี แต่ในวันเหล่านั้น โรงแรมก็ยังปล่อยให้ OTA เข้ามากินสัดส่วนห้องไปถึง 70.69% โดยยอมรับรายได้สุทธิแค่ 106.73 ดอลลาร์ต่อคืน ทั้งๆ ที่ถ้าขายผ่านช่องทาง Direct จะได้กำไรสูงถึง 120.12 ดอลลาร์ต่อคืน

<img width="568" height="348" alt="CPP_Channel Profitability Analysis (1)" src="https://github.com/user-attachments/assets/0a069ba9-acce-47b9-bd3f-bbc61cfdd817" />

* ลูกค้าเก่า (Returning Guests) ยังคงพึ่งพา OTA สูงถึง 70.55% ซึ่งแทบไม่ต่างจากพฤติกรรมของลูกค้าใหม่ (70.05%)

<img width="580" height="348" alt="CPP_Channel Profitability Analysis (2)" src="https://github.com/user-attachments/assets/c9d229ef-f36b-4523-89f5-09b0d9450cfb" />

* การใช้จ่ายงบการตลาดไปกับโฆษณา (Google Ads / Facebook) เพื่อดึงคนเข้า Direct Web ใช้เงินเพียง ~19,470 ดอลลาร์ แต่สร้างยอดขายได้เกือบ 7 ดอลลาร์ คิดเป็นต้นทุน (COA) เพียง 2.82% ในขณะที่การได้ยอดขายจาก Expedia ต้องเสีย COA ถึง 18%

<img width="594" height="354" alt="CPP_Channel Profitability Analysis (3)" src="https://github.com/user-attachments/assets/c923dbb2-f538-4e6f-b1eb-3398dd6ea147" />

* การยอมเสีย Margin เพื่อลดราคาให้ลูกค้า 10% หน้าเว็บไซต์ตัวเอง (RT_PROMO ได้ Net ADR 119.77) เจ็บตัวน้อยกว่า การฝืนขายราคาเต็มบน OTA แล้วถูกหักค่าคอมมิชชัน 15-18% (RT_RACK บน Booking.com ได้ Net ADR 111.73)

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
