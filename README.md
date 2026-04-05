# Lab 03/04: Abstraction & Polymorphism - Smart Home 💡

### The Scenario
You are building a controller for a Smart Home. You have many different devices (Lights, Thermostats, Security Cameras), but your "Master Controller" should be able to turn them all on with one button.

### Your Tasks
1. **Abstraction**: Complete the `abstract class SmartDevice`. It must have a `private String deviceName` and an `abstract void activate()`.
2. **Implementation**: Create two subclasses:
   - `SmartLight`: `activate()` should print "Setting brightness to 100%."
   - `SmartThermostat`: `activate()` should print "Setting temperature to 72 degrees."
3. **Polymorphism**: In `Main.java`, create an `ArrayList<SmartDevice>`. 
4. **The Trigger**: Add one light and one thermostat to the list. Use a `for` loop to call `.activate()` on every device in the list.

### Why this matters:
Notice that the loop doesn't care if the device is a light or a thermostat. It just knows it's a `SmartDevice`. That is Polymorphism!
