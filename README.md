Step – 1:
This is the 1st step of the app, which has no data. Hence we rendered an image saying there's no data.
there are 2 buttons namely, 'Get monkeys' and 'Find Closest'

'Get monkeys' button, when clicked will load the list of monkeys. Similarly, 'Find Closest' will find the monkey which is near to us using lattitude and longitude.
'Unfortunately this can't be calculated without loading all the monkeys' data.
![Screenshot 2023-09-28 151055](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-sainaveenreddy123/assets/126020966/cf9a9182-bada-4c1f-8f00-36975e0d8e54)

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
![Screenshot 2023-09-28 150748](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-sainaveenreddy123/assets/126020966/c694456d-019b-4d01-ac90-69fdb0a4fa01)


Step – 4:

As the user couldn't find their closes monkey previously, now the data has been loaded. So one can now find the closest one.
For this, just need to click on the 'Find Closest' button.
And when the user clicks on the 'Find Closest' button, there's a pop-up that will be displayed
And the use has to click on the given action, 'Ok'.

![Screenshot 2023-09-28 150831](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-sainaveenreddy123/assets/126020966/d45d6935-1303-40b8-8dcc-892c3d792fdd)

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

![Screenshot 2023-09-28 151204](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-sainaveenreddy123/assets/126020966/e0ef6531-9956-40ab-9d73-05e54016a876)

Step – 8:

The user can also cross navigate the entire maps and verify the location that is shown by our app.

![Screenshot 2023-09-28 150905](https://github.com/Wichita-State-CS797R/cs797r-project1-workshop-sainaveenreddy123/assets/126020966/5b9cea8b-3a56-41c0-ada9-6c0b2e82e746)

