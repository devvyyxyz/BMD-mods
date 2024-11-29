Exnesion packages allow you to upload and share bulk actions, events, automations, and thems

## Info.md
```md
{
  "name": "Package's Name", /*Your package name, such as Moderation package*/
  "requirements": {
    "node_modules": [], /*The required node modules to use this package*/
    "automations": ["Workshop"] /*The required extensions to use this package*/
  },
  "translation_support": true, /*If translations are supported make value true otherwise make it false*/
  "reject_legacy": false /*If legacy is supported make value false otherwise make it true*/
}
```

## Download Extension packages example folder
[!file](/assets/Files/Ext%20Template.zip)