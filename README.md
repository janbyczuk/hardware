# Simracing

Simracing addons: Buttonboxes and Displays

The following functions are expected to be mapped on the steering wheel:

* Brake bias settings
* KERS / Hybrid system controls
* Any push to talk buttons
* Dashboard next/prev buttons

## [Starterbox](starterbox/README.md)

This is a box providing

* Ignition switch
* Starter button
* Pit limiter switch
* Traction control 1/2 selection switch (for GTE cars)
* Rotary encoder for traction control setting w. push function TC off
* Rotary encoder for ABS setting w. push function ABS Toggle (for GT cars)
* Rotary encoder for ENGine fuel mix/throttle shaping w. push function to switch between functions
* LED to indicate selected engine setting (fuel mix or throttle shaping)
* Optional bidirectional serial communication with the simulation (see ir2mqtt)

### [Race display](v2rController/README.md)

Some LED work [V2R controller](http://www.eksimracing.com/help/getting-started-with-eksimracing-vtor-controller/) in conjunction with
an LCD display as additional Windows display.

The functionality is similar to [SIM Race LCD](http://www.simdisplay.net/sim-race-lcd-v3)

### [ir2mqtt](ir2mqtt/README.md)

An application for two purposes:

* Integrate with smart home systems/components which have support for the MQTT 
protocol (e.g. [openHAB](https://www.openhab.org/docs/)
* Send pit service flags and pit service fuel information to a button box using
serial communication 

### [iRacing race control button box](rccbox/README.md)

Inspired by the [Simlogic box](https://www.simlogic-shop.com/home)

![Simlogic Box](images/SimlogicBox.png)

this box provides the following features:

##### Stands section

* Clear tires button
* Switch to select between read / oval
* 2 way rocker switch to select left (rear) / right (front) tires depending on road/oval selection
* Rotary encoder to select fuel refill w. push function to clear fuel
* LED to indicate selected tyre change and refueling in pit (optionally synchronized with simulation by [ir2mqtt](ir2mqtt/README.md) 

##### Black box (UI) section

* Button to select lap timing black box
* Button to select relative position black box
* Button to select radio black box
* Button to select fuel black box
* Button to select tire black box
* Button to select in car adjustments black box
* Button to select pit adjustments black box
* Rotary encoder to select black box value
* Rotary encoder to increase/decrease selected black box value w. push function for value toggle

##### Radio section

* Rotary encoder for voice chat volume w. push function to mute voice chat
* Rotary encoder for radio channel select w. push to mute driver

##### Sim section
* 2 way switch to shift driving view up/down
* Exit button to leave simulation