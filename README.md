Step – 1:

This is the 1st step of the app, which has no data. Hence we rendered an image saying there's no data.
there are 2 buttons namely, 'Get monkeys' and 'Find Closest'

'Get monkeys' button, when clicked will load the list of monkeys. Similarly, 'Find Closest' will find the monkey which is near to us using lattitude and longitude.
'Unfortunately this can't be calculated without loading all the monkeys' data.

Step – 2:
As the closest monkey cannot be found until the monkeys data is loaded, so error will pop up.
"Error!
 No data, please Click the 'Get monkeys' button first"
And user has to click on 'Ok'
Forward to Step - 3
Step – 3:

Here the user clicks on the 'Get monkeys' button and hence the monkeys data is loaded as a list using horizontal and vertical stack layouts.
each item is displayed now.
User can browse all by scrolling the list and for that we used 'ScrollView' by keeping the buttons constant in their position.
All the code for this can be found in the 'MainPage.xaml' file.

Step – 4:

As the user couldn't find their closes monkey previously, now the data has been loaded. So one can now find the closest one.
For this, just need to click on the 'Find Closest' button.
And when the user clicks on the 'Find Closest' button, there's a pop-up that will be displayed
And the use has to click on the given action, 'Ok'.
Step – 5:

In some cases, the user might want to reload/refresh the contents of the page, hence in this step we will discuss about the refresh functionality that was incorporated into the app.
To refresh the page or to reload the contents of the page , user has to just drag the page a little from the top of the screen right above the content starts.
The page will refresh and all the data will be retreived again and shown to the user.
Hence for this, we have enclosed all the ContentView of our MainPage in a 'RefreshView' right after the grid layout starts.

Step – 6:

The user can also go into details of each item. He just nees to click on the respective item (anywhere throughout the horizontal space allotted for that item on the grid), and it will navigate to the DetailsPage.
Until here, we are operating our code in the 'MainPage.xaml' file as all this is the common content.
However, now the user wants to get into the details so we are navigating to the 'DetailsPage.xaml'.

Here, we are starting with navigation so we have to Register our new route to 'DetailsPage' in our 'App.xaml.cs'.
And link our xaml page to display the UI contents.

And in the DetailsPage, will give all the onformation needed 


Step – 7:

When the user clicks on the 'Show on Maps' button, maps app will be opened pointing to the exact location of the monkeys with all the functionalitites that are supported my Maps.


Step – 8:

The user can also cross navigate the entire maps and verify the location that is shown by our app.
