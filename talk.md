
*** 
Intro Slide with Agenda
***
Roberto From 3VOT

Hello I am Roberto Rodriguez Artavia and I believe organisations should build their own software. I founded a company called 3VOT to invent products that help organisations build their own software.

This journey started 10 years ago, when I became CTO of Rodco and decided to build software.

Today I will tell you all about this experience, but first, I'd like to share my contact information, I really like this stuff, so ho ahead and and publish your ideas, taughts, questions and comments, on chatter, twitter, email, by phone; I'll be sure to get back to each one of you.

Hi, believe in build, 3VOT, CTO RODCO, Contact

***

We built an App Store designed for Salesforce.com, and its amazing what we did. But when I was getting started in 2003 I didn't set out to build an App Store. I just wanted to replace our legacy software with something better.

We were locked in by software, we could not change our processes, the way we engaged with customers or the way we did business in general.

Today in 2013 when I talk to business owners they tell me the same problem over an over. And it doesn't make sense. 

In 2003 business software was shipped in CD's; it was hard to modify and update. 

But today that's not the case, there is no reason why business software is not updated and improved every day.



We build an App Store, Didn't set out, locked in by software, 2013 talk to business owners, 2003 ship cds, today not the case


***

Today I am going to talk about 2 things
1. Explain why we built our first App Store
2. Show you how to run your own App Store with our technology

Remember to post your comments & questions to chatter or twitter, we have planned for enough time for live questions at the end.


***
3VOT Slide with quote
***

If 100 companies buy the same software from Microsoft or SAP, and software defines how business operates how are any of them going to have a competitive advantage with each other.

I think the companies that re-invented the photo, travel, music, movie and communications industry.

Would they been able to innovate without having control over their software, testing, changing, adapting everyday.... no way. 

*Andersend Horowits says that if he was a CFO of a company, he would figure how a startup could kill his business with software. Then build a company that does just that, or build the software inside his current company.

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

I started experimenting turning business processes into Apps; and I learned a lot from the early days. 

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


Building, changing, inventing Apps is the name of the game, turning an idea into an App should be easy and even fun; 

First, we built a framework to build apps inspired in JQuery's simplicity. 

Experiments, prototypes or full enterprise apps should be delivered in hours, since it's just one app we could just build, replace or change it without affecting other parts of the system.

We stood on the shoulders of giants in the Open Source Community to be able to do this and developing in HTML, CSS and JS, we became better day by day.

The Javascript Open Source community is really professional and organised; this was great because we learned from them and started building, testing and deploying software with confidence, doing it just like the best developers in the world. 

In the end, we were are able to deploy with one button, and we still push that button many times a day.


framework for building apps like jquery, deliver in hours, context app, destory/build/change, open source moves fast, html js css shoulders of giants, build with confidence,

***

Our App Store's simple architecture is based on NodeJS to seamlessly connect Apps with Salesforce.

As a Frontend Developer I want to focus on user experience of the App without dealing with salesforce singularities. The Frontend is independent, querying and update objects takes only one line of code.

NodeJS helps by abstracting and translating Salesforce API's to the REST Standard expected by modern Frontend Frameworks. It also keeps Salesforce Session Authentication with oAuth.

All secure communications are made via standard Salesforce channels. Like the Rest API. So profile, roles and any other security configuration is strictly enforced.

Salesforce got the conn.


this app simple arch, nodejs backend in middle, developer focus on user experience, query one line of code, backedn modern way, translate api, secure communications by salesforce

***

The first problem we encounter when building Javascript Apps is being able to organise the code. Our first attempts quickly started looking like a fettucini Alfredo with no beginning or end.

We just couldn't write Enterprise Apps with jquery plugins, we need a way to write and load modules like other enterprise programming languages.

CommonJS is the technology used by NODEJS to organise code in folders and modules, it's pretty good. We invented a process to organise code in files and load them anywhere in our apps. 

An MVC Framework stores Salesforce Object Data into Models so it's easy to filter and manipulate data.

The UI can register to receive updates when a model changes, refreshing only a part of the UI in Realtime when it happens.





first problem building apps is organize code, cant write enterprise with jquery, solution in open source, commonjs , mvc framework stores objects in models, wait for changes and refresh



***

Traditional Web Applications are made of large blocks of HTML, CSS and JS. That why is so hard to build and improve web apps, a change here can break something over there.

Enterprise Software is based in principles like encapsulation and composition; Javascript does not have this out of the box, but it's got unique  powerful features of it's own.

We took the best of both worlds and invented our version of Web Components, which allows to program for real in javascript.

First, every part of the UI is a component; and each component is isolated, decoupled it doesn't know anything about their neighbours. 

