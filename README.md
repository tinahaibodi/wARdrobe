# wARdrobe
An iOS application that uses AR to enhance the movie-goer experience for AT/T's Hackathon 2018.

## Inspiration
There's something about the childhood experience of wanting to step into a movie like Lucy from Narnia; the way she simply opened the doors to her wardrobe and was given access to a whole new world.

Watching movies in theaters currently is exciting - but figuring out which movie to watch? not so much. We thought about different ways to improve the selection process and found that visuals were key in helping immerse. Because of this, we created wARdrobe, an augmented reality app that allows you to physically step into scenes of different movies, then find showtime information if you have found your ideal movie theater.

## What it does
wARdrobe is an iOS movie application built using Apple's ARKit. On opening the app, there is a camera view in the room. Upon tapping, there will be an augmented reality "portal" to another movie scene, where you physically walk inside another "scene" and view a gallery of AR scenes from the movie. If interested in information about seeing the movie, there is a pull-up information section where a user can find relevant flight showtimes and location information.

## How I built it
We built wARdrobe with Apple's iOS ARKit, a Flask server hosted with Microsoft Azure, the Microsoft Bing Image Search API, CocoaPods, AlamoFire CocoaPods, and the WolframAlpha Simple API. We combine all of the information with the AR to create a comprehensive visual display with helpful information. The Flask server takes in a city/location name, and it processes that string with many APIs to extract information—starting with the Open Movie Database. We hit the OPM endpoints with our location to gather information on popular movies nearby, showtimes, and other general movie information. We then integrate the “popular movie” into the Microsoft Bing Image Search API to get a list of image urls that will be displayed in the iOS application. Following, we use the WolframAlpha API to get information on the population.

## Challenges I ran into
As noted below, we came across challenges when learning how to integrate Azure and Cocoapods into ARKIT. As the integrations with AR Kit are farely new and there is limited documentation on ARKit using Cocoapods, we struggled to integrate the SwiftyJSON and AlamoFire cocoapods into the application.

Upon first making the application, we tried to use Microsoft Azure and OpenCV to integrate video frames of the movies into the Augmented Reality application as well but since there is limited documentation on it (since it has never been done before) outside of MatLab, we would love to revisit the idea and integrate the feature in the future. One of the problems that we came across upon development is the dependencies in software and the fact that the frames would have to be imported in singularity through OpenCV because integrating MatLab with Apple's AR Kit did not allow for logical testing.

## Accomplishments that I'm proud of
We're super proud of the ability to create a tangible marketable solution that will help engage occasional movie-goers and increase the number of purchasing movie tickets per year. With streaming movie services now dominating the movie industry with an increase to 22% in 2017, we felt that having a creative solution using AR was necessary to showcase the importance of seeing movies in the theater. The theater experience allows you to fully immerse yourself in the movie and another world - without distractions and that's what we hope to remind movie-goers with this application. That they can always open the wARdrobe to step into their favorite movies if they please.

## What I learned
We learned how to integrate Sketch components, Microsoft Azure, and CocoaPods into ARKit using XCode. We found that since AR is fairly new there isn't a great amount of documentation on using Cocoapods with AR which made it difficult to integrate the different components.

## What's next for wARdrobe
The future vision for wARdrobe is creating 3D movie scenes that are almost indistinguishable from reality - immersing potential movie-goers into their prospective movie. Imagine stepping into the newest "Batman" and being able to view Wonder Woman and Batman fighting in detail right in front of you, the interactions of the environment, and experience all of the things they do in the movie - right from your home. We would also want to expand this experience by making it social. It would be great to see which of your friends have seen a movie in the past and also to take inspiration from other people's movie experiences.

## Built With:
ar-kit -
flask -
cocoapods -
azure -
alamofire -
bing -
wolfram-technologies 
