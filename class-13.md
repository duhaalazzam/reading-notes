# Reading
# “The Past, Present, and Future of Local Storage for Web Applications”
## Cookies
* Web applications need a storage Area, Cookies was invented for this reason to store small amount of data.
* but cookies has three disadvantages:
1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.
* What we really want is:

1. a lot of storage space
2. on the client
3. that persists beyond a page refresh
4. and isn’t transmitted to the server
Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.

## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5
* In the beginning, there was only Internet Explorer.
* Microsoft invented DHTML Behaviors, and one of these behaviors was called userData.
* userData allows web pages to store up to 64 KB of data per domain.
* In 2002, Adobe introduced a feature known as Local Shared Objects.it allows Flash objects to store up to 100 KB of data per domain.
* In 2007, Google launched Gears,Gears can store unlimited amounts of data per domain in SQL database tables.

## INTRODUCING HTML5 STORAGE
* So what is HTML5 Storage?
1. it’s a way for web pages to store named key/value pairs locally.
2. within the client web browser.
3. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. 
4. Unlike cookies, this data is never transmitted to the remote web server.
5. it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

## USING HTML5 STORAGE
* HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.