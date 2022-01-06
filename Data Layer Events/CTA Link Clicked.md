# CTA Link Clicked

### 

## Javascript Code
```js
window.dataLayerE = window.dataLayerE || [];;
dataLayerE.push({ event_data: null });  // Clear the previous event_data object.;
dataLayerE.push({
  "event": "select_content",
  "apollo_event": "CTA Link Clicked",
    "event_data": {
        "cta_link_click_event": "<cta_link_click_event>",
        "cta_link_id": "<cta_link_id>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|cta_link_click_event|string|Count of revenue taking place offline from internal databases for use in comparing to online revenue.||||||||
|cta_link_id|string|Count of times that visitors began the room booking process.|act now, cancel, ok, 3456, 8765|||||||




