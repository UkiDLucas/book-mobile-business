# Trouble-shooting Server Connections

When troubleshooting things like API calls and Mobile Web content coming from the servers we have to consider two groups of causes: "Not able to connect" and "Server errors".

User could be “offline” for several reasons:

- the device is in the "airplane mode" which is programatically detectable and under user's control
- the WIFI radion may be turned off, no cellullar radio present as it is in case of many tablets - the state of WiFi radio is programatically detectable and the action to turn it on is in user's control
- In tablets with WiFi radio only, the raadio could be turned ON, but not hotspot not reachable, or even worse not reliable because of weak signal, the signal is programmatically detectable, however the right action is hard to determine
- Cell radio is ON and working, but being jammed by electromagnetic iterference, in this case the Internet connection is not available 
- Cell radio on, but network not reachable as it might be the case in basements, tunnels, mountains, etc., in this case the Internet connection is not available.
- Cell radio on, connection good, but Internet failing resolve DNS (cannot reach the server)



And separate category is server problems where the device is able to reach the server, but the server does not return the data, or returns the error messages. The Error message can me useful in diagnosing the problem, or coming form "deeper" in the system and unpredictable if the error handling is not done wright.

