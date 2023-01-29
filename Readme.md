# Hotel Reservation System
# Introduction
This is a hotel reservation system that allows customers to book a hotel using a credit card. The system is implemented in Python and uses the pandas library to read and store the data.

## Files
hotels.csv: stores information about hotels such as id, name and availability.
cards.csv: stores information about valid credit cards.
card_security.csv: stores information about the password associated with each credit card.
## Classes
### Hotel
The Hotel class represents a hotel. It has the following methods:

__init__(self,hotel_id): initializes the hotel with its id and sets the name.
book(self): changes the availability of the hotel to "no".
available(self): returns True if the hotel is available, False otherwise.
### ReservationTicket
The ReservationTicket class represents a reservation ticket. It has the following methods:

__init__(self,customer_name,hotel_object): initializes the reservation ticket with the customer's name and the hotel object.
generate(self): returns a string with the reservation data.
### CreditCard
The CreditCard class represents a credit card. It has the following methods:

__init__(self,number): initializes the credit card with its number.
validate(self,expiration,holder,cvc): returns True if the credit card is valid, False otherwise.
### SecureCreditCard
The SecureCreditCard class extends the CreditCard class. It has the following methods:

authenticate(self,given_password): returns True if the password is correct, False otherwise.
Running the code
The code reads the data from the files and initializes a hotel based on the id entered by the user. Then, it checks if the hotel is available and, if so, validates and authenticates the credit card. If everything goes well, it books the hotel and generates the reservation ticket. If there is a problem with the payment or the authentication, the system prints an error message.

## Conclusion
This system allows customers to book a hotel with a secure credit card. The code is simple, readable and scalable. The use of pandas makes it easy to store and access the data.