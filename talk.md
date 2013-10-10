
*** 
Intro Slide with Agenda
***
Roberto From 3VOT
My Name is Roberto Rodriguez Artavia, I am the founder of 3VOT Corporation, we build Web & Mobile App Stores. 

Today I am going to talk about 2 things
1. Explain why we built an App Store
2. Show you how to run your own App Store with our technology

We have an amazing opportunity to get to know each other, I am really interested on hearing what you think about all this; So go ahead, and engage in chatter, twitt me any time and send me an email. This is my thing, and I love talking about it.

***

This is the reason I built the Rodco App Store, but in 2003 I didn't set out to build an App Store. I just wanted to replace our legacy software with something better.

Replacing legacy software with new trends in technology is easy, what's really hard is figuring out what's actually better for business.

With my experience as CTO of Rodco, iterating around business software for over a decade I invented an Enterprise App Store. And I think it's better.

Recently I founded a company called 3VOT, we want to share the Enterprise App Store Technology with every organisation that want's to innovate; and if you run Salesforce is super easy to get started.

But hold on, let me tell you the story from the beginning. 


***
3VOT Slide with quote
***

When I was choosing Rodco's Legacy Software replacement, this came to mind:

If 100 companies buy the same software from Microsoft, and software defines how business operates how are any of them going to have a competitive advantage with each other.

Think about this, the startups that vanished Kodak, the companies that re-invented the travel, music, movie and communication industry. They all have one thing in common: They build their own software; 

Would they have been able to innovate like that without having control over their software, testing, changing, adapting everyday.... no way. 

Succesfull organizations build their own software, everyday!

***

It depends on the source of your statistic, but in 2007 50& to 70% of all CRM Projects failed.

That same year Steve Jobs launched the Iphone and quoted Alan Key on it's keynote.

People that are really serious about business, should build their own software. 
@rodriguezartav forked from Alan Key

I think people that are serious about business, build their own software; everyday!


***

When I first saw the App Store and the Iphone, everything instantly made sense. 

You wanted to do something, so you find an App for that.

One App does one thing, and another App those another thing. 

An App has an specific purpose, and that made perfect sense.

Then I looked at the software we were building, filled with features that nobody used, and toolbars, and menus, and context menus; 

You need to read a huge book and train for 3 months to learn how to use business software.

So I taught, What if I turned each business process into an App?

Can you think about a business process in your organization that you would want to turn into one app. Come on, post it on Chatter. Let's get a conversation started

What would happened if you turned each process into an app, and build a Platform to deploy those Apps, let's call that an App Store.

***

This is what I built, Lean Style, with very little budget, no team and no graphic designer. Just me and a keyboard.

It was ugly, yes. But Awesome. It really changed, the way we work. It re-wired Rodco from the inside out.

I was amazed to see how such a simple thing, like building a process into an app had such a big effect. 

***

Yes Usability, this is a Single Page App. Like Facebook and Twitter, no page refresh, no click and wait, no window pop-ups. So everybody was super happy to be able to fly trough the UI, they could get things done faster!

But also business involvement. Since we talked in terms of apps; bugs, features and ideas where really easy to discuss. It's just an app we could build or destroy in no time.

It's really easy to get everybody aligned, when we talk to managers we say: We are planning on building an app for that; And it's easy for them to get involved.

When we get our team togheter, we tell the project manager imediantyl understands, the web designers, developers. It just made sense, we are going to build an app for that.

Suddenly Management and Executives came to me and said: Hey what if we build an App for That?

It was a brilliant idea that would cut down cut down billing costs in 15%, another one to cut down shipping times by 48 hours.

Our salesman on the road had access to prices and inventories, and could record orders even when they had no internet. We reduced order processing time from three days, to seconds.

Ahhh, it was so exciting!


***

R1 App Store runs 100% on Javascript, both Frontend and Backend on NodeJS and connects with Salesforce via the Rest and Apex API.

The first time a user visits the app, NodeJS renders the UI and sends the complete Single Page Application to the user. After this the user gets a Single Page Experience and can use the App even when there is no internet.

NodeJS also handles Authentication with Salesforce using oAuth and keeps session information.

