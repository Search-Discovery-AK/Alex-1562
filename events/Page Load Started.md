# Page Load Started

### Page Load Started is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the first event pushed in the page load event sequence.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Page Load Started",
    "page": {
        "isIncognitoMode": "<isIncognitoMode>",
        "pageCategory": "<pageCategory>",
        "pageExperience": "<pageExperience>",
        "productPageTemplate": "<productPageTemplate>",
        "siteType": "<siteType>",
        "subsection2": "<subsection2>",
        "subsection3": "<subsection3>",
        "weekdayOrWeekend": "<weekdayOrWeekend>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|isIncognitoMode|integer|Set on all pages when user is in "incognito mode" in their browser.||||||||
|pageCategory|string|General category or Site Section of the page. Top level of page hierarchy.|Home, About Us, Shop, Account, Blog, Investors|||||||
|pageExperience|string|When a feature ramp up is taking place, capture a code to identify users receiving that feature's experience.||||||||
|productPageTemplate|string|Captures the template of the page.||||||||
|siteType|string|Common language description of the site type of purpose. May be used to group siteName.|Prospecting, Shop, Members, Brand|||||||
|subsection2|string|Second sub-level of hierarchy under pageCategory or Site Section. |Shop &gt; Kids &gt; Tops, Shop &gt; Mens &gt; Shoes|||||||
|subsection3|string|Third sub-level of hierarchy under pageCategory or Site Section. |Shop &gt; Kids &gt; Tops &gt; Tees, Shop &gt; Mens &gt; Shoes &gt; Oxfords|||||||
|weekdayOrWeekend|string|Whether it was a week day or weekend when activity is occurred.||||||||
