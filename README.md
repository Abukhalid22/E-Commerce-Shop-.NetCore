# E-Commerce Web Shop
#### E-commerce web store using Angular 9, .Net Core 3.1 and Stripe for payment processing

## Project Description
### Project includes 
- .Net Core CLI
- C# Generics
- Using Identity, Automapper, specification, repository, and unit of work
- Angular 9 CLI
- Angular lazy loading
- Angular routing
- Angular reactive forms
- Bootstrap
- Redis
- Stripe Payment

The website is a fully functional e-commerce shop, where the customers can purchase variety of products.
The customers can login, register, view their orders, and add prodcuts to the cart. 

## GUI Design (Client Side)

![image](https://user-images.githubusercontent.com/53325143/93302252-952aa380-f7f1-11ea-80a9-bc7e47fb7bf7.png)

This is the home page of the website, therefore, once the customer enters the website, this is the first thing they will see. 

___

![image](https://user-images.githubusercontent.com/53325143/93302312-ae335480-f7f1-11ea-8243-604abc6dbc2b.png)

This is the product page, where the user can purchase different items. On this page the user can search for a specific product, they can sort the products, by alphabetically, or selecting a brand or a type.
This page will also show the number of items in a page, and the full number of products available. 

___


![image](https://user-images.githubusercontent.com/53325143/93302376-c905c900-f7f1-11ea-8471-0464b41bc117.png)

User searches for red boots on this page. Moreover, 
the web page uses bootstraps breadcrumb to indicate to the user on the webpage that they are on using navigational hierarchy. 

___

![image](https://user-images.githubusercontent.com/53325143/93302423-df138980-f7f1-11ea-81fb-d606ffa4b365.png)

User searches products from lowest price to highest, 
the page also includes pagination, where only certain number of products are displayed per page. 

___

![image](https://user-images.githubusercontent.com/53325143/93302455-ed61a580-f7f1-11ea-8fac-fa97e684e4d5.png)

Once the customer hovers over the product, they then can either view the product, or add it to the cart straight away. 

___

![image](https://user-images.githubusercontent.com/53325143/93302486-fa7e9480-f7f1-11ea-9b00-848e43dba1dc.png)

On this page, the customer can view the product description, as well as choose the number of quantities they require.
Once finished the customer selects add to cart button. 

___

![image](https://user-images.githubusercontent.com/53325143/93302509-066a5680-f7f2-11ea-9b63-3827cdf25996.png)

Once the customer is ready to purchase the items, they will be redirected to the basket webpage, where they can either increase or decrease the quantity amounts, as well as remove items from the cart. This uses Redis-cache as a storage. 
Moreover, the webpage also displays summary of the order, such as the total amount for all the products in the cart. 

___

![image](https://user-images.githubusercontent.com/53325143/93302545-16823600-f7f2-11ea-9a9e-1a731d0b7da1.png)

Before the user can purchase the items, they first must login with their correct credentials. 
If the wrong credentials are inputted, the system will display an error message.

___

![image](https://user-images.githubusercontent.com/53325143/93302577-21d56180-f7f2-11ea-9418-b38bfab6dfd3.png)

If the customer Is new to the website, they can register by selecting the sign-up button. 

___


![image](https://user-images.githubusercontent.com/53325143/93302604-2c8ff680-f7f2-11ea-88e9-85d5912772d0.png)

If the email already exists, the system will display an error message as shown above. 
Likewise, the password must also be inputted correctly.

___

![image](https://user-images.githubusercontent.com/53325143/93302636-39ace580-f7f2-11ea-9bf0-43ea452d591d.png)

Once the user is logged in, they can see their name displayed at the top, 
likewise, the shopping cart will also display the number of products inside the cart. 

___

![image](https://user-images.githubusercontent.com/53325143/93302735-5e08c200-f7f2-11ea-8e32-6ce129244fc3.png)

On this page the user must enter their shipping address details. 
Likewise, the details can later be changed and updated in the future. 

___

![image](https://user-images.githubusercontent.com/53325143/93302793-724cbf00-f7f2-11ea-9035-4f3129ba0e77.png)

If user does not put correct details, they will not be able to proceed to the delivery page,
as the button is disabled as shown above. 

___

![image](https://user-images.githubusercontent.com/53325143/93302840-7e388100-f7f2-11ea-99d9-88fb45486833.png)

User updates details as shown above in the image. 

___

![image](https://user-images.githubusercontent.com/53325143/93302883-8abcd980-f7f2-11ea-9fb3-62833e4f2eb4.png)

The user then must choose the delivery method. This will then be added onto the order summary as shown above on the image. 

___

![image](https://user-images.githubusercontent.com/53325143/93302950-a45e2100-f7f2-11ea-9e9f-cc3abc72e852.png)

The user can then review their order one more time before moving onto the payment page. 

___

![image](https://user-images.githubusercontent.com/53325143/93302981-af18b600-f7f2-11ea-9493-7ab43640c318.png)

The user must then input their payment details. 
The submit order button will remain disabled if the payments details are incorrect. 

___

![image](https://user-images.githubusercontent.com/53325143/93303015-bb9d0e80-f7f2-11ea-8273-e4d5246c15f2.png)

User inputs incorrect card details. 

___

![image](https://user-images.githubusercontent.com/53325143/93303031-c48de000-f7f2-11ea-964f-6b0c4168ec53.png)

User inputs expired card details. 

___

![image](https://user-images.githubusercontent.com/53325143/93303049-ceafde80-f7f2-11ea-800b-4ff25c20a3f4.png)

If user inputs card details with insufficient funds, the system will display error message as shown above on the image.  

___

![image](https://user-images.githubusercontent.com/53325143/93303096-dd969100-f7f2-11ea-9838-581552fce630.png)

Once the user selects the submit order button, the system will display a success message telling the user the order is confirmed. The user can then view their order by selecting the view order button. 

___

![image](https://user-images.githubusercontent.com/53325143/93303120-e9825300-f7f2-11ea-8c20-843a045c9e8f.png)

The user can view all the orders that they have made in the past with the website. Moreover, each order will display its current status of whether the payment has gone through or if the payment has failed as shown above. 

___

![image](https://user-images.githubusercontent.com/53325143/93303151-f7d06f00-f7f2-11ea-835c-2ec750600426.png)

This order shows that the payment has gone through successfully. 

___

![image](https://user-images.githubusercontent.com/53325143/93303179-028b0400-f7f3-11ea-839d-b31e0b709287.png)

This order shows that the payment did not go through successfully and failed. This is done through using Stripe webhooks. 

___

![image](https://user-images.githubusercontent.com/53325143/93304154-77127280-f7f4-11ea-990b-c31a94b5182d.png)

___

![image](https://user-images.githubusercontent.com/53325143/93303237-15053d80-f7f3-11ea-9613-26290e754538.png)

All the payments can then be seen on Stripe’s dashboard, moreover, it also shows whether each order payment was successful or unsuccessful as shown above on the images. 





___















































































































