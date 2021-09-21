# shopify-image-repo
Winter 2022 - Shopify Developer Intern Challenge

This challenge was implemented in Python using Flask and sqlite3.

To use this application, clone the repo and run `python3 server.py` at the root of the project directory.
This will start the Flask server and also set up the necessary database tables we use to track product info/transactions.

Open http://127.0.0.1:5000/ to view the application in the browser. Then, you'll see a list of products with their images, names, price, and the 
quantity of those products left in stock.

This data is pulled directly from a database table and is generated live with an HTML template to serve as the user interface. The images for
the products are served from a static folder within the project directory.

You can interact with the application by clicking on the `BUY` button that can be seen on each product card. Once this is clicked, it will make sure that there
is in fact some of this product left in stock and record this transction with the following information in our transactions table: product, price, and time.
It will also decrement that product's inventory appropriately. At the top of the page, you can also see the total dollar amount of all transactions
we have conducted/processed to-date.

## Note:
There's also a `Reset DB` option to reset our database and clear all data within it. You can utilize this option if you'd like to re-start the application
from scratch without having to manually quit the application and rerun it again.
