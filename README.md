# Track Location
This is a simple android app where you can brodcast your location and everyone who has your dynamically generated unique key can track you in near real-time.

This project is just for learning puposes particularly about firebase (firestore db), google maps api and google location api.


***
### References
- [Set Up Google Play Services](https://developers.google.com/android/guides/setup)
- [Getting Started - Google Maps](https://developers.google.com/maps/documentation/android-api/start)
- [Get API Key](https://developers.google.com/maps/documentation/android-api/signup)
- [Add Marker in Maps](https://developers.google.com/maps/documentation/android-api/map-with-marker)
- Firebase Documentation (Guides) ([Link](https://firebase.google.com/docs/guides/))
- [Get Started with Firebase Firestore](https://firebase.google.com/docs/firestore/quickstart)
- [Firestore Data Model](https://firebase.google.com/docs/firestore/data-model)
- [Firestore - Get Data](https://firebase.google.com/docs/firestore/query-data/get-data)
- [Firestore - Structure Data](https://firebase.google.com/docs/firestore/manage-data/structure-data)

***
### How it works?
![](images/hiw.png)

- The first device get continous location update from gps, network etc. then
- Write and update the location data to a specific firebase firestore document
- Last, the second device read that firebase firestore document and show the marker in that location


***
### Hot to integrate Google Maps & Location API
To use google maps in an android app you can use `SupportMapFragment` or `MapView`

- Using google maps fragment (inside a layout or as a root tag)
 
```xml
<fragment
	android:id="@+id/map"
	android:name="com.google.android.gms.maps.SupportMapFragment"
	android:layout_width="match_parent"
	android:layout_height="match_parent"/>
```

- Then you have to add permissions and google maps api key in the *AndroidManifest.xml* file


