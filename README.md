# Weather-Dashboard
Week-06 homework

See the deployed app here:https://nekohawke.github.io/cmcd-wk06/

# Challenges, Opportunities for Improvement

This app was created using the Open Weather Map data API.  In order to get all the information needed, a good deal of manipulation of the response from the get request was needed, including taking information from one response to generate a new request.  For example, the initial search based on city name returns latitude and longitude coordinates, and these coordinates are used in the UV Index get request.

Another technology used in this app is the javascript Date object.  In order to display dates on the current condition and forecasts, the timestamp returned by the Open Weather Map response is converted into a Date, then the getDate, getMonth, and getFullYear methods are used to generate the date strings displayed on the page.

One problem with the app is if the Open Weather Map fails to find a city that matches what the user typed, no feedback is provided to the user.  I tried to write code that displays a message if a 404 error code is returned, but the javascript just doesn't execute, so the only way to know when that happens is the error message logged in the console.