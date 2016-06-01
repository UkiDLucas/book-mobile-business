# BEST PRACTICES

## UX and UI standards

### Define Style Naming





I don’t want to re-iterate the existing and very good documentation available for both Apple iOS and Android devices, but included are few tips that may not be voiced in official websites.

### Clarity of code over Performance

Very often developers and architects get into very academic (useless) discussions about a virtue of, for example, using Android RelativeLayout over LinearLayout to save on one UI element per record. The problem here is that RelativeLayout is much less readable and easy to understand than
LinearLayout which may cause maintenance problems and poor graphic design. Also, the savings are minimal because we talk about couple of dozen of records and if you are displaying thousands of records you should change approach. I would be willing to sacrifice 1/1000 of a microsecond of performance for greater readability in this particular case.

## Using Correct Input Types and Keyboards

Android provides developer with wide variety of input types and associated keyboards that help users with the task, the list below is very self-explanatory:
date
datetime
number
numberDecimal
numberSigned
phone
text
textAutoComplete
textAutoCorrect
textCapCharacters
textCapSentences
textCapWords
textEmailAddress
textEmailSubject
textFilter
textImeMultiLine
textLongMessage
textMultiLine
textNoSuggestions
textPassword
textPersonName
textPhonetic
textPostalAddress
textShortMessage
textUri
textVisiblePassword
textWebEditText
time

## Technological Debt

Very often the project in the corporation goes like that:
1) big boss sets a grandiose vision, everyone is excited
2) idea of a really cool project is born, often with use of external
“creative agency”
3) management wants a “quick win” so they set some “aggressive”
deadlines
4) a product manager is appointed, she gets the vision documents and
the impossible deadlines
5) the corners are being cut to make the deadline
6) the product has to be “cross platform” and since web developers are
plentiful the UI gets compromised as well
7) the creative company is ashamed, the UI stops talking to engineers
8) product gets delivered, turn over is high, everyone looses interest
9) users hate it, product looses further funding
This sounds like a script from a techno-horror, but as consultant I have seen it over and over, but that is not the worse part because what management does not realize, is that with all that rushing, in addition to loosing clients, motivation and time, they did not make any progress, nor improvements in fundamental technology. Quite opposite, because of patchwork of hacks and kludges they developed that is called a “technological debt” which is destined to be never repaid, as nobody every heard about “going back to take time to do it correctly this time”.
Content & Navigation - Principles
Q: What are the best practices to display content and navigation on
mobile?
• follow the operating system specific guidelines
• don’t cover content with hand, or widgets
• use device physical size and orientation
• design for large tablets in landscape
• consider physical keyboards
• differentiate Apple from Android from Windows Mobile
• the content provided will define the design
It is important to follow the guidelines, especially from Apple, or your app may not be accepted. Consider if you want user to cover the content with their hand, if not don’t put the selections on top. Consider the physical size of the device and orientation, if user holds the device usually in one hand and select with the other, you should make it easier to do so.
Consider that user often use thumbs in landscape on tablets, place the selections lower within the reach. Consider that many users like to use physical or Bluetooth keyboards, don’t force the virtual keyboard usage.
Android user in most cases do not like Apple look-alike functionality, the menu works differently, navigational buttons should be utilized, the settings should make the app easy to use and flexible to customize.
Content Prioritization
For dynamically generated pages, it is a good practice to prioritize content in database in at least two* of the following:
• *full site, 12 inch
• extra large tablet, 10 inch (1200x800)
• large tablet, 7 inch (1024x600)
• *high resolution phone, 4 inch (960x600, 800x480)
• medium phone (480x320)
• small phone (320x240)
If the budget does not allow for it, all devices above 1024x600 should be considered as a full resolution screens.
User-Customized Content
Another way to display less content on the mobile device is to customize the content for the particular user more aggressively on smaller devices. So for examples on the Web page we might display article, several related products and advertisements, on tablet we may go to article without additional content, fewer related products and less advertisement and on the phone we may display just the article, one suggested product and one ad banner. In each case the viewing experience has to be smooth, fast and well designed.

Columns on display
In a similar fashion to limiting the content on mobile devices, the number of columns should adjusted:
• full site: 3 columns
• extra large tablet: 2-3 columns
• large tablet: 2 columns
• high resolution phone: 1 column
• medium phone: 1 column, limited content
• small phone: 1 column, very limited content
• Placement of Navigation
The content should always be displayed towards the top, and the links to navigate to the other pages placed under the content. On iOS devices the placement is limited by the guidelines. On Android devices it is usually a mistake to place too many menu items on the screen as Android users have a dedicated button for that. This principle is however not followed even by Google who in Gmail place the annoying buttons right on the page.
Logout button on every page
It may be a requirement for your commercial application that uses payments that you include “log-out” button on every page, your UX should keep that in mind.
Search button & Voice Commands
The search button is gone, so much for idea of everyone using “voice commands”.
I tried voice commands for a while but honestly I never liked the idea — it annoys people around you, and it is as difficult as selecting by hand while driving - which of course I never do.
More and more manufactures are not including the physical SEARCH button, and it looks like Google gave up on the idea in apps like Market where the search magnifying-glass icon is prominently on top. Also, the
Android 3+ tablets are missing all the physical buttons, which I personally miss a lot. Samsung Galaxy 7 tablet has all 4 buttons, but Galaxy 10.1 already does not have any.
I think as the voice recognition improves the button may come back, but for now only simple commands work and Google Voice mailbox is sometimes comical, everyone call me and says “Hello Auntie!”

