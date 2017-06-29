## Confirm Order

เป็น Webhook ที่ใช้ติดต่อกับ Server ของผู้ใช้ เมื่อมีผู้ใช้มีการ Confirm Order

### [Json](https://fen555.github.io/SellsukiDocs/#/WebHook?id=json) {#json}

```js
{
    "bill": {
        "id": "O0117HWH23200407",
        "url": "lIogaCd",
        "expire": "2017-02-07 16:59:59",
        "discount": "0.00",
        "ship_cost": "30.00",
        "net": "4310.00",
        "note": "FB14602",
        "print_tag_date": null,
        "shipping_ref_code": null,
        "bill_type": "standard",
        "bill_offer_type": "bill",
        "current_state": "pending",
        "shipment_timestamp": null,
        "flag_bill_seen": "0",
        "status": "1",
        "create_by_sellsuki_user_id": "16766",
        "update_by_sellsuki_user_id": "16801",
        "create_time": "2017-01-30 12:28:14",
        "update_time": "2017-02-06 14:21:34",
        "currency_id": "139",
        "store_id": "13823",
        "store_channel_type": "facebook",
        "customer_name": "Makhampom",
        "customer_shipping_name": "\u0e0d\u0e32\u0e14\u0e32  \u0e40\u0e01\u0e23\u0e35\u0e22\u0e07\u0e44\u0e01\u0e23\u0e27\u0e38\u0e12\u0e34\u0e01\u0e38\u0e25",
        "customer_address": "480 \u0e2b\u0e21\u0e39\u0e48 7  \u0e15.\u0e40\u0e0a\u0e35\u0e22\u0e07\u0e14\u0e32\u0e27  \u0e2d.\u0e40\u0e0a\u0e35\u0e22\u0e07\u0e14\u0e32\u0e27\r\n\u0e08.\u0e40\u0e0a\u0e35\u0e22\u0e07\u0e43\u0e2b\u0e21\u0e48",
        "customer_postcode": "50170",
        "customer_country": "Thailand",
        "customer_tel": "+66811111111",
        "customer_email": "test@hotmail.com",
        "customer_picture_credential": "1132160111111111",
        "store_offer_id": "30861",
        "flag_closed_bill": "0",
        "stock_timestamp: null,
        "cache_shipping_type": "EMS",
        "concat_warehouse": "sellsuki",
        "prepare_shipment_timestamp": null,
        "notify_shipment_timestamp": null
    },
    "event": "asktoconfirm",
    "sku": [{
        "sku_photo": "https:\/\/sellsuki-picture.s3-ap-southeast-1.amazonaws.com\/20160704215806fHmPSBzRid_13823",
        "sku_name": "NAVY,23.0,",
        "sku_id": "3280774",
        "product_name": "COTTON [REAL SUPPORT]",
        "amount": "1.00",
        "price": "4280.00",
        "sku_code": "COTTONNV230",
        "line_item_sfdc_id": null
    }],
}
```



