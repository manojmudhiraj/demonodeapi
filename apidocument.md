// page 1

>>List of city

(Get)http://localhost:9100/location

>>List of restaurant

(Get)http://localhost:9100/Restaurants

 >>Restaurant on the basis of city

(Get)http://localhost:9100/Restaurants?stateId=2

 >> List of QuickSearch

(Get)http://localhost:9100/mealType

////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
//Page2

>>List of restaurant on basis of meal  
(Get)http://localhost:9100/Restaurants?mealId=1
(Get)http://localhost:9100/Restaurants?mealId=1&stateId=2

 >>Filter on basis of cuisine Filter 

 (Get)http://localhost:9100/filter/1?cuisineId=2 

 >>on basis of cost 

(Get) http://localhost:9100/filter/1?lcost=700&hcost=1200

 >>Sort on basis of cost

(Get)http://localhost:9100/filter/1?lcost=500&hcost=1200&sort=-1


//Page3

>>Details of the restaurant 

(Get)http://localhost:9100/details/5 

>>Menu of the restaurant

(Get)http://localhost:9100/menu/7

//page4

>>Menu details (selected item) 

(Post) localhost:9100/menuItem [1,4,6]

>>place order

(post) localhost:9100/placeOrder 

  {
        "_id": "62a4530019c457ec5e3eacc0",
        "orderId": 1,
        "name": "sujeeth",
        "email": "sujeeth@gmail.com",
        "address": "Hom 29",
        "phone": 99779058,
        "cost": 568,
        "menuItem": [
            4,
            8,
            9
        ],
        "bank_name": "HDFC",
        "date": "29/05/2023",
        "status": "TAX_SUCCESS"
    },
//page5

>>List of order placed

(Get)http://localhost:9100/orders    (we will get details of all the orders)

 >>List of order placed of particular 

 (Get)http://localhost:9100/orders?email=amit@gmail.com    (we will get the order details of a particular user here amit is the user)
 
  >>Update order status

>>(PUT) http://localhost:9100/updateOrder/2 

{
    "status":"TAX_FAIL",
    "bank_name":"AXIS",
    "date":"29/05/2023"
}

 //////////////////////////////////////////////////////////////////////////////////////////


>>Delete orderset 

(Delete) localhost:9100/deleteOrder/628c485d93399d546c136d84













//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
// page 1

List of city

(Get) http://localhost:9100/location List of restaurant (Get) http://localhost:9100/restaurants Restaurant on the basis of city (Get) http://localhost:9100/restaurants?stateId=3 List of QuickSearch (Get) http://localhost:9100/mealType

//Page2

List of restaurant on basis of meal

(Get) http://localhost:9100/restaurants?mealId=5 http://localhost:9100/restaurants?mealId=5&stateId=2 Filter on basis of cuisine (Get) http://localhost:9100/filter/1?cuisineId=2 Filter on basis of cost (>(Get) http://localhost:9100/filter/1?lcost=700&hcost=1200 Sort on basis of cost (Get) http://localhost:9100/filter/1?lcost=500&hcost=1200&sort=-1

//Page3

Details of the restaurant

(Get) http://localhost:9100/details/5 Menu of the restaurant (Get) http://localhost:9100/menu/7

//page4

Menu details (selected item)

(Post) localhost:9100/menuItem [1,4,6] Place order (Post) localhost:9100/placeOrder ( { "name":"Nikita", "email":"nikita@gmail.com", "address":"Hom 39", "phone":934645457, "cost":845, "menuItem":[10,13,17] } )

//page5

List of order placed

(Get) http://localhost:9100/orders List of order placed of particular user (Get) http://localhost:9100/orders?email=amit@gmail.com Update order status (Put) http://localhost:9100/updateOrder/2 ( { "status":"TAX_FAIL", "bank_name":"AXIS", "date":"29/05/2023" }
)

////////////////////////////////

Delete orders

(Delete) localhost:9100/deleteOrder/628c485d93399d546c136d84