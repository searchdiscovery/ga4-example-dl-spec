# Page View

Fire whenever a user views a page. This will usually be picked up automatically by GTM on desktop but may need to be manually sent on mobile.

## Javascript Code

```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  event: 'page_view',
  page_location: '{{page_location}}',
  page_referrer: '{{page_referrer}}'
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_location|string|The URL of the page viewed.|https://www.example.com|
|page_referrer|string|The URL of the page viewed before the current page.|https://www.example-referrer.com|
