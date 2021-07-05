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
| skus\[0\]\[id\] | id ของ sku |
| skus\[0\]\[price\] | ราคาของสินค้า |
| skus\[0\]\[amount\] | จำนวนของสินค้า |
| skus\[0\]\[name\] | ชื่อสินค้า |
| skus\[0\]\[option_1 , option_2 , option_3\] | รายละเอียดย่อยของสินค้า \(ถ้ามี\) |
| skus\[0\]\[warehouse\] | warehouse ที่สินค้าอยู่ |
| email | email ของลูกค้า |
| tel | หมายเลขโทรศัพท์ของลูกค้า |
| shipping\_type | ประเภทของการจัดส่ง |
| shipping\_price | ค่าจัดส่ง |
| day\_expire | จำนวนวัน ที่กำหนดให้บิลหมดอายุ |
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
        "option_1": "1",
        "option_2": "2",
        "option_3": "3",
        "warehouse": "sellsuki"
    }],
    "email": "",
    "tel": "",
    "shipping_type": "-",
    "shipping_price": 0,
    "day_expire" : 3,
    "debts": [{
        "pay_order": 1,
        "debt_balance": 100
    }]
}
```



