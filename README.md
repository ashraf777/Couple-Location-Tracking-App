# Track Location
This is a simple android app where you can brodcast your location and everyone who has your dynamically generated unique key can track you in near real-time.

This project is just for learning puposes particularly about firebase (firestore db), google maps api and google location api.

***
### How it works?
![](images/hiw.png)

- The first device get continous location update from gps, network etc. then
- Write and update the location data to a specific firebase firestore document
- Last, the second device read that firebase firestore document and show the marker in that location



