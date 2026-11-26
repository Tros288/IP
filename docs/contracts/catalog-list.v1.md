# API รายการสินค้า
สถานะ: PROPOSED
รุ่น: v1
เจ้าของข้อเสนอ: Microservice

คำขอ: GET /api/v1/catalog/products
Request body: ไม่ส่ง
Query: available เลือกใส่ได้ รับ true หรือ false



id        | name        | priceSatang | available
pencil    | ดินสอ        | 1200        | true 
ruler     | ไม้บรรทัด     | 2000         | false 
eraser    | ยางลบ       | 800          | true
sharpener | กบเหลาดินสอ  | 1500         | false 

Query
available = true | pencil, eracer | ส่งอันที่เป็น true
available = false | ruler, sharpener | ส่งอันที่เป็น false 
available = [] | all | ส่งทุกอัน
available = yes | available ไม่รองรับ

field
[
  {
    "id": "pencil",
    "ชื่อสินค้า": "ดินสอ",
    "priceSatang": 1200,
    "available": true
  },
  {
    "id": "ruler",
    "ชื่อสินค้า": "ไม้บรรทัด",
    "priceSatang": 2000,
    "available": false
  },
  {
    "id": "eraser",
    "ชื่อสินค้า": "ยางลบ",
    "priceSatang": 800,
    "available": true
  },
  {
    "id": "sharpener",
    "ชื่อสินค้า": "กบเหลาดินสอ",
    "priceSatang": 1500,
    "available": false
  }
]