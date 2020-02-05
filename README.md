# Introduction
It is a virtual pet simulator. Originally forked from [Neo-Oli](https://github.com/Neo-Oli/pet/tree/master).

# Configuration
The configuration file is put in config/default.yml with some default settings. The pet was set to have  5 different states: eating, playing, learning, cleaning and sleeping. By default the pet would grow by days. The time required for learning is 3600 s, eating is 60 s...etc. You can also change the default initial values when you generate a new pet. You can only own one pet at the same time, and a pet can only do one thing at a time.
The state values would slowly drop as time goes by, you can change the speed in yml file (end with 'mod'). The pet would be unhappy if states drop to certain values. It may also get sick -- it would die if it is sick for a long time! You can also change value increase after certain care behaviors.

# Installation
> git clone https://github.com/HelloJocelynLu/pet.git
<br>
> python setup.py install

# Setup
First we need to generate a new pet:
> pet new [PetName]

# Take care of your pet
* Feed your pet (All following commands are equivalent)
	> pet feed
	<br>
	> pet eat
	<br>
	> pet food
	<br>
	> pet fd
* Clean your pet
	> pet clean
	<br>
	> pet wash
	<br>
	> pet bath
	<br>
	> pet bathe
	<br>
	> pet cln
* Play with your pet
	> pet play
	<br>
	> pet fun
*  Make it learn
	> pet teach
	<br>
	> pet study
	<br>
	> pet lrn
	<br>
	> pet learn
* Sleep 
	> pet sleep
	<br>
	> pet bed
	<br>
	> pet zzz

# Other Operations
* Change the name of your pet
	> pet rename [NewName]
* Check the status
	> pet
* Check the age
	> pet age
	<br>
	> pet old
* Cancel current activity
	> pet cancel
	<br>
	> pet stop
	<br>
	> pet interrupt
* Heal the pet (If it gets sick)
	> pet heal
	<br>
	> pet medicine

# Log file
After each run, the log file would be updated in ~/.config/pet/default.state.json
