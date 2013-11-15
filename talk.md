
*** 
Intro Slide with Agenda
***
Roberto From 3VOT

Hello I am Roberto Rodriguez Artavia and today I will share with all of you; why I believe organisations should build their own software. I founded a company called 3VOT to invent products that help organisations build their own software.

This journey started 10 years ago, when I became CTO of Rodco and decided to build software.

Today I will tell you all about this experience, but first, I'd like to share my contact information, I really like this stuff, so go ahead and publish your ideas, taughts, questions and comments, on chatter, twitter, email, by phone; I'll be sure to get back to each one of you.


SUM: Roberto, Believe Build, 3VOT invent products to build

***

We built an App Store designed for Salesforce.com. But when I was getting started in 2003 I didn't set out to build an App Store. I just wanted to replace our legacy software with something better.

We were locked in by software, we could not change our processes, could not change the way we engaged with customers or the way we did business in general.

Today when I talk to business owners they tell they still have same problem. And it doesn't make sense. 

Back then business software was shipped in CD's; it was hard to modify and update. 

But today that's not the case, there is no reason why business software is not updated and improved every day.



Product we build is App Store, did not set out to build, we were locked, talk to owners, Back the cd's, no reason why not build

***

Today I am going to talk about 2 things
1. Explain why we built our first App Store
2. Show you how to run your own App Store with our technology

Remember to post your comments & questions to chatter or twitter, we have planned for enough time for live questions at the end.


***
3VOT Slide with quote
***

If 100 companies buy the same software from Microsoft or SAP, and software defines how business operates how are any of them going to have a competitive advantage with each other.

I think about the companies that re-invented the photo, travel, music, movie and communications industry.

Would they been able to innovate without having control over their software, testing, changing, adapting everyday.... no way. 

Successful organisations build their own software, everyday!

if 100 companies, reinvented, been abel to innovate?, Andersen Horowits, Successfull Orgs

***

It depends on the source of your statistic, but in 2007 50% to 70% of all Traditional CRM Projects failed.

That same year Steve Jobs launched the Iphone and quoted Alan Key on it's keynote.

People that are really serious about hardware, should build their own software. 
@rodriguezartav forked from Alan Key

I think people that are serious about business, build their own software;



Approach business in terms of apps, sources of crm statistics, steve jobs iphone, people serious hardware, build everyday

***

When I first saw the App Store and the Iphone, everything instantly made sense. 

One App does one thing, and another App those another thing. 

It's simple, everyone on the world understood there's an App for That.

Then I looked at business software, there's no purpose; it's filled with features that nobody used, and toolbars, and menus, and context menus; 

You need to read a huge book and train for 3 months to learn how to use it.

There's a better way to build software.

first saw app store, one thing, app for that, business software toolbars, read huge book, business software in terms of apps

***

Apps has been proven 50 billion times, each app download off the Apple Store and the Android Store validate's this pattern.

I realised Business Software should be approached in terms of Apps, each App represents a task that must be done by one or several people in Realtime.

All those Apps published in an App Store, where everybody customers, partners or employees can use just the apps they need; from any browser or mobile device.


app pattern 50 billion, experiment process into app, somewhere to put apps, really interested app struff, made sense

***

R1 was our first attempt to turn each business process into an App and simply make them available to our staff in a Private App Store.

They used the Rodco App Store from any browser, nothing to install, just login with salesforce credentials.

Each one of them able to see only the Apps enabled for their profile, just click on App and start using it. No training required.


r1 first attemps, make available app store, any browser, no install, login, see all apps by profile

***

It is a Single Page App. Like Facebook and Twitter, no page refresh, no click and wait, no window pop-ups. So everybody was super happy to be able to fly trough the UI, they could get things done faster!

But also business involvement. Since we talked in terms of apps; bugs, features and ideas where really easy to discuss. It's just an app we could build or destroy in no time.

It's really easy to get everybody aligned, when we talk to managers we say: We are planning on building an app for that; And it's easy for them to get involved.

When we get our team togheter, the project manager immediately understands, the web designers, developers. It just made sense, we are going to build an app for that.

Suddenly Management and Executives came to me and said: Hey what if we build an App for That?

It was a brilliant idea that would cut down cut down billing costs in 15%, another one to cut down shipping times by 48 hours.

Our salesman on the road had access to prices and inventories, and could record orders even when they had no internet. We reduced order processing time from three days, to seconds.

Ahhh, it was so exciting!


***

This is the Architecture of the App Store

On one side we got the App Store and the apps that you just saw on the video, with no page refresh and realtime behaviour.

Salesforce on the other end provides the data and security via the Rest API. Profile, roles and every other security permission is strictly enforced by Salesforce.com

There's a NodeJS server that sits in the middle, it's main role is to translate Salesforce Singularities into the Standard Rest expected by frontend frameworks like Angular, Bootstrap and ours. It also helps with user authentication ,sessions and integrating with other systems. Like Twilio for example for voice and sms.



***

The frontends job is to quickly turn ideas into an Apps. 

First, we developed a framework to build apps something that's simple and Open Source like Jquery.

We wanted be able to build an App in hours without worrying about anything else.

Since it's just an App; We can build, modify or replace it without worrying about breaking another part of the system.

Apps are build in the universal combination of HTML and Javascript.

Everything powered by a build system, that let's us integrate, test and deploy in seconds.


***

The first problem we encounter when building Javascript Apps is being able to organise the code. Our first attempts quickly started looking like a fettucini Alfredo with no beginning or end.


We can't write Enterprise Apps like Jquery plugins, we need a way to write and load modules like other enterprise programming languages.

CommonJS is the technology used by NODEJS to organise code in folders and modules, it's pretty good. 

