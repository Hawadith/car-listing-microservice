# car-listing-microservice

1. table Car
```SQL
CREATE TABLE Car (Plate_num varchar(255) NOT NULL, CarType varchar (255) NOT NULL, Registration_date DATE NOT NULL, Expiration_date DATE NOT NULL, Plate_Type varchar(255), Car_Color varchar(255), VIN varchar(255) NOT NULL, Car_model vahrchar(255) NOT NULL, UserID INT, PRIMARY KEY (Plate_num), FOREIGN KEY (UserID) REFERENCES User (UserID))
```
```MangoDB

db.createCollection( Car,
   {
     Plate_num: <int>,
     CarType: <string>,
     RegistrationDate: <date>,
     ExpirationDate: <date>,
     PlateType: <string>,
     CarColor: <string>,
     VIN: <string>,
     CarModel: <string>
   }
```
