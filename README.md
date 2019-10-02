This project implements an employee attendance system using an RFID sensor which is interfaced with an Arduino.

On the hardware side here, we use an Arduino Uno, MFRC522 RFID Sensor and an LCD Display.

The MFRC522 libraries for the arduino can be found on Miguel Balboa's repository and and he holds the license rights, Link to which are: https://github.com/miguelbalboa/rfid. The MFRC522.cpp and MFRC522.h files have anyway been included with the project. For installation of these libraries follow Miguel's instructions.

Python is being used interfacing between the Arduino and the system connected/hosting to the MySQL database. Install the respective Python libraries used in the program before use.

A MySQL database as "employee_attendance.sql". Import this to your database.

A Python file input.py to input new user data to the Database. This can be done by the Administrator.

For quick referencing for every employee with certain "emp_id", say n, a separate table named as "n_attn_mon" is created which keeps a track of the months the employee was present. Next say employee was present at least on one day in Dec 2016, then this data will be stored in "n_attn_mon" as "122016". Also a table for that month, here Dec, will be created as "n_122016" and this table will keep the day to day attendance track for the employee. This makes future referencing easier.

The code is easy to understand and you are free to use the code as it is or add additional features as per your requirement (like open a door,etc). Just follow the licensing norms.

In case of any issues, you can ping me at anantshukla1234@gmail.com or anantshuklauav@gmail.com

In my next release, I'll try to include an employee management web portal, where a user can create their profile, thus eliminating the use for the python script.