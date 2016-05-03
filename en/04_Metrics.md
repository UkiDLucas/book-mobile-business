# METRICS

## Tools

You should investigate tools like:
Google Analytics
Flurry
Crashlytics 
DynaTrace

New Users (Installs)
The Installs / New Users metrics show you how effective your marketing is, to increase this number you could:
• Rename the application with catchy and descriptive title
• Post a better marketing description
• Improve the promotional images
• Encourage people to write favorable reviews
• Encourage people to post 5-star ratings
• Promote the app via social media (Facebook and Twitter)
• Improve viral marketability of the app
Uninstalls
Uninstalls are really bad, they show:
You app does not what is advertising to do: 
Title and description may be misleading
The app may lack needed functionality
Check error logs, people maybe uninstalling the app because they are frustrated with crashes
Allow users to log in with their favorite social media (Facebook, Google+, Twitter, LinkedIn)
Sessions
Sessions is one of the most important metrics. The growth in the graph over time shows that users keep on using the application. 
Session Length
Session Length is specific to your application. If your application is a game, you would expect very long sessions, if the app is a quick reference app you would expect short, but hopefully frequent sessions.
Active Users
A growing number of “active users” shows you that people who downloaded the application keep on using it. If downloads are much larger than active users, even if the last grow, you may still have a retention problem.

Page Flow and Navigation

To understand how your users navigate thru your application will help you weed out unnecessary pages, bad navigation patterns, shift around and consolidate the information.

Events, User Actions and Conversion
This is a favorite metric of any business manager. It allows you to capture the events such as clicks, swipes, selections and text entry and provide multitude of parameters that will help you understand the user behavior.
When logging, many people only track Event Group and Event names, however most of the time you are able to log in additional parameters and their values. The example of it would be 
EventGroup: VideoPlayer, 
Event: VideoPlayFinished, 
Parameter: YouTubeId, 
Value: YTUYTYGFH. 
You can go even a step farther and provide JSON like values to really make a reach report.
Data Collection Privacy Issues 
Do not collect any identifying information about children, in general you should not be able to identify who the child is and where is their location, unless the app is designed for parents to track them.
In general it is also questionable, and I strongly discourage you from collecting identifying information about adults. You can collect info about all users in general and what is their usage trend, but having data that pinpoints an actual person and their actions is a bad practice.
Using Personas to Collect Data
It is a common (however annoying) practice in UX to use Personas to describe customer types. For example John, is a twenty-something trainer, he uses the application in X, Y and Z ways. You can use these user types to group user behavior and find a new ways how they like to solve problems. Some of the functionality can be geared towards specific user types.

Exception and Error Logging
It is most crucial that you weed out and handle any errors, especially these coming from the 3rd party APIs. Not all reporting packages are equally useful in providing the stack traces so you will have to experiment. Business stakeholders are particularly interested to hear on regular basis what are the bugs, which are new and what have you done about them.

