# Google Tag Manager Standard eCommerce Tag
This tag utilizes Google Tag Manager’s `dataLayer` to populate a formatted Partnerize purchase event tracking tag.
## dataLayer Format
The [Standard Ecommerce Developer Guide](https://support.google.com/tagmanager/answer/6107169?hl=en) lists the required formatted for the `dataLayer` as it relates to this tag.
### Example
```<script>
window.dataLayer = window.dataLayer || [];
dataLayer.push({
   'transactionId': '1234',
   'transactionAffiliation': 'Acme Clothing',
   'transactionTotal': 38.26,
   'transactionTax': 1.29,
   'transactionShipping': 5,
   'transactionProducts': [{
       'sku': 'DD44',
       'name': 'T-Shirt',
       'category': 'Apparel',
       'price': 11.99,
       'quantity': 1
   },{
       'sku': 'AA1243544',
       'name': 'Hat',
       'category': 'Apparel',
       'price': 9.99,
       'quantity': 2
   }]
});
</script>```
