
# OOAD-WEEK011 Homework
##Activity Diagram

### Activity Diagram1
Code
```
@startuml

start
:login;
:entervalue;
:submitvalue;
:calculatevalue;
stop
@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Hormwork1/Activity%20Diagram01.png?raw=true">

### Activity Diagram2
Code
```
@startuml

start
: insertdata;
:encryption;
if () then (submit)
  :storedata;
else (retrieve)
  :decrypt;
  :displaydata;
endif
stop 
@enduml

```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Hormwork1/Activity%20Diagram02.png?raw=true">

### Activity Diagram3
Code
```
@startuml
|starttyping|
start
:admin;
|#AntiqueWhite|System|
:login;
if () then (yes)
  :update;
else (no)
  :filldata;
  :closerecord;
  :activity;
  endif
stop
@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Hormwork1/Activity%20Diagram03.png?raw=true">

### Activity Diagram4
Code
```
@startuml
start  
note right
    "client is registered"
  end note
  :cliententerlogin;
if (correctlogin) then (yes)
  :clienthassuccessfully;
  :clientsettings;
else (no)
  :invalidlogin;
  :cliententerlogin;
endif
stop
note right
    "client log inot the system"
  end note
@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Hormwork1/Activity%20Diagram04.png?raw=true">

### Activity Diagram5
Code
```
@startuml
|user|
start
|#AntiqueWhite|System|
 :choosecategory;
|#AntiqueWhite|database|
 :dataretrieved\nfortable;
|#AntiqueWhite|System|
 :selectitems;
|#AntiqueWhite|database|
 :retrieveddata;
|#AntiqueWhite|System|
 :eachvaluesofeach;
 :selectamongchoices;
 :checkout;
 :selectyesfrom\nconfirmation;
|#AntiqueWhite|database|
 :soldcount\nupdated;

stop
@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Hormwork1/Activity%20Diagram05.png?raw=true">
