PDX_ART_TREKKER
===============

An Android app created for the google places API developer challenge. This is a prototype project that can be replicated by any city that desires an Art Trekker app of their own. 

PDX Art Trekker is an open source mobile application built using PhoneGap (Apache Cordova). It is written entirely using HTML, CSS, and JavaScript. PhoneGap Supports a wide range of devices (Android, iOS, Windows, Blackberry). 


## About PDX Art Trekker

PDX Art Trekker lets everyone view Portland Oregon's rich and diverse collection of public art. The app shows you the location of the art along with detailed information about each piece. The gallery feature lets you easily view all the thumbnails and you can save your favorites in a separate gallery. The nearby feature displays the art that is closest to your location. It is a fun way to learn about the public art that surrounds us. 

Check out a video of it in action at: 
* https://www.youtube.com/watch?v=xaRHWuUWkK8

PDX Art Trekker can be found in the Google Play Store:
* https://play.google.com/store/apps/details?id=com.SparkChicks.PDXArtTrekker


## How to build and Art Trekker for your city

### Setup Instructions
1. You will need a public art data set for your city. I have included a Sample.csv file that contains all the fields that this code uses to display details about the art. There are only a few required fields (record_id (just a unique number), artist, title, lat, lng, image_url). All of the other fields are optional. Populate Sample.csv with your cities public art data.

2. This app uses [Parse](https://parse.com/), a NoSQL cloud database, to store and serve the public art data to the app. Create a free account on Parse. Follow the easy instructions on how to create your database. Use the Parse Data Browser feature to import your csv file.

3. Get your Parse API keys (Application ID and Javascript key) and plug them into the top of the application.js file in the project.

4. Get a Google Places API key using the [Google API console](https://code.google.com/apis/console/) and plug that into the main.html file.

5. I use Eclipse for this project to compile the android apk. Google has great instructions on how to get Eclipse and set it up with the android sdk. 
 <ul>
    <li>http://developer.android.com/sdk/index.html</li>
    <li>http://developer.android.com/sdk/installing/installing-adt.html</li>
</ul>

 
6. The last step is to change a few variables to reflect your city.

 <ul>
    <li>change app title from "PDX Art Trekker" to your city's name</li>
    <li>change the default lat and lng from portland to your city's lat and lng</li>
    <li>update the about box info to reflect information about your app</li>
    <li>update the message string displayed to the user when they launch an external URL to reflect your apps name</li>
</ul>

## Data Sets

All of the public art information displayed within PDX Art Trekker is freely available from the [Civic Apps for Greater Portland](http://www.civicapps.org/datasets/public-art). PDX Art Trekker uses a data set provided by the [Regional Arts and Culture Council](http://www.racc.org/). This data set was last updated on November 9, 2010. The PDX Art Trekker is not responsible for the quality or accuracy of this data.

All of the museum and gallery information is provided via the [Google Places API](https://developers.google.com/places/).


## Libraries

The following libraries were used within this application:

* [Google Places API](https://developers.google.com/places/)
* [Google Web Fonts - Ubuntu](http://www.google.com/webfonts)
* [PhoneGap](http://www.phonegap.com)
* [PhoneGap Child Browser Plugin](https://github.com/phonegap/phonegap-plugins/tree/master/Android/ChildBrowser)
* [jQuery](http://www.jquery.com)
* [Mustache.js](https://github.com/janl/mustache.js)
* [app-UI](http://triceam.github.com/app-UI)
* [Parse](https://parse.com/)
* [BootStrap](http://twitter.github.com/bootstrap/)
* [InfoBubble](http://google-maps-utility-library-v3.googlecode.com/svn/trunk/infobubble/examples/example.html/)
* [Google Maps](https://developers.google.com/maps/)


## License
THIS SOFTWARE IS PROVIDED BY APRIL JOHNSON "AS IS" AND ANY EXPRESS OR
IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
EVENT SHALL APRIL JOHNSON OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE
OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
