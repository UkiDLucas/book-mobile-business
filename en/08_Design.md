# DESIGN


Design for mobile isn’t Simple


Native development for phones give you a wonderful opportunity for beautiful designs that match device’s size, screen resolution and orientation, however, unfortunately, this is where most developers drop the ball.
Most companies, including mobile development teams and design agencies, underestimate the amount of work that goes into graphical design for mobile. You should estimate much more time for mobile UI/UX because whereas for the web the developer can “chop-up” the design images once and use the pieces for any display size, for mobile applications the design has to be specific for the target platform with several display resolutions, sizes. Resizing of the original images is a bad idea that ends up in a lower quality product. On top of that in Android you don’t “chop up” the images, but you create a custom, single “9patch” stretchable image, which make life easier, but hardly any design artist I talked to knows what it is, and how to do it.
Common Design Deliverables
• style guide per platform
• UX - wireframe flow of the application
• UI - screenshots
• graphical asset delivery per platform
Apple is not Android
Many companies say incorrectly: “We want a consistent look across all platforms.” which is a very, very bad approach. First of all it is not possible unless you cut corners, and once you start doing so, you already failed.
Blackberry cannot support the richness of iPhone and iPhone does not support features of Android. Windows phones use entirely different approach to displaying content called Metro. Users of each platform are used to different type of experience, forcing outherwise makes for unhappy customers. Each platform should be considered a different media channel with its own rules to follow.
Couple of examples:
If you want to have an alarm app (check out our Shame Alarm app) on iPhone you have to start it and leave it in the foreground -- and that is only one of the many problems of iOS, Google solved it long time ago.
I use desktop widgets on my phone all the time, iPhone may have them soon.
Switching between running apps, I do it all the time bouncing between email and chat and browser and blogger.
I type probably 3 hours a day on my phone, including my blogs, emails, chat, there is no keyboard on any iPhone
I cannot live without the above, and hundred other features users of iOS never heard of.
Let me know what features of each platform you find a must-have.
Who is responsible for providing creative assets?
I am a very strong believer that the designers should provide the implementation of their art which might include the following assets: HTML & CSS, Flex/Flash, mobile layouts, stretchable images, etc. If the designer can come up only with wireframes, or with the static Photoshop images, then they are not doing much favor to the end product.
It is sometimes worthwhile to hire a design firm to provide an idea and creative direction, but each product development team will need an artist sitting together with developers and working together. The practice of throwing the design “over the fence” to technology department, as it is common in many companies will result in a terrible product. If the company considers the mobile product as a long term strategy then the artists should become the core part of the team.
Major Android device sizes
The listing is provided below in order of importance, make sure to approach your development in this order. Only first 3 categories make commercial sense at this time, but with Amazon entering 10 inch tablet market, you might want to extend this to first 4 categories.
• normal-hdpi (most modern phones)
• normal-mdpi (smaller, low-end phones)
• large (7 inch tablets)
• xlarge (10 inch tablets)
• normal-xhdpi (newest phones)
• small (you can consider  ignoring it in USA)
Most sources tell you to create layouts in normal, large, xlarge directories and put graphical assets in ldpi, mdpi, hdpi, xhdpi directories, I don’t subscribe to this method. The differences are huge in device sizes and for example small 3.5 inch phone in my opinion should not share graphical resources with 7 inch tablet just because they both use mdpi resolution displays.
High DPI take more pixels for the same Content Few UI designers understand this, yet it is absolutely essential:
To display the same amount of content on different size devices you do not have to use the same amount of pixels. In general, on tablet you can show the same content using many LESS pixels than on the high density phones.
Think about a balloon that you blow to 50% capacity (phone size) and draw 1 inch square on it, than blow it to 70% capacity (7 inch tablet). At this point your original square is much bigger. You could draw another 1 inch square that would be as easy to see, but you would use much less of balloon rubber to do that (less pixels). Blow up the balloon to 100% of the holding capacity and again the squares got bigger. If you use the same size area of content you will use less pixels on tablets, so exactly same size line of text could be 320px on 3 inch phone, 480px on new phone, 385px on the 7 inch tablet, and only 330px on 10 inch tablet.
Text size Setting
1) You should not use more than 3 fonts (size/color combinations).
2) Text sizes should be set using SP units. They are fairly consistent
between different devices (scale-independent) and take in consideration
user settings.
3) Text sizes such as large header (H1), sub-header (H2), and default
should be set for each device combination.
Always set values in this order, testing each on a real device:
29 of 88 pages
• values-normal-hdpi (most modern 4 inch phones 800x480, 854x480,
960x540)
• values-large-hdpi (most 7 inch tablets 1024x600)
• values-large-mdpi (most 7 inch cheap tablets 800x480)
• values-xlarge (most 10 inch tablets 1200x800)
• values-normal-mdpi (most low end 3.x inch phones 320x480)
• values-small (you can ignore it)
Being lazy on tablets
It is a cardinal sin -- and most of us are guilty of it -- to make your apps stretch on tablets! If you go from HTC Evo to Galaxy Tab 7 it seems that you have only a small area increase between 4.3 and 7 inch screen, but indeed you leave about 60% of the screen unused! On 10 inch tablet you leave 4/5th of the screen unused, this is the area when given a little time and effort your application could make an absolute killing, and differentiate itself from the crowd.
Tablet developer: allow full Website access, or do your homework.
There is nothing more frustrating to people spending $500 to $800 on a new shiny tablet to find out that your app tries to “enhance” your user experience by providing 3 inch phone functionality.
The full-size, mobile safe, site would work quite nice on the tablet, especially with ability to pinch and pan to get to the particular section.
Going a step further, which is actually not that much extra work, is to provide the comfortable experience taking advantage of the vaste real estate of the tablet.
The other day I was comparing Android Gmail applications between 4, 7, and 10 inch screens. The 10 inch was done in nice 2 column layout with small fonts which made easy to view my email content. The 7 inch was nothing, but blown up small phone app, with huge fonts as if Google was assuming all Galaxy Tab 7 users were vision impaired.
The small screen Gmail app wasted a lot of screen with big buttons in editing mode, buttons that should have been in menu with better, more beautiful iconography, I am sure users would learn to press menu really quickly.
Even the Blogger app I am using now has several buttons that take screen space. I assume that Blogger app is used very frequently, so it should be designed for frequent users, too.

