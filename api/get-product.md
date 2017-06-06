## API Get Products

API Get Product เป็น API ที่ให้บริการในการดึงค่าข้อมูลต่างๆ ของสินค้า เช่น รหัสสินค้า ชื่อสินค้า เป็นต้น

### วิธีการใช้งาน

API Call

```
https://api.sellsuki.com/public/{Sellsuki Key}/products
```

โดยผลลัพธ์ที่ได้รับมาจะมีลักษณะดังนี้

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

โดยรายละเอียดของแต่ละ Key มีดังนี้

