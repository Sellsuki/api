## API Create Order

API Create Order เป็น API ที่ให้บริการในการสร้าง Order ของการสั่งซื้อสินค้า โดยสามารถใช้งาน API นี้ได้ตั้งแต่ขั้นตอนแรกของการสร้าง Order

### API Call

```
[POST] https://api.sellsuki.com/public/{SELLSUKI_KEY}/submit
```

### Attribute

| **Name** | **Description** |
| :--- | :--- |
| skus | array ที่เก็บข้อมูลของสินค้าแต่ละ sku |
| \[sku\] id | id ของ sku |
| \[sku\] price | ราคาของสินค้า |
| \[sku\] amount | จำนวนของสินค้า |
| \[sku\] name | ชื่อสินค้า |
| \[sku\] option1 , option2 , option3 | รายละเอียดย่อยของสินค้า \(ถ้ามี\) |
| \[sku\] warehouse | warehouse ที่สินค้าอยู่ |
| email | email ของลูกค้า |
| tel | หมายเลขโทรศัพท์ของลูกค้า |
| shipping\_type | ประเภทของการจัดส่ง |
| shipping\_price | ค่าจัดส่ง |
| pay\_order | \(Default value is 1.\) |
| debt\_balance | ยอดชำระของบิล |

### Json

```js
{
    "skus": [{
        "id": "46484",
        "price": "100",
        "amount": "1",
        "name": "หมา",
        "option1": "1",
        "option2": "2",
        "option3": "3",
        "warehouse": "sellsuki"
    }],
    "email": "",
    "tel": "",
    "shipping_type": "-",
    "shipping_price": 0,
    "debts": [{
        "pay_order": 1,
        "debt_balance": 100
    }]
}
```