Components communicate via events, they register to listen and broadcast events. Events can even be pushed externally from salesforce in Realtime.

It's really cool because now we can group the small HTML, JS and CSS files for each component in a folder; instead of fishing for them in a sea of huge files and folders.

Now that all our files are in one place, we can actually do some real unit testing of each component. It's just right.


***

When you are building an App the most common operation is retrieving and updating salesforce data; it's essential that this is really easy.

Salesforce REST API was not made to work out of the box with Javascript Apps, retrieving and updating data can get really messy, developers would have a hard time building apps.

We designed an AJAX Framework to work out of the box with Salesforce; 

It's awesome, we are able to retrieve or update salesforce with one line of code.


***

The Rodco App Store required us to invent and improve several technologies, we were able to do it by standing in the shoulders of giants in the Open Source Community.

This is how we invented our version of Web Components ahead of it's time, which is finally what allowed us to build apps and the App Store.

You see, an App is just a component thats encapsulated, can communicate with salesforce on one line of code and it's fully testable.

The result is a super advanced App Store, build in HTML and JS, based on Open Source Projects that can be modified in every way.


***

Technology is cool, but people are awesome; And the coolest part of building the App Store was experiencing the connection of business and technology.

Because business and technology working hand in hand is not something you can just do, it's something the happens; all you can do is create the conditions for it to happened.

This is why Gamification is so important, and infographics and kanban apps where people in business can visualise what they are doing.

An believe it or no, Apps and the App Store are catalyst of of business innovation. 

In our experience it happend this way, first we improved user experience that the way to a user's heart right; 

Then we took suggestions, feedback and ideas and quickly turn them into apps.

After a while everybody started thinking in terms of apps, until you get to the point where the CEO comes and says; so I have an idea for an App and it's brilliant, we tell managers, they get it; we tell project managers they get it, designers, programmers; and in a couple of days, here it is, We just changed our industry.



***

This is what I mean when I say that I believe every organisation should build their own software and build it in terms of apps.

I founded 3VOT because I figured out how to connect business and Technology, and I want everybody to be able to do it.

This is how I imagine it:

First, every organisation that uses Salesforce can instantly run their own App Store.

There's an App Toolkit that includes all of our inventions and Javascript Developers can build Enterprise Apps that seamlessly consume Salesforce Data.

All the Security, profiles, roles and permissions are enforced by Salesforce.com

While Administrators can simply make those apps available on you own App Store that runs on every browser and mobile device. 


***

We call it R2 and it's the best way to build apps.

***

With Salesforce Connect Apps Technology it's super easy to install.

With one click you'll enable all you users to login to your App Store with their salesforce account.

That's it. Then it's all about building Apps and choosing which users can use them.

R2 is free when installed on a Sandbox Environment, and you may find the link anytime in 3vot.com

***

With R2 you get an App Toolkit to easily build javascript apps for Salesforce.com

An App Store to deploy those apps and simply make them available to all your users depending on their Profile.

Your Salesforce Users  Login with theri Salesforce Accounts and bring in their profiles, roles, permisions and every security measure configure in Salesforce.com

***

The App Toolkit brings all of 3VOT innovations, the technologies in the R2 App Toolkit are so ground breaking and state of the art that it's worth it to play around with R2 just to get to know them.

Build Javascript Apps that consume Salesforce Data with one line of code.

Organise files in a magical way. Html, css and js files for each component and app togheter on one folder. There's nothing else you need to do.

Super Modular Testing possible feels like a dream; With the Toolkit each App and Component can be unit tested individually on a headless web environment where you can simulate clicks, fill forms, etc. Everything automatically. 

The AppToolkit also uses Responsive Server Side Components, a step up of Responsive Web Design that makes building Apps for Web & Mobile like Lego; You choose which components and apps go for Web, which are used for tablets and which for mobile. It's that simple


***

With R2 you get the App Toolkit and the App Store.

But the App Store is not just an App Store.

R2 comes integrated with Chatter, so the App Store is also a Social Network where everything has and profile and can be followed.

R2 also comes with tools and apps to show metrics in terms of Infographics, we are pushing our philosophy that Business Inteligence is not just about showing data in bar charts, but actually navigating it's history and be able to ..... (predict)


***

R2 comes bundled with an App for Administrators to easily create Apps and assigned them each Profile; so that users in that Profile can only use the Apps enabled by it's administrators.

It's so powerful that you can even choose which apps should show if the user is on a Mobile Device or on a Web Device; This enables developers to create Apps that are target just to mobile devices, web devices or build responsive ones for both.

***

Currently R2 is in Beta, it's free to be used on any Sandbox Enviroment.


Your can use The R2 Platform to build a Private, Public App Store, Open Data or any business strategy.



