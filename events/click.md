# Click

Fire each time a user clicks a link.

## HTML Data Attributes

```html
<a href="{{link_url}}"
  data-layer-link_classes="{{link_classes}}"
  data-layer-link_domain="{{link_domain}}"
  data-layer-link_id="{{link_id}}"
  data-layer-link_url="{{link_url}}"
  data-layer-outbound="{{outbound}}"
>
```

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  event: "click",
  link_classes: '{{link_classes}}',
  link_domain: '{{link_domain}}',
  link_id: '{{link_id}}',
  link_url: '{{link_url}}',
  outbound: '{{outbound}}',
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|link_classes|string|The list of HTML/CSS classes applied to the link.|https://www.example.com|
|link_domain|string|The domain of the link.|https://www.example.com|
|link_id|string|The HTML/CSS ID of the link.|https://www.example.com|
|link_url|string|The full URL of the link.|https://www.example.com|
|outbound|boolean|Does the link point to a different domain?|https://www.example.com|