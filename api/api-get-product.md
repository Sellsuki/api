## API Get Product

API Get Product เป็น API ที่ให้บริการในการดึงค่าข้อมูลต่างๆ ของสินค้าแต่ละชิ้นในระบบ เช่น รหัสสินค้า ชื่อสินค้า เป็นต้น

### API Call

```
[GET] https://api.sellsuki.com/public/{SELLSUKI_KEY}/products/{id}
```

### Attribute

* #### Attribute Product

| **Name** | **Description** |
| :--- | :--- |
| id | id ของ product นั้น โดยจะเป็นการ  running number |
| code\_temp | รหัสสินค้าที่ระบบของ Sellsuki ทำการ Generate ให้อัตโนมัติ |
| name | ชื่อสินค้า |
| description | คำอธิบายของสินค้า |
| status | สถานะของสินค้า \(0 - delete , 1 - active\) |
| store\_id | id ของร้านค้า |
| variant\_1 , variant\_2 , variant\_3 | เก็บ variant ของสินค้าเช่น size,color หากไม่กำหนดจะเก็บข้อมูลเป็น SKU ที่ variant\_1 |
| warehouse\_name | ชื่อของ warehouse |
| photos | รูปภาพของสินค้า \(array\) |

* #### Attribute Product SKU

| **Name** | **Description** |
| :--- | :--- |
| id | id ของ product\_sku เป็นการ running number |
| option1 , option2 , option3 | ข้อมูลที่ตัดมาจาก option\_concat\_1 , option\_concat\_2 , option\_concat\_3 |
| code | รหัสสินค้าที่ร้านค้ากำหนดขึ้นเอง |
| price | ราคาของสินค้า |
| status | สถานะของสินค้า \(0 - delete , 1 - active\) |
| product\_id | รหัสของสินค้า จากตาราง Product |
| stock | จำนวนคงเหลือใน Stack |
| src | รูปภาพของสินค้า |

### Json

```js
results: [
{
    id: "399804",
    code_temp: "PD00020",
    name: "EMS",
    description: "",
    status: "1",
    create_by_sellsuki_user_id: "9554",
    update_by_sellsuki_user_id: "9554",
    create_time: "2017-05-22 10:18:26",
    update_time: "2017-05-22 10:18:26",
    variant_1: "Size",
    variant_2: "",
    variant_3: "",
    gen_url: "",
    product_brand: null,
    product_tags: null,
    product_src: "https://sellsuki-picture.s3-ap-southeast-1.amazonaws.com/kQDKQCsKKx420150731T0523S2318740056711316220.png",
    photos: [
    "https://sellsuki-picture.s3-ap-southeast-1.amazonaws.com/kQDKQCsKKx420150731T0523S2318740056711316220.png"
    ],
    skus: [
    {
        id: "796514",
        option1: "s",
        option2: "",
        option3: "",
        code: "PD00020-1",
        price: "250.00",
        status: "1",
        stock: "10",
        src: "https://sellsuki-picture.s3-ap-southeast-1.amazonaws.com/kQDKQCsKKx420150731T0523S2318740056711316220.png"
    },
    {
        id: "796515",
        option1: "m",
        option2: "",
        option3: "",
        code: "PD00020-2",
        price: "250.00",
        status: "1",
        stock: "10",
        src: ""
    },
    {
        id: "796516",
        option1: "l",
        option2: "",
        option3: "",
        code: "PD00020-3",
        price: "250.00",
        status: "1",
        stock: "10",
        src: ""
    }
    ]
}
]
```



