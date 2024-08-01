# Booking-rooms-data

Hi  there 👋

Project Objective:-


  The objective of this assignment is to execute the steps discussed  in the Power Query for the given datasets. 

  Performed all the function on two CSV files :

	bookings_data.csv

	rooms_data.csv



1. bookings_data: The bookings_data file consisted of several columns, such as date, property_id, property_name, hotel_type, city|city_code, room_id, 

		  successful_bookings, and capacity. This file provides insights into the number of successful bookings made for a property on a given 

		  date and in a specific city, as well as the overall capacity of the property.



2. rooms_data: The rooms_data file consisted of two columns, room_id and room_class. This file is useful in determining the room_class associated 

	       with each room_id in the bookings_data file.

   



//........  Used external resources or search engines such as Google to help complete this .




To complete this assignment, I followed the steps below:

1. Opened a new Excel file and load the two provided CSV files using the "From Text/CSV" option. Then, open Power Query.

2. Changed the data type of the "property_id" column to "text".

3. Some values in the "property_name" column were shown as "Atliq bay" instead of "Atliq Bay". Replace those values to show "Atliq Bay" instead.

4. Formated the "property_type" column by removing any unnecessary leading or trailing spaces using the TRIM() function.

5. The "city|city_code" column includes both the city and city_code separated by a '|' symbol. Splited this column to 

   separate these two entities and renamed the resulting columns accordingly.

6. Created a new conditional column called "Availability Status". If "successful_bookings" equals "capacity", set the value to "sold out"; otherwise, set it to "vacant".

7. Created a new custom column called "occ%", which represents the ratio of successful_bookings to capacity. Changed the data type to a percentage format.

8. Merged the two tables, "bookings_data" and "rooms_data", on the "room_id" column to add the "room_class" column to the "bookings_data" table.

   Reorder the columns so that "room_class" is next to "room_id".

9. Extracted the month_name from the "date" column.

