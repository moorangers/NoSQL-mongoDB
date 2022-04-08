<img src="https://img.shields.io/badge/MongoDB-282C34?logo=mongodb&logoColor=47A248" alt="MongoDB logo" title="MongoDB" height="50" />

# NoSQL

### Querying Documents
- ภาษาที่ใช้ใน MongoDB ชื่อว่า MongoDB Query Language (MQL)
- MongoDB มีวิธี Query ตัว Document หลักๆ อยู่สองวิธี ได้แก่
  - find เป็น Function ที่เอาไว้หา Document หลายอันในคราวเดียว

        db.movies.find({
          <Field>: Value
        })
        
  - find เป็น Function ที่เอาไว้หา Document ทีละอัน

        db.movies.findOne({
          <Field>: Value
        })
        
### Projection
- ถ้าเราอยากเห็นข้อมูลแค่บางส่วน เราสามารถใช้เทคนิคที่เรียกว่า Projection ได้


### Query Operators
  - Comparison Operator


  - Logical Operator

### Sorting
- `.sort()` เป็น Function ที่รับ Input เป็น Object ของ Field ที่มี Value เป็น `-1` หรือ `1`
    - `-1` เป็นการเรียงแบบ Descending (จากมากไปน้อย)
    - `1` เป็นการเรียงแบบ Ascending (จากน้อยไปมาก)

### Insert
- sertOne เป็น Function ที่เอาไว้สร้าง Document หนึ่งอันเข้าไปใน Database ตามตัวอย่างด้านล่าง

- insertMany เป็น Function ที่เอาไว้สร้าง Document หลายๆ อันเข้าไปใน Database ตามตัวอย่างด้านล่าง

### Update
- updateOne เป็น Function ที่เอาไว้อัปเดต Document ทีละหนึ่งอัน

- updateMany เป็น Function ที่เอาไว้อัปเดต Document ทีละหลายอัน

- upsert เป็นส่วนผสมของคำว่า update และ insert

### Delete
- deleteOne เป็น Function ที่ใช้ลบ Document ทีละหนึ่งตัว

- deleteMany เป็น Function ที่ใช้ลบ Document ทีละหลายตัว
