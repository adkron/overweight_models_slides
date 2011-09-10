!SLIDE
### Don't worry we will see some code soon ###

!SLIDE smbullets incremental
# Hold Up Playa #

* skinny controller and fat model aren't enough
* validations don't need to be run all the time
* objects have different behaviors in certain instances

!SLIDE smbullets incremental
## skinny controller and fat model aren't enough ##

* I'm tired of opening up a model file and seeing 200 lines
* it doesn't follow SRP

!SLIDE smbullets incremental
## validations waste time ##

* validate uniqueness when I haven't changed the field
* validations stop actions that do not care

!SLIDE smbullets incremental
## objects have different behaviors in certain instances ##

* data owner vs admin vs other user
* state changes but the backing data model does not

!SLIDE fade
# Now onto the code! #

!SLIDE bullets
# Basic App #

* adding requirements breaks functionality

!SLIDE bullets incremental
# The Middle Man #

* supports single responsibility
* fixes validation requirements
* uniqueness only runs when the nickname changes