>"เฮ้อ เมื่อไหร่จะได้กลับบ้านสักทีนะ หมาแมวรอจะแย่ละ"

> "ตกลงมันไม่มีรถสายนี้กันหรือไงหะ" หรือ "พอจะขึ้นก็ไม่มา พอไม่ขึ้นนี้มีเพียบเลย"

ผู้คนไม่น้อยที่ต้องอาศัยรถโดยสารประเภทต่างๆคงมีความคิดเช่นนี้ในระหว่างรอรถโดยสารที่จะกลับบ้านหรือเดินทางไปที่ต่างๆ แน่นอน ถ้าถนนมี 4 เลน แต่มีเลนของรถประจำทางแค่ 1 เลน คิดเป็น 25 % ของถนน

ถ้าสมมุติว่ามีรถทุกประเภทวิ่งอยู่ตลอดเวลา อัตรส่วนของรถจะต้องตรงกับอัตราส่วนของเลนในถนนไม่ใช่หรือไงกัน ถึงแม้จะมี application ต่างๆที่เกี่ยวกับรถประจำทางในกรุงเทพไม่ว่าจะให้ข้อมูลสายของรถประจำทางหรือเวลาออกจากท่า แต่ก็ไม่อาจทราบถึงปริยังเป็นปริศนากันอยู่ทุกว่าดวงจะไม่เจอหรือว่ามันมีน้อยจริงๆ แม้แต่สวรรค์ก็ไม่อาจทราบได้

เรามีรถที่จดทะเบียนในประเทศไทยเท่าไหร่กันแน่ มันช่างเยอะแยะเหลือกเกินทั้งที่บางทีบางบ้านจอดรถได้แค่คันเดียว หรือทำไมเวลาที่ไปเที่ยวต่างจังหวัดถึงพบรถส่วนตัวแบบ 4 ล้อ มากกว่ารถจักรยานยนต์ เราจึงนำมาเป็นหัวข้อในการทำ data analysis  

# จะเอาอะไรมาหาคำตอบ
เราใช้ open data ที่รัฐบาลยอมเปิดเผยจากเว็บไชต์ https://data.go.th/ จำนวนรถจดทะเบียน (สะสม) ณ วันที่ 31 ธันวาคม 2558

---

# ข้อมุลหยาบ (Raw Data)
### รถจดทะเบียนในภาคต่างๆ
![](/Result%20Graph/Total-Central.png)
![](/Result%20Graph/Total-East.png)
![](/Result%20Graph/Total-NEast.png)
![](/Result%20Graph/Total-North.png)
![](/Result%20Graph/Total-South.png)
![](/Result%20Graph/Total-West.png)

### รถจดทะเบียนในทุกจังหวัดดในประเทศไทย
![](/Result%20Graph/Total-All.png)

# อัตราส่วนรถโดยสาร (Bus) ต่อ รถส่วนตัว (Sedan)

Bus หมายถึง รถโดยสารประเภทต่างๆที่จดทะเบียน ณ กรมการขนส่งทางบกเมื่อปี 2558
Sedan หมายถึง รถยนต์ส่วนบุคคลประเภทต่างๆ ที่ขึ้นทะเบียนต่อกรมขนส่งในปี 2558

สมมติว่าเราเพิ่งมาถึงป้ายรอรถประจำทางริมถนน
ถ้าอัตราส่วนของรถกับเวลาคงที่ใน 1 วินาที/1 วัน/1 เดือน/1 ปี แสดงว่าพอเราเดินมาถึงป้ายรอรถโดยสารประจำทางเราจะพว่า

###  ป้ายรถโดยสารทั้งอณาจักร คิดจากกราฟ Whole Kingdom ที่มีอัตราส่วนของ Bus:Sedan เป็น 1.9%  
เราจะพบรถโดยสารใดๆ 1 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 86,400 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 31,536,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 0.99%  

### ป้ายรถโดยสารใดๆในกรุงเทพมหานคร คิดจากกราฟ Bangkok ที่มีอัตราส่วนของ Bus:Sedan เป็น 1.1%   
เราจะพบรถโดยสารใดๆ 1 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 86,400 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 31,536,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 0.99%  

### ป้ายรถโดยสารใดๆในส่วนภูมิภาค คิดจากกราฟ Regional ที่มีอัตราส่วนของ Bus:Sedan เป็น 2.6%   
เราจะพบรถโดยสารใดๆ 2 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 172,800 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 63,072,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 1.96%

### ป้ายโดยสารใดๆในภาคกลาง คิดจากกราฟ Central ที่มีอัตราส่วนของ Bus:Sedan เป็น 4.4%
![](/Result%20Graph/Central.png)

เราจะพบรถโดยสารใดๆ 4 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 345,600 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 126,144,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 3.99%

### ป้ายรถโดยสารใดๆในภาคอีสาน คิดจากกราฟ Eastern ที่มีอัตราส่วนของ Bus:Sedan เป็น 2.5%
![](/Result%20Graph/Eastern.png)

เราจะพบรถโดยสารใดๆ 2 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 172,800 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 63,072,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 1.96%

### ป้ายรถโดยสารใดๆในภาคเหนือ คิดจากกราฟ Northern ที่มีอัตราส่วนของ Bus:Sedan เป็น 1.8%  
![](/Result%20Graph/Northern.png)
เราจะพบรถโดยสารใดๆ 1 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 86,400 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 31,536,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 0.99%  

### ป้ายรถโดยสารใดๆในภาคเหนือ คิดจากกราฟ Northern Eastern ที่มีอัตราส่วนของ Bus:Sedan เป็น 1.8%  
![](/Result%20Graph/North%20Eastern.png)

