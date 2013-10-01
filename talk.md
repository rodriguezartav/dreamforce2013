
*** 
Intro Slide with Agenda
***
Roberto From 3VOT
My Name is Roberto Rodriguez Artavia, I am the founder of 3VOT Corporation, we build Web & Mobile App Stores. 

Today I am going to talk about 2 things
1. Explain why we built an App Store
2. and show you how to build your own

This is an innovative topic, let's talk openly about it on Dreamforce chatter, no right and wrong here; This is about the future and how we shape it. Post your ideas, comments and questions, It will definitely start a conversation and I promise to follow up.

***
3VOT Slide with quote
***
I founded 3VOT because I believe every organisation should control their own software, you should be able to change it, improve it, innovate every day.

I going to "fork" a quote:

People that are really serious about business, should build their own software. 
@rodriguezartav forked from Alan Key

Think about this, the startups that took down Kodak, the companies that re-invented the travel, music, movie and communication industry. They all have one thing in common: They build their own software; Would they have been able to innovate like that without having control over their software... no way

***
100 companies
***

If 100 companies buy the same software from Microsoft, and software defines how business operates how are any of them going to have a competitive advantage with each other.

We need to build our own software.

How many of here feel like you can innovate with your actual platform. Go ahead and post it on chatter, please tell me why, why not? I'am really interested in knowing what you think!

***
Build it with Salesforce

We all know that Salesforce is the most innovative company of 2013, why?

In essence, I think it's because they believe that we should control our software. That's what Salesforce is all about. They give us all the tools and open up all the data so we shape our software whichever way we want.

10 Years Ago, when I became the CTO of Rodco I decided we were going to build our own software and I choose Salesforce to do it.

I wanted to invent the next generation business software.

***
Next Generation 
***
The single page experience we enjoy today in Facebook, Twitter and the UI of our smartphones. Where every action is available from the Home Screen, we click a button and the screen moves, it's alive with realtime updates, it's just amazing.

Most action don't require page refresh, business users can't wait for the browser to refresh every time they click a button. In 2007, the same year the iPhone was introduced 56% of CRM projects failed, they failed because they suck, people didn't want to use them. 

When I first looked at the Apple App Store, it just made sense. I can choose an App for that, vote for it and share it. It shows up on my phone, I clicked on it and start using it. 

The Apple App Store just celebrated 50 billion downloads. This is a proven pattern. 

What if our business software platform could have the same amazing experience, where everything just makes sense.

Objective Web Design the next step of Responsive Web Design, this is a 3VOT innovation.  Instead of building one version that adapts to different screen sizes; we created the technology to simply build one version specific for each device.

But it does not end there, since we are Appified; When you are on your laptop, you get the Laptop UI and the Laptop Apps, when your on your smartphone; Smartphone UI and only apps build specifically for your smartphone.

I think we have learned the lesson that the customer of enterprise software, is not the CEO, the CIO, the CTO, or any O for that matter. The Cesar that decides, thumbs up or down, is every user.... If we want business software, if we want people to innovate; we need to re-invent the experience of Business Users!


***
Demo
***
This is WHY I invented the Rodco App Store and the response was HUGE

We encapsulated each business processes into an App. Apps appear on the home screen, you click on an App, used it, went back to the Home Screen, click another one. It behaved just like the Smartphone.

Data comes from Salesforce, Salesforce enforces security and roles; Profiles define what apps where shown in each user's home screen.


***
Recap
***

Users loved it, but more than that; It made sense to them.

When we think and talk in terms of apps; everything instantly makes sense to everyone. Executives understand when we talk to them about building an App.

The team, project managers, designers, developers, even users understand when we tell them: We are building an App that's going to do this.

New requirements, business ideas, or process improvements just means building a new App, testing it and replacing it for the old one.

When our business system is made of Apps, then we can innovate with software.

***
Chatter Questions

First, can you change your business software. Build a new feature, change an old one. Go ahead raise your hands if you can, tell us on chatter.

If you could build an App for your organisation, in just a week, don't worry about money, people, deployments. Let's say you could, what would that App do? Talk to the person to your right, share it with us on Chatter.

***
HOW

Here's secret sauce of how we built our App Store, it's got 3 ingredients. We'll cover each with detail.

The First is Web Components. Each part of the UI is encapsulated in a web component.  The Chatter Component, The Menu Component, The Home Screen, everything is a web component.

But what's actually magical, is the each App is also a Web Component. So we can load apps dynamically depending on the device and profile of the logged in user. That's how the App Store work, and why it's so easy to build apps; It's just a new web component.

This technology allows us to organise our app in folders, load components dynamically when we need them, use our Objective Web Design Technology to build specific components for the web, for tablets and for mobile. Each component has it's own layout, css and javascript encapsulated on it's own folder.

The second ingredient is the glue that joins web components into an App and helps them get data from Salesforce. 

This is the RSpine Front-end Enterprise MVC Framework which is a based on SPineJS, a framework similar to backbone. We modified so it's appropriate for the enterprise and that it works with Salesforce.com

The third an final ingredient is a Proxy Server that runs on Heroku. The proxy server main role is to translate salesforce communications into the standard rest patterns that the modern front-end apps expect. 



***
Introducing R2 The Web & Mobile App Store

Today I have something revolutionary to show you. It's a product to build apps and simply make them available to everybody via their own Private App Store. 

It's for every organisation, It's a Web & Mobile App Store that works with Salesforce. 

But it is much more than that, it's a way for companies to innovate with software; A quick way to turn an idea into an app, and the simplest path to publish that app.

It's the future of enterprise computing. 

The Future of Enterprise Computing is about each organisation building it's own software;

***
This is R2

Let me show you the latest version of R2 and explain you how it works. 
















