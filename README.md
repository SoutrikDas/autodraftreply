# autodraftreply
Google Appscript to automatically draft a reply depending on the labels that a mail can contain

```js
  var cases = [
    {
      "label": "TLabc",
      "body": `Hello this is a sample \n reply text for  \n mails containing abc <a href="http://google.com">This is a link</a>`,
      "htmlBody": `Hello this is a sample \n reply text but inside htmlBody for  \n mails containing abc <a href="http://google.com">This is a link</a>`
    },
    {
      "label": "TLefg",
      "body": "this mail has efg and this is the reply",
      "htmlBody": ""
    },
  ]
```
You can edit the cases , this program when run will check for all those incoming mails that have the corresponding `label` and then draft a reply based on the htmlBody attribute of that case. 