เราจะพบรถโดยสารใดๆ 1 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 86,400 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 31,536,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 0.99%  

### ป้ายรถโดยสารใดๆในภาคตะวันตก คิดจากกราฟ Western ที่มีอัตราส่วนของ Bus:Sedan เป็น 2.8%   
![](/Result%20Graph/Western.png)

เราจะพบรถโดยสารใดๆ 2 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 172,800 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 63,072,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 3,153,600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 1.96%

### ป้ายรถโดยสารใดๆในภาคใต้ คิดจากกราฟ Southern ที่มีอัตราส่วนของ Bus:Sedan เป็น 3.6%   
![](/Result%20Graph/Southern.png)

เราจะพบรถโดยสารใดๆ 3 ครั้ง ต่อรถส่วนตัว 100 ครั้ง ใน 1 วินาที พบรถโดยสาร 259,200 ครั้ง พบรถส่วนตัว 8,640,000 ครั้ง ใน 1 วัน  

พบรถโดยสาร 94,608,000 ครั้ง ใน 1 ปี พบรถส่วนตัว 315,3600,000 ครั้ง ใน 1 ปี  

แสดงว่าเรามีโอกาสเจอรถโดยสารไม่ว่าจะเวลาใดก็ตามที่ป้ายรถโดยสารทั้งอาณาจักรเป็น 2.91%

จะเห็นได้ว่าภาคที่มีโอกาสพบรถโดยสารมากเป็นอันดับ 1 คือ ภาคกลาง เพราะเป็นที่รวมศูนย์กลางความเจริญของประเทศ ลำดับ 2 คือ ภาคใต้ เพราะมีจังหวัดหาดใหญ่ที่เป็นที่นิยมของภาคใต้ ลำดับที่ 3 คือส่วนภูมิภาค ภาคอีสาน และภาคตะวันตก

หรือการที่ภาคที่มีจังหวัดท่องเที่ยวก็มีอัตรส่วนของ Bus:Sedan น้อยเพราะว่าคนส่วนใหญ่นิยมใช้รถส่วนตัวหรือเป็นรถโดยสารที่ไม่ได้ขึ้นทะเบียนกับกรมขนส่ง  

สาเหตุของการที่มีรถโดยสารน้อย
- อาชีพคนขับรถโดยสารอาจไม่เป็นที่นิยม
- เพื่อความสมดุลของปริมาณรถในถนน
- ผู้คนไม่ชอบความลำบากในการโดยสาร
- ความไม่ไว้วางใจการขึ้นรถโดยสาร
- การที่มีรถส่วนตัวมาก
- ความรักสบาย
- นโยบายรถคันแรกตั้งแต่ ปี พ.ศ. 2554  
- ไม่มีกฏหมายจำกัดอายุการใช้งานรถ
- ค่านิยมของการมีรถ
- รอรถไฟฟ้าสาธารณะที่กำลังสร้าง

# 5 ลำดับรถที่ถูกจดทะเบียนในประเทศไทยในปี 2016
ภาคที่มีการจดทะเบียนรถมากที่สุดในปี 2016
![](/Result%20Graph/Top-Vehicle.png)

เป็นที่แน่นอนว่ากรุงเทพมีรถที่ถูกจดทะเบียนมากที่สุดเพราะมีการคมนาคมที่คับคั่ง มีถนนมากมายหลายเส้นทำให้เหมาะแก่การมีรถในครอบครอง รองลงมาเป็นภาคตะวันออกและภาคตะวันออกเฉียงเหนือ อาจเป็นเพราะสภาพภูมิประเทศที่เป็นที่ราบสูงสลับหุบเขา ทำให้ต้องใช้รถในการเดินทางเป็นส่วนมาก และรถส่วนมากที่นิยมจดทะเบียนอันดับ 1 คือรถจักรยานยนต์ อันดับ 2 คือรถส่วนตัว อันดับ 3 คือรถตู้และรถ Pic Up การที่มีรถจักรยานยนต์เป็นจำนวนมากมีสาเหตุจากราคาที่ถูกที่สุดในบรรดารถทั้งหมด ส่วนที่เหลือมีจุดประสงค์เพื่อความสะดวกสะบายหรือเพื่อใช้ในธุรกิจ

# อัตราส่วนของรถส่วนตัวกับรถจักรยานยนต์
กรุงเทพและภาคกลางมีถนนมากมายจึงทำให้เหมาะกับการใช้รถจักรยานยนต์จึง แต่ภาคตะวันตกมีอัตรส่วนของรถส่วนตัวกับรถจักรยานยนต์มากที่สุดเพราะสภาพภูมิประเทศอยู่ติดกับฝั่นเมียนมาร์เป็นทางตรงยาว

จึงเหมาะแก่การใช้รถส่วนตัวมากกว่ารถจักรยานยนต์ในการเดินทางที่ไกล

และภาคตะวันออกเฉียงเหนือที่มีอัตรส่วนของรถส่วนตัวกับรถจักรยานยนต์มากเป็นอันดับสองเพราะสภาพภูมิประเทศที่เป็นที่ราบสูงสลับหุบเขาทำให้รถส่วนตัวเหมาะแก่การใช้ในการเดินทางมากกว่า

# Team Members
|Name|Student ID|GitHub Username|
|-|-|-|
|Kunanon Srisuntiroj|59070022|@sagelga
|Thinnaphob Chaiyakhet|59070058|	@singleearkportraitphotography
|Napasin Hongngern|59070084|@tiltgod
|Pawin Thamroungthong|59070095|@Closesun
