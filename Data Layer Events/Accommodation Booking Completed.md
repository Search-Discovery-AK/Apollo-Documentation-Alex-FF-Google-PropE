# Accommodation Booking Completed

### 

## Javascript Code
```js
window.dataLayerE = window.dataLayerE || [];
dataLayerE.push({ ecommerce: null });  // Clear the previous ecommerce object.;;
dataLayerE.push({
  "event": "purchase",
  "apollo_event": "Accommodation Booking Completed",
    "ecommerce": {
        "booking_reservation_id": "<booking_reservation_id>",
        "coupon": "<coupon>",
        "items": [
            {
                "affiliation": "<affiliation>",
                "currency": "<currency>",
                "index": <index>,
                "item_id": "<item_id>",
                "item_list_id": "<item_list_id>",
                "item_list_name": "<item_list_name>",
                "item_name": "<item_name>",
                "item_variant": "<item_variant>",
                "location_id": "<location_id>"
            }
        ],
        "lodging_location_id": "<lodging_location_id>",
        "transaction_id": "<transaction_id>",
        "value": <value>
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|affiliation|string|A product affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|booking_reservation_id|string|Captures the reservation ID associated with each booking.||^[a-zA-Z0-9]{6,20}$|6|20||||
|coupon|string|Order-level coupon code used for a purchase.|summer\_fun|||||||
|currency|string|The currency, in 3-letter ISO 4217 format.|USD|||||||
|index|number|The index\/position of the item in a list.|1, 2, 3, 4|||||||
|item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\) |SKU\_12345|||||||
|item_list_id|string|The computer-readible machine name of the list the item showed up in \(if sent with a view\_item\_list event\). Use UUID provided by the component if no more specific ID is available.|12345abcde12345|||||||
|item_list_name|string|The human-readible name of the item list the item showed up in \(if sent with a view\_item\_list event\). If one is not available, populate with numerical index of which list this is on the page \(1-indexed\). For filter\_by\_group component, use that value.|filter\_by\_group, recommended\_products, recently\_viewed\_products|||||||
|item_name|string|Item Name \(context-specific\).|jeggings|||||||
|item_variant|string|The variant of the item.|Black|||||||
|location_id|string|The location associated with the event. If possible, set to the Google Place ID that corresponds to the associated item. Can also be overridden to a custom location ID string.|L\_12345|||||||
|lodging_location_id|string|Captures a unique ID of a physical location such as a store, banking branch, atm, hotel, office, or other.|155, 65588, 987764448|||||||
|transaction_id|string|The unique identifier of a transaction.|T\_12345, 19283j2nm9jdjs|^[a-zA-Z0-9]{6,20}$|6|20||||
|value|number|The monetary value of the event.	|7.77, 239.55, 659|||||||




