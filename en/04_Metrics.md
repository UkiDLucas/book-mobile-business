# METRICS

Some people, especially the MBA types, could spend whole days in spreadsheets analizing statistics, and they would probably be right. If you cannot measure it, you cannot improve it as the saying goes.

## Tools

The iTunes Connect and Android Console do provide rudimentary metric tools, however you should investigate tools like for extra functionality:

- Google Analytics

- Flurry
- Crashlytics 
- DynaTrace

I have been using all 4 in different mixes on various projects. 

DynaTrace is particularly useful when you are trobleshooting complex server side micro-services architecture and you need to determine the bottlenecks and problem components.

Crashylitics is ve ry good at distributing the builds to different groups of testers and verifying that they are testing and finding what crashes they get.

Google Analytics is good at tracking events such as clicks, or pagepageloads.

### New Users (Installs)

The Installs / New Users metrics show you **how effective your marketing is**, to increase this number you could:

- Rename the application with catchy and descriptive title
- Post a better marketing description
- Improve the promotional images
- Encourage people to write favorable reviews
- Encourage people to post 5-star ratings
- Promote the app via social media (Facebook, Linkedin, Google+, Twitter, etc.)
- Improve viral marketability of the app

### Uninstalls

Uninstalls are really bad, they may be indicating some of the following:

- You app does not do what you advertise it to do 
- Title and description may be misleading
- The app may be frustrating users by being unstable and crashing
- The user experience may be terrible
- Users might have never had a chance to try your app because of a blocker such as login
- Very rarely, but the app may be lacking needed functionality

First start with defining your app: name and short description, if you have a hard time then maybe the app does not have a clear purpose and should be simplified. Once you understand the purpose test (on others) how easy it is to accomplish the main goal the app is trying to solve. Check error logs, people maybe uninstalling the app because they are frustrated with crashes.
Allow users to log in with their favorite social media (Facebook, Google+, Twitter, LinkedIn), do not create custom logins with passwords people have to remember.

### Sessions

Sessions is one of the most important metrics. The growth in the graph over time shows that users keep on coming back to use the application. 

### Session Length

Session length is specific to your application. If your application is a game, you would expect very long sessions, if the app is a quick reference app you would expect short, but hopefully frequent sessions.

### Active Users

A growing number of active users shows you that people who downloaded the application keep on using it. If downloads are much larger than active users you may need to work on trying to entice user to return and use the app.

### Page Flow and Navigation

To understand how your users navigate thru your application will help you weed out unnecessary pages, bad navigation patterns, shift focus around and consolidate the information.

### Events - User Actions and Conversion

This is a favorite metric of any business manager. It allows you to capture the events such as clicks, swipes, selections and text entry and provide multitude of parameters that will help you understand the user behavior.

When logging, many people only track Event Group and Event names, however most of the time you are able to log in additional parameters and their values. The example of it would be 

- EventGroup: VideoPlayer 

- Event: VideoPlayFinished 
- Parameter: YouTubeId 
- Value: YTUYTYGFH

You can go even a step farther and provide JSON like values to really make a reach report.



### Data Collection Privacy Issues 

Do not collect any identifying information about children, in general you should not be able to identify who the child is and where is their location, unless the app is designed for parents to track them.
In general it is also questionable, and I strongly discourage you from collecting identifying information about anyone. You can collect info about users in general and what is their usage trend, but having data that pinpoints an actual person and their actions is a bad practice.


### Using Personas to Collect Data

It is a common (however annoying) practice in UX to use Personas to describe customer types. For example John, is a twenty-something trainer, he uses the application in X, Y and Z ways. You can use these user types to group user behavior and find a new ways how they like to solve problems. Some of the functionality can be geared towards specific user types.

### Exception and Error Logging

It is most crucial that you weed out and handle any errors, especially these coming from the 3rd party APIs. Not all reporting packages are equally useful in providing the stack traces so you will have to experiment. Business stakeholders are particularly interested to hear on regular basis what are the bugs, which are new and what have you done about them.

