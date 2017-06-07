## API Prepare to Ship

API Prepare to Ship เป็น API ที่ให้บริการในการดึงค่าข้อมูลต่างๆ ที่สถานะอยู่ในขั้นตอนของการเตรียมจัดส่ง

### API Call

```
[POST] https://api.sellsuki.com/public/{SELLSUKI_KEY}/prepare-bill
```

### Attribute

| **Name** | **Description** |
| :--- | :--- |
| bill\_id | เป็นเลข ID ของ Bill |

### Parameter Json

```

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