Multiple Navigational Menu Items
On many websites it is common to see multiple buttons across the top of the screen that are easy to click with a mouse, on mobile this should be replaced with a drop-down, or selection list type of widget. Placing several small buttons next to each other is a big design mistake on the smaller displays.
Ins and outs of Android Options Menu
The standard Android Menu is one of the most common elements of an Android application, and provides users a familiar way to perform actions. It  contains a collection of primary options and functionality which shows up when the user touches the MENU button on the device.
In this section we will explore how to make this simple item of Android user experience perfect.

Step 1. Create a menu icon
Open Photoshop, create a file with canvas size 72x72 (Notice: always
start from the larger size)
Create your shape using Pen tool (P), or if you have it ready in some vector format paste it as a shape into your document. For the sake of sharpness it is important to use the shape tool and to adjust it, by moving its nods so that the margins fit to the pixel grid.
Scale it to 48x48 and center it. Keep this size for more square icons but make them a little bigger in case you have a custom shape icon so they will appear visually approximately the same size
Apply the following layer styles
Save it as *.png
Scale and save the icon for mdpi (48x38) and ldpi (36x36).
Note: The menu icons are not the case to improvise. The better we follow the guidelines the better and crisper they will look. I advise you to download the Icon Templates Pack - where you can find the PSD template for every screen size. Create your shape in Illustrator, paste it in the PSD template, copy the layer styles from the template layer and paste it to yours. Voila, you got the icon.

Step 2. Copy the icon to an existing project Import (Checkout) an existing project in Eclipse IDE (see Software
Installation and set up for Android Development). If one is absent you might want to download an open source application.
In the project explorer take a look at the resources folder (/res/). Its content is of the most interest to us, designers.
Notice that we have a lot of drawable folders in which reside all our graphical assets as well as elements/shapes drawn in xml which we will explore another time.
When an application is downloaded on the device, the app performs a check of the screen size and density and runs using the graphics from the appropriate folder. If graphics for a given device is not found, or it deals with an element shared with all the screen sizes, then the app is looking for it in the default folder .../drawable/.
To import the icons in the project just drag and drop them in the specific folders.
Note: The icon should have exactly the same file name for all the screen densities. After importing you should get the following structure:
/drawable-normal-hdpi/ic_help.png
/drawable-normal-mdpi/ic_help.png
/drawable-small-ldpi/ic_help.png

For the menu icons we will not consider screen sizes, only screen densities.
Step 3. Menu layout
Unfold the ../res/menu and ... /res/values:
In the menu.xml and events.xml, if we read attentively, even without knowing any programming its clear that we have a <menu> which contains
<items>. android:id=”@+id/about_us” - is the name of the activity/functionality that will be started when we tap, until you do not get very comfortable with the programming part its better not to make changes here.
android:icon=”@drawable/ic_help” - notice that even if the icon is placed in different folders, we do refer to the “/drawable”, this is why it is so important to keep the same filename for all the desnsities.
android:title=”@string/home_about” - in the image of the folders above, in the values folder there is a strings.xml file. This file stores all the strings (titles, notification messages, etc.) we might need including the title of the menu elements. Notice that in the <menu> we refer to string title and not to its content. Knowing this you can change the content or correct spelling yourself.
Note: Having an existing project with at least one menu item you should be able to add as many of them as you need to test. Just make copies of the <item> inside the <menu> in the xml menu file, and make sure to copy and create strings for the item title as well. As for android:id, you can copy the same value in all of them as our goal is to test the look of the icons and we do not care about the activity that follows, just be careful not to commit your experiments. If you want to temporally remove an item from the menu you can comment it out by selecting it in xml file and pressing command
+shift+C.
Step 4. Run and test the application right click on the project and choose Refresh connect the device to the computer or set up your emulator right click on the project, select Run and choose as Android Project
Success!
Keyboard Usage
Most of the phones and tablets are using the virtual on-screen keyboards which make typing more difficult even with use of Swipe/SlideIt enhancements. When designing your application you should however consider phones that have the physical, or bluetooth paired keyboards and utilize the display accordingly.
Please keep in mind that the type of virtual keyboard should be adjusted depending on type of input:
• text
• numbers only
• Internet addresses
44 of 88 pages