Each action the users takes in the UI is sent using Ajax to the Backend NodeJS Server, after attaching salesforce security tokens the request is forwarded to salesforce.


***

On the Frontend we used a MVC Framework called SpineJS, it's amazing and we have a great relationship with the author of the Open Source Framework.

SpineJS brings CommonJS to the Client side, a technology that allows us to organise our application in a better way. For us code organisation and management is key, since we are handling multiple apps inside one App Store.

SpineJS also has the regular features of Two Way Binding and Events; it's similar BackboneJS and AngularJS, however I find it a better fit for Enterprise Apps.

The Ajax Component is essential because in order to build amazing apps, our developers must be able to easily send, receive and store salesforce data without worrying about any specifics.

The Salesforce Model also place a key role in this area, for example removing the __c from Custom Objects and removing any other salesforce specific idiom that breaks apart from modern Frontend Development in Spine, Backbone, or AngularJS.

***

Basically we need to be able to do this:

Get access to our Models from anywhere and query our Saleforce.com Data.

Wait for the Data be sent to us, and refresh our UI with it.

But it needs to be super simple, if not; Our developers won't be able to build UI that turn a complicated process into something we actually enjoy doing.


***
An app is a just module like everything else, A Spine JS Component you can bind to any element in the HTML DOM.

Everything is a component, in R1 we used a big IF to select which apps belong to which profiles, we have fixed that on R2 in a much better way

Finally the App Store was compromised of Frontend and NodeJS Backend Proxy, and we used Heroku amazing deploy service to push changes with one command.

***

All this is very important because when we build apps or even when we built the App Store we had to focus on much more complex things, so our framework had to work for us.

The security mananger choose which profiles can access what Apps, and decided what data to load or refresh at start up,

The Layout Manager handles the instantiation of Apps, UI transitions and also the release of Apps when they exit. This is very important because Javascript is a memory leak with legs

The Real time manager is really cool, it registers to Socket Channels and update data on Realtime. For Social, Chat, and Integrated Processes

The Connection Manager handles session times and makes sure all non-real time data remains updated by querying frequently.

***

We managed to improve user Experience by experimenting with many many Apps, slight changes, feedback from users, revolutionary ideas. 

We pushed for User Engagement by providing a Real Time experience, where users always had in mind they where part of a process 

An enabled communication, mostly based on Chatter. But most importantly we created visual apps, we did not know at the moment. But in R2 we have expanded Visual Kanban Apps , Trello Style, to a whole new level.

On The Development Part we were free to innovate in any way we wanted.

We could build apps in days, complex business strategy changes just made us build a new app and replace the old.

We could deploy changes in minutes, and with heroku we could also rollback a change in seconds for those monday morning deploys without enought coffee.

***

But R1 was build for Rodco, for its requirements, data consumption, and user base. We did not leave any space so we could adapt it to another company.

R1 Javascript App is huge, 1.5MB or even more. Because we packed everything into one file Rails 3.1 Style. Even the stuff we did not need when the app launched, and the Apps that were not going to be used by a profiles 

R1 is not 100% responsive. It's easy to make a web page with a some links on the header and a side bar responsive. But such a complex and large application, it makes little sense because sooner or later you will start degrading the experience of every device on the name of the holy grail of responsive web design.

Finally, R1 is not truly scalable. We can Scale with Heroku but our session management and Salesforce API Limits won't let it scale.

***

Today we are introducing R2, an amazing product built for salesforce.com.

We have used all of our experience to correct R1 limitations.

For instance, R2 introduces Dynamic Loading. With an incredible Build Process that allow us to progresively load different parts of the apps as we need them and only send the Apps each user profiles is going to use.

We expanded Responsive Web Design and call it Objective Web Design. Because now we can built an App store for the Web , one for Tablets and one for Mobile, as if we were building a Lego. Since we adopted 100% component based design, we just tell the build process which components to use for web, tablet and mobile. 

Even better, we can build apps specific for mobile that only show on mobile phones; or apps that only show on web & tablet. Anything we want.

Our design is now infinitly scalable using CDN's to push our application assets to the outter rims of the internet, making is insanly fast to access.

