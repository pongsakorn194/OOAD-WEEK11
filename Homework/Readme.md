# OOAD-WEEK011 Homework
##State Diagram

### State Diagram1
Code
```
@startuml

[*] --> Internetcafe

Internetcafe -> Play
Play -> Timeout
Timeout -> overtime
overtime -> Play
Timeout --> [*]

@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Homework/State%20Diagram01.png?raw=true">

### State Diagram2
Code
```
@startuml
[*] --> Active

state Active {
[*] -> lamp

lamp -down-> switchoff
lamp -> switchon

switchoff --> lampoff : off
switchon --> lampon : on

@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Homework/State%20Diagram02.png?raw=true">
### State Diagram3
Code
```
@startuml

[*] --> running
state running {

washing -> rinsing
rinsing ->spinning
spinning -> [*]
}
running -> poweroff:powercut
poweroff -> running: restorepower

@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Homework/State%20Diagram03.png?raw=true">
### State Diagram4
Code
```
@startuml

[*] --> wedbrowser

wedbrowser ->editdata

state "editdata" as editdata {
[*] --> data
}
editdata -down-> cancel : error
editdata ->Therecordeddata
Therecordeddata ->[*]

@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Homework/State%20Diagram04.png?raw=true">
### State Diagram5
Code
```
@startuml

[*] --> selectdrink
state selectdrink {
coffee -down-> makepayment
chocolate -down-> makepayment
tea -down-> makepayment
milk -down-> makepayment
}
state makepayment {
}
state makedrink{
makepayment -down-> makedrink : amount=price
makepayment -down-> makedrink : amount>price
makepayment -down-> makedrink : amount<price
}
state drinkready{
makedrink -> drinkready : timedelay
}
drinkready -> [*] : drinkremoved

@enduml
```
Diagram

<img src="https://github.com/pongsakorn194/OOAD-WEEK11/blob/master/Homework/State%20Diagram05.png?raw=true">
