# API_Little_Lemon
Little Lemon API
The Little Lemon API is an API for the Little Lemon restaurant. Little Lemon's management wants to have an online-based order management system and mobile application. The LittleLemonAPI is the back-end API that allows customers to browse food items, view the item of the day and place orders. Managers are able to update the item of the day and monitor orders and assign deliveries. The delivery crew are able to check the orders assigned to them and update an order once it is delivered.

Features
User groups It contains two user groups (Manager & Delivery crew) and some random users assigned to these groups from the Django admin panel.

Manager

Delivery crew

Users not assigned to a group will be considered customers.

This API makes it possible end-users to perform certain tasks. It has the following functionalities.

The admin can assign users to the manager group

-GET method:
    -from Managers and Superusers:
        Lists all users in the managers group
-POST method:
    -from Managers and Superusers:
        Adds a user to the managers group given:
            username

     -GET method:
    Displays all details of the given {menuitemId} 
-PATCH method:
    from Managers and Superusers:
        Toggles the featured status of the given {menuitemId}
-DELETE method:
    from Superusers:
        Deletes the given {menuitemId}       
        -GET method:
    -from Managers and Superusers:
        Lists all users in the managers group
-POST method:
    -from Managers and Superusers:
        Adds a user to the managers group given:
            username
            -DELETE method:
    from Managers and Superusers:
        Removes the User associated with {userId} from the managers group 
        -DELETE method:
    from Managers and Superusers:
        Removes the User associated with {userId} from the delivery crew group
        -GET method:
    from Users:
        Displays orders owned by user
    from Delivery Crew:
        Displays orders assigned to delivery crew member
    from Managers and Superusers:
        Displays all orders
-POST method:
    places an order based on items in the user's cart, and empties the cart.
    -GET method:
    from User:
        Shows the order details associated with {orderId} details if user is owner of order.
    from Delivery crew, Managers and Superusers:
        Shows the order details associated with {orderId}
-PATCH method:
    from from Delivery crew, Managers and Superusers:
        Toggles the status of the order associated with {orderId}
-PUT method:
    from Managers and Superusers:
        Assigns a delivery crew to the the order associated with {orderId}
-DELETE method:
    from Managers and Superusers:
        Deletes the order associated with {orderId}
        
