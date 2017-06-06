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
| option\_concat\_1 , option\_concat\_2 , option\_concat\_3 | เก็บลักษณะย่อยของ variant เช่น variant\_1 เก็บ size ใน option\_concat\_1 ก็จะเก็บเป็น S,M,L,XL เป็นต้น |

* #### Attribute Product SKU

| **Name** | **Description** |
| :--- | :--- |
| id | id ของ product\_sku เป็นการ running number |
| code\_temp | รหัสสินค้าที่ระบบของ sellsuki ทำการ generate ให้อัตโนมัติ |
| code | รหัสสินค้าที่ร้านค้ากำหนดขึ้นเอง |
| price | ราคาของสินค้า |
| status | สถานะของสินค้า \(0 - delete , 1 - active\) |
| product\_id | รหัสของสินค้า จากตาราง Product |
| option1 , option2 , option3 | ข้อมูลที่ตัดมาจาก option\_concat\_1 , option\_concat\_2 , option\_concat\_3 ตามลำดับ |

### Json

```js
results: [
{
    id: "110001",
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
    product_tags: null,
    concat_lot_type_all_warehouse: "normal:;:normal:;:normal",
    concat_warehouse_name_all_warehouse: "sellsuki:;:sellsuki:;:sellsuki",
    concat_remaining_quantity_all_warehouse: "10:;:10:;:10",
    concat_sku_cost: "200.00:;:200.00:;:200.00",
    warehouse_name: "sellsuki",
    product_brand: null,
    product_src: "https://sellsuki-picture.s3-ap-southeast-1.amazonaws.com/kQDKQCsKKx420150731T0523S2318740056711316220.png",
    concat_product_category: null,
    concat_product_tag: null,
    concat_product_shelf: null,
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
},
```



