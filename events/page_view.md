# Account Created

Fire whenever a user completes the process of registering for an account.

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

