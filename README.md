# DADS5001 Mini-Project

## Topic: ผลกระทบจากเศรษฐกิจทำให้อัตราเด็กเกิดใหม่ลดลงหรือไม่

By: Nithida Phookriangkrai (student id: 6420422004)

## Dataset
1. ประชากรเกิดใหม่ตั้งแต่ปี 2536-2564

    source: https://stat.bora.dopa.go.th/stat/statnew/statMenu/newStat/stat/

2. รายได้และรายจ่ายของทุกจังหวัดในประเทศไทย

    source: http://statbbi.nso.go.th/staticreport/page/sector/th/08.aspx

3. Consumer Price Index (CPI) ตั้งแต่ปี 2541-2564

    source: http://www.price.moc.go.th/th

4. GPP ตั้งแต่ปี 2556-2564

    source: https://www.nesdc.go.th/main.php?filename=gross_regional


## Question & Answer
1. จำนวนเด็กเกิดใหม่ที่ลดลงในประเทศไทย ส่วนมากเกิดที่ภาคใด 

    คำตอบ: อัตราการเกิดในภาคอีสานมีจำนวนสูงสุด และลดลงมากที่สุดเมื่อเปรียบเทียบกับจังหวัดอื่นๆ

2. จังหวัดที่มี %การเกิดใหม่ลดลงมากที่สุด 5 อันดับและน้อยที่สุด 5 อันดับคือจังหวัดอะไร

    คำตอบ: 

    - มากที่สุด 5 อันดับ คือ ชัยนาท อ่างทอง พังงา ตรัง และหนองคาย

    - น้อยที่สุด 5 อันดับ คือ เชียงใหม่ ยะลา ปทุมธานี แม่ฮ่องสอน และตาก (ตากเป็นจังหวัดเดียวที่มีเด็กเกิดใหม่เพิ่มขึ้น)

3. อัตราเด็กไทยเกิดใหม่ลดลง มีผลมาจากค่าใช้จ่ายที่สูงขึ้นหรือไม่ 

    คำตอบ: คาดว่าเป็นไปได้ แต่น่าจะมีปัจจัยอื่นๆร่วมด้วย เช่น วิกฤตอุทกภัยหรือเศรษฐกิจต่างๆ

4. จังหวัดที่ค่าครองชีพสูงจะมีอัตราการเกิดต่ำกว่าจังหวัดที่มีค่าครองชีพต่ำ

    คำตอบ: ไม่พบความสัมพันธ์ระหว่างค่าครองชีพกับ %เด็กเกิดใหม่

5. รายได้และรายจ่ายของคนในแต่ละจังหวัดส่งผลต่ออัตราการเกิด

    คำตอบ: คาดว่ามีความเกี่ยวข้อง เนื่องจากพบว่าภาคอีสานที่มันอัตราการเกิดลดลงมากที่สุด มีค่าเฉลี่ยรายได้และรายจ่ายใกล้เคียงกัน

6. GPP (มูลค่าการผลิตสินค้าและบริการขั้นสุดท้ายของจังหวัด) มีผลต่ออัตราการเกิดหรือไม่ 

    คำตอบ: ไม่พบความสัมพันธ์ระหว่าง GPP และอัตราการเกิด
    
## Challenge
1. ต้องรวบรวมข้อมูลจากหลายแหล่ง และนำมาประกอบเป็น file ที่ต้องใช้ เนื่องจากเว็บไซต์มาจากคนละแหล่ง ซึ่งแต่ละแหล่งนั้น แยกข้อมูลรายจังหวัด หรือแยกเป็นรายปี


2. เนื่องจากข้อมูลมีจำนวนปีที่ไม่เท่ากัน ทำให้เวลาจะเลือกวิเคราะห์ ต้องตัดเฉพาะจำนวนปีที่มีข้อมูลมาวิเคราะห์ เช่น การวิเคราะห์ที่ดูเป็นรายจังหวัด ต้องเริ่มปี 2554 เนื่องจากเพิ่มจังหวัดบึงกาฬเข้ามา


3. เนื่องจากข้อมูลเป็นภาษาไทย ทำให้ตอนแรกที่ plot graph ไม่สามารถอ่านตัวอักษรภาษาไทยได้ จึงต้องไป import font ภาษาไทย

## ขั้นตอน

1. Import library และ dataset ที่ต้องใช้