Our Build process is key and is controlled by each developer on a simple text file, so we can really assemble the app store and it's app like lego.

***

R2 uses the latest Salesforce advances so in 3 steps you can have an App Store.

First install the connected apps so every user can login to R2

Then , as Platform Admin Login to R2 using your Salesforce Credentials

And finally Build and Deploy your Apps to your App Store

The best of all is free to develop on Salesforce Sandbox and Testing, we do have a great pricing model for renting or purchasing the App Store Technology.

***

This is R2, and amazing platform that lets anybody that knows about javascript apps to build Apps for Salesforce.

Each App Store is independent, they only show the apps for each organization, each profile and each device like web, tablet and mobile.

It's build on the Kanban Approach, Trello Style of visual cards and it's got all the awesomeness of R1 Realtime features.

***

So let me show how to build an App.

The first two steps to use R2 as easy.

First click the Link to R2 Connected App, this will take you to your Sandbox where Salesforce will setup R2 Remote Site Settings instantaneously

Then visit R2 and login with salesforce credentials.

Easy, yes! 

Well building an App is even easier!

***

R2 is 100% Javascript, HTML and CSS so that's all you need to know. We can finally get developers from the largest developer community in the world. Actually we can help build Apps as well.

R2 development enviroment is based on Grunt, the most famous Javascript Tool out there. That lets you automate everything, our development process is so cool that we even got Live Reload, so when you make a change in your code, the browser reload automatically showing your change.

R2 is also build, tested and deployed from the Command Line, so its blazing fast to work. Really when a developer is able to do it's job simply from the command line, he'll never go back to IDE's or Visual Programming. Is just right!

***

So here I got a video that shows how to build an App

First we got our default App Store with Two Apps. We want to build a third and will use our tools: The Command Line or Terminal and a Text Editor.

So Let's see, we type grunt app --name=newApp. And that's it R2 takes care of building the new app.

So we still got two apps in our store; All we need to do now is configure our build process to include it for our profile. 

My Profile is Marketing User, I am just adding the Path for my app and I manually run my build process for my app and refresh my browser.

Voila, my App is there.

***

So now lets actually do something with this app, to show you how easy it is.

First we got our 3 apps, and our new App only has placeholder text.

Next we need to create a model that represents a salesforce object. So let's build that.

R2 also helps us build a Model using the command line. Using grunt model and this time we are creating an Account Model.

The only thing we need to do is go to model on its folder and tell R2 this is a Standard Object. 

R2 takes care of everything, Ajax and any translation from standard front end mechanics.

So let's head to our Actual App and use the Account Data in our App.

First we need to include the Account Module

Then tell R2 to fetch and query the data from salesforce

We need to adjust the layout of out App, and here we are using a stock list layout.

Notice the placeholder were we are going to show out Account Names. Is prefixed js and called js-list

We are going to build a template for each account, many ways to do this; So just create a new file and in it's layout we are going to show each Account Name.

Finally we need to tell our App to refresh it's account list every time we get data from salesforce. And this is the way to do it.

We are telling R2 that when we get Accounts, to refresh the js-list element with our accounts as specified on the template file.

And that's it, that's all we need to do.

As you can see in the background, our browser refreshed automatically. It's called Live Reload, let's check it out.

click on our app. and voila. We got data from salesforce.

It's so easy that we managed to build an App in under 3 minutes, imagine what we can do in 7 days.

***

Now let me show you how to deploy an App.

Remember where we configured our app when we created it, this is the way we configure our whole build process, it's automated and very specific. 

Check out how the apps for the marketing user are named apps_marketing_user and are located in a folder with my OrgID. Here I got all the other parts of the apps, assembled like I told my build process to do it. Just like Lego.

So all in need to do is deploy my apps and components to R2 Platform, so they can be CDN'ed. I do that from the Command Line too.

Is very simple, simply type Grunt Build and you can watch you whole process run, including all your tests. Finally every asset is uploaded to the cloud and pushed to the CDN for maximun speed and infinite scalability.

So now our new App is live and blazing fast. Isn't this amazing!!!

***






