MAHALS FURNITURE BILLING – FINAL CUSTOMER/PRODUCT FIX

1. Extract this ZIP into a NEW folder.
2. Open OPEN_MAHALS_BILLING.bat from this new folder.
3. Do not use the old desktop shortcut for the first test.
4. Customers -> + Add Customer should open the customer form.
5. Customers -> Edit should open the selected customer.
6. Products / Inventory -> + Add Product should open the product form.
7. Products / Inventory -> Edit should open the selected product.

Important: this version uses the same localStorage database key as the previous versions, so existing billing data in the same browser profile is retained.

The previous startup problem was caused by the invoice GST verification handler referencing UI elements that were missing from the page. That prevented the rest of the JavaScript from initializing. The missing elements are now present and the handler is defensive as well.
