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
