# Local Storage


**localStorage is a property that allows JavaScript sites and apps to save key-value pairs in a web browser with no expiration date.
This means the data stored in the browser will persist even after the browser window is closed.**


Where is localStorage stored?
In Google Chrome, web storage data is saved in an SQLite file in a subfolder in the user’s profile. The subfolder is located at \AppData\Local\Google\Chrome\User Data\Default\Local Storage on Windows machines
and ~/Library/Application Support/Google/Chrome/Default/Local Storage on macOS.




# A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think.
To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars,
Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData.

userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.
(Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.)
IE does not present any form of permissions dialog, and there is no allowance for increasing the amount of storage available.

In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.” Within the Flash environment,
the feature is properly known as Local Shared Objects. Briefly, it allows Flash objects to store up to 100 KB of data per domain.
Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System),
but it was limited by some of Flash’s design quirks. By 2006, with the advent of ExternalInterface in Flash 8,
accessing LSOs from JavaScript became an order of magnitude easier and faster. Brad rewrote AMASS and integrated it into
the popular Dojo Toolkit under the moniker dojox.storage. Flash gives each domain 100 KB of storage “for free.” Beyond that,
it prompts the user for each order of magnitude increase in data storage (1 Mb, 10 Mb, and so on).

In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers.
(We’ve previously discussed Gears in the context of providing a geolocation API in Internet Explorer.)
Gears provides an API to an embedded SQL database based on SQLite. After obtaining permission from the user once,
Gears can store unlimited amounts of data per domain in SQL database tables.

In the meantime, Brad Neuberg and others continued to hack away on dojox.storage to provide a unified interface to all these different plugins
and APIs. By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) Adobe Flash, Gears, Adobe AIR,
and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.

As you survey these solutions, a pattern emerges: all of them are either specific to a single browser,
or reliant on a third-party plugin. Despite heroic efforts to paper over the differences (in dojox.storage),
they all expose radically different interfaces, have different storage limitations, and present different user experiences.
So this is the problem that HTML5 set out to solve: to provide a standardized API, implemented natively and consistently in multiple browsers,
without having to rely on third-party plugins.


![image](https://user-images.githubusercontent.com/85109819/124730397-27598080-dec6-11eb-9855-772b01b375d3.png)



## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

ersistent local storage is one of the areas where native client applications have held an advantage over web applications.
For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data
like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform
convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database,
invent your own file format, or any number of other solutions.

Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history,
and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
Cookies are included with every HTTP request, thereby sending data unencrypted over the internet
(unless your entire web application is served over SSL)
Cookies are limited to about 4 KB of data — enough to slow down your application (see above),
but not enough to be terribly useful
What we really want is

* a lot of storage space
* on the client
* that persists beyond a page refresh
* and isn’t transmitted to the server