We used it to organise code in files and load them anywhere in our apps with a simple line of code.

The App Store follows the MVC Pattern, Salesforce Object Data like Accounts are represented by Models and it's easy to filter and manipulate data.

Any part of the View can register to receive updates when a model changes, updating only that part of the UI in Realtime when it happens.





first problem building apps is organize code, cant write enterprise with jquery, solution in open source, commonjs , mvc framework stores objects in models, wait for changes and refresh



***


Traditional Web Applications are made of large blocks of HTML, CSS and JS. That why is so hard to build and improve web apps, a change here can break something over there.

Enterprise Software is based in principles like encapsulation and composition; Javascript does not have this out of the box, but it's got unique  powerful features of it's own.

We took the best of both worlds and invented our version of Web Components, which is sooo powerful.

First, every part of the UI is a component; and each component is isolated, decoupled it doesn't know anything about their neighbours. 

Components communicate via events, they register to listen and broadcast events. Events can even be pushed externally from salesforce in Realtime.

It's really cool because now we can group the small HTML, JS and CSS files for each component in a folder; instead of fishing for them in a sea of huge files and folders.

Now that all our files are in one place, we can actually do some real unit testing of each component . It's just right.


***

When you are building an App the most common operation is retrieving and updating salesforce data; it's essential that this is really easy.

Salesforce REST API was not made to work out of the box with Javascript Apps, retrieving and updating data can get really messy, developers would have a hard time building apps.

We designed an AJAX Framework to work out of the box with Salesforce; 

It's awesome, we are able to retrieve or update salesforce with one line of code.


***

The Rodco App Store required us to invent and improve several technologies, we were able to do it by standing in the shoulders of giants in the Open Source Community.

The extreme momentum of today's Javascript Community pushed us to invented our version of Web Components so ahead of it's time, which is finally what allowed us to build apps and the App Store.

You see, an App is just a component thats encapsulated, can communicate with salesforce on one line of code and it's fully testable.

The result is a super advanced App Store, build in HTML and JS, based on Open Source Projects that can be modified in every way.


***

The coolest part of building the App Store was experiencing the connection of business and technology.

Because business and technology working hand in hand is not something you can just do, it's something the happens; all you can do is create the conditions for it to happened.

This is why Gamification is so important, and infographics and kanban apps where people in business can visualise what they are doing.

An believe it or not, Apps and the App Store are catalyst of business innovation. 

In our experience it happend this way, first we improved user experience.

Then we took suggestions, feedback and ideas and quickly turn them into apps.

After a while everybody started thinking in terms of apps, until you get to the point where the CEO comes and says; so I have an idea for an App and it's brilliant, we tell managers, they get it; we tell project managers they get it, designers, programmers; and in a couple of days, here it is, We just changed our industry.


***

This is what I mean when I say that I believe every organisation should build their own software and build it in terms of apps.

I founded 3VOT because I figured out how to connect business and Technology, and I want everybody to be able to do it.

This is how I imagine it:

First, every organisation that uses Salesforce can instantly run their own App Store.

There's an App Toolkit that includes all of our inventions and Javascript Developers can build Enterprise Apps that seamlessly consume Salesforce Data.

All the Security, profiles, roles and permissions are enforced by Salesforce.com

While Administrators can simply make those apps available on your own App Store that runs on every browser and mobile device. 


***

We call it R2 and it's the best way to build apps.

***

The R2 Appstore is available instantly with Salesforce Connected Apps

With one click Admins enable users to login into your own App Store with their salesforce account.

That's it. With one click, you get an App Store; Free to try with Salesforce Sandbox

***


The R2 App Store includes the App Toolkit to build Javascript Apps that consume salesforce data.

An App Store to deploy those apps and simply make them available to all your users depending on their Profile.

User Login with Salesforce to your R2 App Store, and they are governed by profiles, roles and permissions including Apps by Profile


***

Let's take a look at the App Toolkit, it includes the most cutting edge technologies in web development and R2 it's a great way to check them out.

Build Javascript Apps that consume Salesforce Data with one line of code.

Keep code organised, instead of keeping html in one place, css on the other and JS over there. Just create a folder for an app, and keep all it's html,js and css files there. There's nothing else you need to do.

When I invented Super Modular Testing, I was like wowwwwwww; This is really going to make a difference.

Each App and Component can be unit tested individually on a full web environment where you can simulate clicks and such. Just write the tests and choose what components you need; tests run automatically on a headless browser.

The App Toolkit use Responsive Server Side Components, a step up of Responsive Web Design that makes building Apps for Web & Mobile like Lego; You choose which components and apps go for Web, which are used for tablets and which for mobile. It's that simple


***

With R2 you get the App Toolkit and the App Store.

But the App Store is not just an App Store.

R2 comes integrated with Chatter, so the App Store is also a super powerful Social Network.

R2 also comes with tools and apps to show metrics in terms of Infographics, we are pushing our philosophy that Business Intelligence is not just about showing data in bar charts, but actually navigating it's history and do forecasting.


***

R2 comes bundled with an App for Administrators to easily create Apps and assigned them each Profile; so that users in that Profile can only use the Apps enabled by it's administrators.

It's so powerful that you can even choose which apps should show if the user is on a Mobile Device or on a Web Device; This enables developers to create Apps that are target just to mobile devices, web devices or build responsive ones for both.

***

R2 can be used as a Private App Store, as a Public App Store or an Open Data Platform.

But most importantly, it can be used to connect business and technology.

Technology to make business better; constantly improving processes and customer relationships.

Creating the grounds for innovation to occur,

business people and technology people speaking the language of apps

working as a team, dreaming of that moment

where the powerful business ideas change an industry forever 


Try R2, go first and start a revolution today






