## Dummy Laravel API

Návod na rozbehanie cez Docker:

- stiahnuť cez git
- composer install
- cp .env.example .env
- sail up -d
- sail artisan key:generate
- sail artisan migrate
- sail artisan db:seed

Routes:

| Method       | URL                                          | Description |
|--------------|----------------------------------------------|-------------|
| GET          | api/order-categories	                        |		Get list of order categories |
| POST	        | 	api/order-categories		                      |		Store order category|
| GET	         | api/order-categories/{order_category}	       |	Get order category|
| PUT \| PATCH | 	api/order-categories/{order_category}	      |	Update order category|
| DELETE       | 	api/order-categories/{order_category}	      |	Delete order category|
| GET	         | api/order-statuses		                         |		Get list of order statuses|
| GET          | 	api/orders			                               |		Get list of orders|
| POST	        | 	api/orders		                                |			Store order|
| GET          | 	api/orders/{order}		                        |		Get order|
| PUT \| PATCH | 	api/orders/{order}		                        |		Update order|
| DELETE       | 	api/orders/{order}	                         |			Delete order|
| GET          | 	api/orders/{order}/generate-pdf	            |		Get PDF of order|
| GET          | 	api/orders/{order}/order-items		            |	Get list of order items|
| POST	        | 	api/orders/{order}/order-items		            |	Store order item|
| GET          | 	api/orders/{order}/order-items/{order_item} |	Get order item|
| PUT \| PATCH |	api/orders/{order}/order-items/{order_item}	|Update order item|
| DELETE       | 	api/orders/{order}/order-items/{order_item} |	Delete order item|
| GET	         | api/orders/{order}/status-history		          |Get status history of order|
| GET	         | api/user				                                 |	Get authenticated user data|
| POST	        | 	api/user/update-profile		                   |		Update user profile|
| GET          | 	api/users				                               |	Get list of users|
| POST	        | 	api/users			                                |		Store user|
| GET	         | api/users/{user}		                           |		Get user|
| PUT \| PATCH | api/users/{user}			                          |	Update user|
| DELETE       | 	api/users/{user}	                           |			Delete user|
| GET	         | api/vat-rates			                             |		Get VAT rates|
| POST	        | 	forgot-password		                           |			Send forgot password email|
| POST	        | 	login				                                   |		Login user using credentials|
| POST	        | 	logout				                                  |		Logout user|
| POST	        | 	reset-password		                            |			Reset user password|
| GET	         | sanctum/csrf-cookie	                         |			Get CSRF cookie|
| PUT	         | 	user/password		                             |			Update user password|
