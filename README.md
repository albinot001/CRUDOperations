##Api endpoint explenation :

We have 4 crud operation : create , display , update and delete.

For their funcionallity everything is set in controller , functions are tested with postman heres the data on how you can test it out

For example if we look to get all the data back is gonna turn empty because we haven't put anything yet but you can test it out with this endpoint : http://localhost:8000/api/products , now 8000 its my number in ur pc might be different , you should get 200response back but empty response

If u wanna create a product u should use same endpoint put the request as post request in postman and put data in json format at body - raw : {
"name":"Product 2",
"description":"Description",
"price":10.99
}

If u want to test it out to delete u use this endpoint http://localhost:8000/api/products/1 if we consider that this product has id 1 then it will be deleted if you are not sure you go to the get endpoint to get procudcts data and u check what kind of id have ,

And for the update or put as it can be showed in postman , is the same endpoing : http://localhost:8000/api/products/1 , we suppose that we want to change data of a product that already exist otherwise isn't gonna work , you fill the same data as we did in post method and change something small from the inputs not from the variables , and if u request it and it works u can go to get method to get the products and see the changes.

This task took me 40 minutes to be done 25 minutes coding and 15 minutes working with api , as i had 404 error problem , because when i create the project it created it in laravel 11 and you basiclly have to install api folder by ur self with command php aritsan install:api ,
