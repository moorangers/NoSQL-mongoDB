<img src="https://img.shields.io/badge/MongoDB-282C34?logo=mongodb&logoColor=47A248" alt="MongoDB logo" title="MongoDB" height="50" />

# NoSQL

## mongoDB
ภาษาที่ใช้ใน MongoDB ชื่อว่า MongoDB Query Language (MQL)
 
#### Basic command in Mongo Shell

`show dbs` แสดงชื่อฐานข้อมูลภายในเครื่อง

`db` แสดงชื่อฐานข้อมูลภายในเครื่อง

`use <db_name>` เลือกฐานข้อมูลที่ต้องการ

`show clooection` แสดงรายชื่อ collection
        
### Query Command
- `find` เป็น Function ที่เอาไว้หา Document หลายอันในคราวเดียว `db.<db_name>.find()`
        
- `findOne` เป็น Function ที่เอาไว้หา Document ทีละอัน `db.<db_name>.findOne()`

### Projection
- ถ้าเราอยากเห็นข้อมูลแค่บางส่วน เราสามารถใช้เทคนิคที่เรียกว่า Projection ได้ `db.<db_name>.findOne({Query},{Projection})`

### Insert Command
- `insertOne` เป็น Function ที่เอาไว้สร้าง Document หนึ่งอันเข้าไปใน Database `db.<db_name>.insertOne({ data })`

- `insertMany` เป็น Function ที่เอาไว้สร้าง Document หลายๆ อันเข้าไปใน Database `db.<db_name>.insertMany([{ data }, {data}, ...])`

### UpdateCommand
- `updateOne` เป็น Function ที่เอาไว้อัปเดต Document ทีละหนึ่งอัน `db.<db_name>.updateOne({ data })`

- `updateMany` เป็น Function ที่เอาไว้อัปเดต Document ทีละหลายอัน `db.<db_name>.update([{ data }, {data}, ...])`

- `upsert` เป็นส่วนผสมของคำว่า update และ insert

### Delete Command
- `deleteOne` เป็น Function ที่ใช้ลบ Document ทีละหนึ่งตัว `db.<db_name>.deleteOne({ data })`

- `deleteMany` เป็น Function ที่ใช้ลบ Document ทีละหลายตัว `db.<db_name>.deleteOne({ data })`

### Sorting Command
- `.sort()` เป็น Function ที่รับ Input เป็น Object ของ Field ที่มี Value เป็น `-1` หรือ `1`
    - `-1` เป็นการเรียงแบบ Descending (จากมากไปน้อย)
    - `1` เป็นการเรียงแบบ Ascending (จากน้อยไปมาก)

### Query Operators
  - Comparison Operator
    - `$gte` **G**reater **t**han or **e**qual
    - `$gt` **G**reater **t**han
    - `$lte` **L**ess **t**han or **e**qual
    - `$lt` **L**ess **t**han

  - Logical Operator
    - `$and`
    - `$or`
    - `$not`