![Screen Shot 2565-10-14 at 22 38 41](https://user-images.githubusercontent.com/56344603/195886281-9654c6c6-e30e-45e3-81d3-87ee25500c82.png)

![Screen Shot 2565-10-14 at 22 39 43](https://user-images.githubusercontent.com/56344603/195886478-82206687-c983-47cf-9f28-22b90c0ca85b.png)

![Screen Shot 2565-10-14 at 22 40 41](https://user-images.githubusercontent.com/56344603/195886669-cfeb9cc9-04dd-4b6f-a15f-f890d6085cea.png)

<img width="837" alt="Screen Shot 2565-10-14 at 22 41 06" src="https://user-images.githubusercontent.com/56344603/195886735-d2129dc0-32b7-443f-808c-2b91678547e4.png">

<img width="744" alt="Screen Shot 2565-10-14 at 22 41 19" src="https://user-images.githubusercontent.com/56344603/195886782-880022c8-4de9-4ac2-b9f8-7f8997475ff7.png">

<img width="770" alt="Screen Shot 2565-10-14 at 22 41 45" src="https://user-images.githubusercontent.com/56344603/195886931-555d9c6d-074a-4def-973c-0214f3818837.png">

2. Prepare data (reshape data, join data)

เนื่องจาก raw data มีแค่ชื่อจังหวัด ไม่มีภาค จึงต้อง join ข้อมูล

<img width="303" alt="Screen Shot 2565-10-14 at 22 43 57" src="https://user-images.githubusercontent.com/56344603/195887268-6f37bb7a-f9d0-42e8-8d0a-198d266b6902.png">

<img width="692" alt="Screen Shot 2565-10-14 at 22 44 10" src="https://user-images.githubusercontent.com/56344603/195887310-27acc467-4859-4a13-9147-3c11729197bd.png">

รวม file รายได้และรายจ่ายไว้ใน table เดียวกัน

เนื่องจาก file รายได้และรายจ่ายมียอดรวมทั่วประเทศด้วย จึงต้องเลือก row ที่จะนำไปใช้

<img width="284" alt="Screen Shot 2565-10-14 at 22 44 56" src="https://user-images.githubusercontent.com/56344603/195887453-c0d74d73-f728-422b-8a8c-fce9cf74cf19.png">

<img width="381" alt="Screen Shot 2565-10-14 at 22 45 42" src="https://user-images.githubusercontent.com/56344603/195887592-a7b6f3ce-65b9-4b5e-ab3b-af2b5318ec3a.png">

<img width="291" alt="Screen Shot 2565-10-14 at 22 45 54" src="https://user-images.githubusercontent.com/56344603/195887637-bb9c9f6d-6062-4cf3-9dd7-0fa18eccbfd1.png">

<img width="389" alt="Screen Shot 2565-10-14 at 22 46 08" src="https://user-images.githubusercontent.com/56344603/195887684-d372c4e4-e222-49f7-a085-97b3e2dfc289.png">

<img width="889" alt="Screen Shot 2565-10-14 at 22 46 23" src="https://user-images.githubusercontent.com/56344603/195887723-8079e48a-2820-4558-b98f-74de33a234a9.png">

<img width="743" alt="Screen Shot 2565-10-14 at 22 46 43" src="https://user-images.githubusercontent.com/56344603/195887788-794c1a76-18c8-49c0-9721-af0943c5a17c.png">

## วิเคราะห์ข้อมูลเพื่อตอบคำถาม

1. จำนวนเด็กเกิดใหม่ทั้งประเทศ ช่วงเวลาตั้งแต่ปี พ.ศ. 2536 - 2564

<img width="291" alt="Screen Shot 2565-10-14 at 22 49 01" src="https://user-images.githubusercontent.com/56344603/195888252-ddfd84f8-ad12-46b1-9fee-1236562577de.png">

<img width="474" alt="Screen Shot 2565-10-14 at 22 49 18" src="https://user-images.githubusercontent.com/56344603/195888302-91ad427c-9618-4671-8c71-41c8381151af.png">

![image](https://user-images.githubusercontent.com/56344603/195888339-636af9cf-de6e-492f-8126-3c6a795a5b0a.png)

จะเห็นว่าจำนวนเด็กเกิดใหม่จะลดลงหลังจากมีเหตุการณ์สำคัญในประเทศไทย เช่น วิกฤตอุทกภัย 2538 หรือวิกฤตเศรษฐกิจต้มยำกุ้ง

2. จำนวนเด็กเกิดใหม่ในแต่ละภาค ช่วงเวลาตั้งแต่ปี พ.ศ. 2536 - 2564

<img width="776" alt="Screen Shot 2565-10-14 at 22 51 47" src="https://user-images.githubusercontent.com/56344603/195888786-eb11a0e0-5665-401c-8e5b-eef973c6e0c5.png">

<img width="401" alt="Screen Shot 2565-10-14 at 22 51 58" src="https://user-images.githubusercontent.com/56344603/195888822-7f779bc2-d944-4f54-9551-5259d1a7de85.png">

จะเห็นว่าภาคตะวันออกเฉียงเหนือมีจำนวนเด็กเกิดใหม่สูงสุดเทียบกับภาคอื่นๆ และมีแนวโน้มที่ลดลงอย่างชัดเจน

3. จังหวัดที่มี %การเกิดใหม่ลดลงมากที่สุด 5 อันดับแรกและน้อยที่สุด 5 อันดับสุดท้ายคือจังหวัดอะไร

<img width="628" alt="Screen Shot 2565-10-14 at 22 54 11" src="https://user-images.githubusercontent.com/56344603/195889255-9683b0f9-7860-449e-b56c-ca5ea695e14d.png">

<img width="905" alt="Screen Shot 2565-10-14 at 22 54 46" src="https://user-images.githubusercontent.com/56344603/195889385-8959fa8e-f443-4314-9e8a-15ff100e8f27.png">

<img width="1181" alt="Screen Shot 2565-10-14 at 22 54 59" src="https://user-images.githubusercontent.com/56344603/195889431-5dcd40ed-80be-46f4-9f1e-4cefd3363004.png">

<img width="820" alt="Screen Shot 2565-10-14 at 22 55 10" src="https://user-images.githubusercontent.com/56344603/195889486-a52e9583-ad4c-4f89-bc97-828c4fe3f7c7.png">

<img width="579" alt="Screen Shot 2565-10-14 at 22 55 22" src="https://user-images.githubusercontent.com/56344603/195889524-7589c8c3-dcba-4e65-bae8-c8f44fa9c4b8.png">

<img width="940" alt="Screen Shot 2565-10-14 at 22 56 07" src="https://user-images.githubusercontent.com/56344603/195889700-bdeb125c-846f-45e0-ab6b-aa6a4ded2e0a.png">

<img width="948" alt="Screen Shot 2565-10-14 at 22 56 38" src="https://user-images.githubusercontent.com/56344603/195889781-5f3657f5-cd2a-4f82-9e4e-b10665b2469c.png">

<img width="1105" alt="Screen Shot 2565-10-14 at 22 56 58" src="https://user-images.githubusercontent.com/56344603/195889841-adcd487c-690b-448a-bbf5-7ca8b458ec90.png">

<img width="1115" alt="Screen Shot 2565-10-14 at 22 57 13" src="https://user-images.githubusercontent.com/56344603/195889914-347d8c4b-5858-470e-b030-f29335f40db0.png">

Plot bar สำหรับจังหวัดที่มี %การเกิดใหม่ลดลงมากที่สุด 5 อันดับ

<img width="631" alt="Screen Shot 2565-10-14 at 22 57 28" src="https://user-images.githubusercontent.com/56344603/195889986-6c799a48-2ccc-4ab6-8c67-dcbf730fbdf5.png">

![image](https://user-images.githubusercontent.com/56344603/195890086-27044a30-7240-4a4a-92d5-bd3153489bf2.png)

Plot bar สำหรับจังหวัดที่มี %การเกิดใหม่ลดลงน้อยที่สุด 5 อันดับ



3. อัตราเด็กไทยเกิดใหม่ลดลง มีผลมาจากค่าใช้จ่ายที่สูงขึ้นหรือไม่ 

    คำตอบ: คาดว่าเป็นไปได้ แต่น่าจะมีปัจจัยอื่นๆร่วมด้วย เช่น วิกฤตอุทกภัยหรือเศรษฐกิจต่างๆ

4. จังหวัดที่ค่าครองชีพสูงจะมีอัตราการเกิดต่ำกว่าจังหวัดที่มีค่าครองชีพต่ำ

    คำตอบ: ไม่พบความสัมพันธ์ระหว่างค่าครองชีพกับ %เด็กเกิดใหม่

5. รายได้และรายจ่ายของคนในแต่ละจังหวัดส่งผลต่ออัตราการเกิด

    คำตอบ: คาดว่ามีความเกี่ยวข้อง เนื่องจากพบว่าภาคอีสานที่มันอัตราการเกิดลดลงมากที่สุด มีค่าเฉลี่ยรายได้และรายจ่ายใกล้เคียงกัน

6. GPP (มูลค่าการผลิตสินค้าและบริการขั้นสุดท้ายของจังหวัด) มีผลต่ออัตราการเกิดหรือไม่ 

    คำตอบ: ไม่พบความสัมพันธ์ระหว่าง GPP และอัตราการเกิด




