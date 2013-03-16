TrafficLight
============

A traffic light application to drive home some Ruby OOP principles.

# INSTALL

1. Get a copy of Shoes running, resources online at:
    https://github.com/shoes/shoes/wiki/Building-Shoes
    http://shoesrb.com/manual/Installing.html
    
2. Fork your own copy of this exercise and clone it
  * fork
  * git clone url
  * cd TrafficLight

3. Run
    shoes traffic.rb
    
# TODO

We'll be modifying a Shoes application that models a traffic light.

* Using inheritance, implement 3 subclasses of Bulb: GoBulb, WaitBulb and 
StopBulb. Change the subclasses so that when we define them, the correct colour
is displayed. Suggest that the following colours are used:
  |Go  | "#00FF30" | 
  |Wait| "#FFFC00" |
  |Stop| "#FF0000" |
* Refactor the implementation so that the colours are defined once in a module 
called TL, and we can refer to colours with the following syntax:
  |TL:Go  | "#00FF30" | 
  |TL:Wait| "#FFFC00" |
  |TL:Stop| "#FF0000" |
* Refactor the implementation so that a bulb only shows its true colour when it 
is switched on, otherwise it shows grey. Fix the application so that it shows 
the TL::Stop state on startup. 
* Implement the click method, so that every time the traffic light is clicked, 
the colours cycle through the states given in the TrafficLight class
* Change the TrafficLight class so the pattern matches US-style traffic lights.