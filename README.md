# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (2pts) User sees an app icon on the home screen and a styled launch screen.
- [x] (5pts) User can view and scroll through a list of movies now playing in theaters.
- [x] (3pts) User can view the movie poster image for each movie.

#### BONUS
- [ ] (2pt) User can view the app on various device sizes and orientations.
- [ ] (1pt) Run your app on a real device.

### App Walkthrough GIF
<img src="https://recordit.co/atMrATKQzW.gif" width=250><br>

### Challenge
Installing AlamofireImage has been a huge unexpected challenge. 
Even after cleaning the build and re-building, manually building the framework, 
and deleting the 'derived data' folder, I was still receiving 100+ errors on Xcode, 
mainly two errors: "Could not build Objective-C module 'AlamofireImage'" and 
"No such module 'AlamofireImage'". 
The solution was to specify the version in the Podfile. For my specific case, I add the following, 
and Alamofire (4.9.1) and AlamofireImage (3.6.0) were installed instead.  
```
#Pods for flixster
pod 'AlamofireImage', '~> 3.1'
```
