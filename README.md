# gps
more or less (only) a to do list




The Dbus is the main collaboration point - we shall deliver "current position data" to the Dbus, and apps will take it from here. 

The App part it not currently our concern - if we deliver the data in regular way the apps only has to be recompiled (or even maybe not).

we have currently NO geo data on the DBus (python check program)

Therefore the "normal" test plan for CPS (https://wiki.ubuntu.com/Process/Merges/TestPlan/location-service) do not have much idea yet .

The data to the DBus has to be delivered in an combination of libhybis/cyan android HAL + ubuntu location-service. 


The ubuntu-location service first of all need to know provider etc in its config.ini
And we need to see how its called (seems like its currently called with HERE-providers...it shall use the config.ini)

Maybe this will do the trick  (try...) 

:C

1) python to make some looking at the Dbus (a nice test program anyway)
2) Config the ubuntu-localisation-service
3) (if that do not work from day one:) we need some way to see the output from android etc BEFORE the Dbus. 
4) Info from the GPS-equipment that android do not get (satellite positions etc)

---

and then - when we at all get some info at the DBus, we can start at second level: To make it faster with A-GPS (seems almost included in the ubuntu-localisation-service).






