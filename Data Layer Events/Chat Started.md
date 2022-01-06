# Chat Started

### 

## Javascript Code
```js
window.dataLayerE = window.dataLayerE || [];;
dataLayerE.push({ event_data: null });  // Clear the previous event_data object.;
dataLayerE.push({
  "event": "chat_started",
  "apollo_event": "Chat Started",
    "event_data": {
        "chat_portal_id": "<chat_portal_id>",
        "chat_service_line": "<chat_service_line>",
        "chat_session_id": "<chat_session_id>",
        "chat_started_counter": "<chat_started_counter>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|chat_portal_id|string|Count of times the price of a product was hidden in the cart due to MAP \(Minimum Advertised Pricing\) requirements.
  Set in the product string for only those products where it is applicable, with a value of 1||||||||
|chat_service_line|string|Count of times a product was out of stock at the time of cart view.||||||||
|chat_session_id|string|Count of times that visitors encountered a product that was back-ordered.||||||||
|chat_started_counter|unknown|Count of times that a user requested a physical product catalog.||||||||




