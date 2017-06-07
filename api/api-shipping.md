## API Shipping

API Shipping เป็น API ที่ให้บริการในการดึงค่าข้อมูลต่างๆ ที่สถานะอยู่ในขั้นตอนของการจัดส่ง

### API Call

```
[POST] https://api.sellsuki.com/public/{SELLSUKI_KEY}/shipping-bill
```

### Attribute

| **Name** | **Description** |
| :--- | :--- |
| bill\_id | เป็นเลข ID ของ Bill |
| tracking\_number \(Optional\) | เลข Tracking Number ของพัสดุที่จัดส่ง |

### Parameter Json

```js
{
	"bill_id": "O0117AERVDER00001",
	"logistic_refcode": "AA1234567890TH"
}
```

โดยจะได้รับค่าส่งคืนกลับมา

* success

```
"result":[{"success":1}]}
```

* failed

```
"result":[{"success":0}]}
```



