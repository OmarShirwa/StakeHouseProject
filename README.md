# StakeHouseProject . C-Language Program to manage a restaurant

The Program and project report be found in the .rar file above.

1- whats the purpose of the program and how it works.
2- sections in detail.
3- code and what method or algorithms i used.


          step 1 : the structure of the program
 
For this project, I chose to make a Resturant Food/Order Management.
In this program, you have the customers and employee's. You can add new employee's and you can remove employee's too.
And then you have the customer service, The can make an order and as well as have it delivery it to them.


         step 2 : The Sections

Once you run the program, You can see that in the Main Menu you get 4 options. 

 1 - The administration Section

In This section, You can add, remove, Search, and also view the Employee's records. and also View the previous orders the was placed.
To add a new employee, you select the "Add record" option. and put in their information such as ID, name, date of birth, and etc.
After add a new employee record, your given the choice to add another employee or go back to the Administration section.

And if select the second Option which is the "search the record", your given the choice to search by ID or by Name. 
if you choose by ID then you just need to enter the employee's ID and then their record will appear. 
and If you chose by name then you just need to enter the employee's Name and then their record whill appear.

If you select the third Option, which is the "Delete Record", then your asked to the employee's ID then their info will appear.
then your given the choice to Delete them.

if you select the fourth Option, which is the "View Records", then all of the Employee's record will appear.

if you select the fifth Option, which is the "View the preivous Orders", it will show you the  orders.


  2 - Customer Section

In this section, you are given two choices "Vegetarian" and "Non-Vegetarian" depending on what the customer wants.

if they choose Option 1, which is the "Vegetarian", then the Vegetarian Menu appears, From here the Customer order what they want and how much they would like.
After they order, They asked to Fill in the contact form, which asks for their name, place, and etc. 
After they have filled in the form everything gets saved in the order File.

if they choose Option 2, which is the "Non-Vegetarian", then the Non-vegetarian Menu appear, From here the Customer order what they want and how much they would like.
After they order, They asked to Fill in the contact form, which asks for their name, place, and etc.
After they have filled in the form everything gets saved in the order File.

  3 - About Us Section

In this section, I didn't put in too much detail information, just creating details.



    	 Step 3 :  The Code

In the script, what i did was I created different functions/methods for every Section so that my code was simple and flexable.
such as mainMenu, Administration, addRecord, deleteRecord, searchRecord, viewRecord, customer, vegetarain, nonVegetarian, details, aboutUs and etc.
and I also created a data type Structure named "employee", that has couple variables such as the total, quantity and so on.

In the administration function, I used a switch case statement. so that when the user one of the options in the administration section, it can run different functions.
for instance, in the Administration section, choice number 1 is "Add Record" and choice number 2 is "Seach Record" and so on. so if the user selects choice 1.
the Switch case runs the "addRecord" function"

In the addRecord function, we have another function called "getData". what this function does is, It asks the users to enter their infor or this case the Employee's info.
After the Employee's data, It creates a "record.txt" file and save that data in there. and if the record file already exists then it just opens it and adds the data.

And if the user selected choice number 2, it runs the "searchRecord" function. in This function, 
It asks the user to choose if they want to search an employee's record by ID or name.
Then it open the "record.txt" file.
if they choose by ID, it asks the user to enter an ID and then Searchs the file for a record with that ID.
If they choose by name, it does the same and searchs the file for a record with that Name.

And if the  user selected choice number 3, it runs the "deleteRecord" function. In this function,
it asks the user to enter the employee's ID. once it has the ID, it open the record file and search for a record with that ID and displays it.
once it displays the record info, it asks the user if they want to delete this record. if they say yes, 
Then what it does is it creates a new file called "test1" as temporary File.
then it scans the record file for any record that doesn't have the same ID the user gave. it copies that record into the test1 file.
now that All the record have been transfered into the temporary file, it deletes the "record.txt" file with the employee's record that the user wanted to delete.
then it renames the the temporray file test1 to "record.txt" file.

if the user selected the choice number 4, then it runs the "viewRecord" function. In this function,
it opens the record file, and displays all the data in it.

if the user selected the choice number 5, then it opens the "order.txt" file and displays the order data.

In the Customer Function, it asks the user to choice betwenn vegetarian and Non-vegetarian. 

if the user chooses the vegetarian option, then it runs the "vegetarain" function, In this function,
It displays the vegetarain Menu, and asks the user to make an order.
once they choose something from the menu, it asks how much they want(the quantity),
and they sums up the total and display it. then it runs the detail funtion which asks the customer to fill their contact detail and then display it and save it all in the order.txt file.

and If they user choose the Non-vegetarain option, it runs the "vegetarain" function and basically does the same thing.

