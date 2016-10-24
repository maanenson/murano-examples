# Murano Lock Example

This is a self-contained example of a smart lock device, intended to provide developers an example of using Exosite's Murano platform for some common use cases. It contains code simulating both the smart lock firmware, the cloud event handlers, and the application UI. Here's a demo:

TODO

It is designed to illustrate the use of Murano to build connected products and applications, including:

1. **Device data logging** periodically log the battery level of the smart lock, and update a web app in real time using the Websocket services.
2. **Device control** remotely unlock the smart lock.
3. **User Access control** show how to provide user login and role-based permissions using Murano's User and Keystore services. Additionally show how to aggregate locks into dwellings (e.g. home and garage) that contain multiple locks. 

In contrast to Exosite's home automation example (aka "lightbulb example") this removes any JavaScript UI framework, so that the Device API and Solution API interactions are highlighted. This makes it ideal for training developers integrating their applications with Murano. This one's for the nerds!


## Setup

TODO


## TODO

- add `_init` that sets up users, dwellings
- add blessings to simulator to show state and requests/responses 
- make simulator load in eeprom (product/device identities that are hard coded)
- make simulator save current state (e.g. battery) 
- pull in a simple UI framework (e.g. bootstrap)
- port simulator to Electron to get native Windows/OSX/Linux installers