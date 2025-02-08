# **Lab 2a and b, Javascript and Security**
## *Jackson Dubreuil*
### *Friday 7th of Febuary, 2025*

In this lab, I coded in JavaScript, making a base script that could display my web page correclty.  With that, it was also able to make the page interactable, allowing users to input new lines and delete lines on the page.  With this functionality, the page became viable.  As the last little bit, I also used CertBot to create a certificate to validate my page as HTTPS.

![Basic Contructor](/Constructor.png "Constructor")

This first set of code comes from the JavaScript Constructor.  First things first, the class "Task" was made in order to properly set up the design.  From there, the data needed to be formatted correctly, so the toHTML function comes into play.  It first reformats the data into variable that we use in the rest of the lab, then from there has a "< li >" piece of data that formats how they are displayed on the screen.

![Function CreateTask](/CreateTask.png "CreateTask")

This photo now shows the functions I created in order to properly add and store new files.  The code begins by pasring the data, then runs it through the ringer of formatting in order to be of the same data of the other tasks, in other words, it needs to conform to the same guidelines.  From there, it runs through the function "readTasks" which reads through the array and assigns the new task a value in that map.  From there, the data is updated in the storage.  Then the tasks are displayed with the new addition.

![Function DeleteTask](/DeleteTask.png "DeleteTask")

These final functions show how we can remove tasks from the page.  It is quite simple, all that is done is a simple read from the console to find the task that was selected.  From there, that information is passed to the filter which finds the task and removes it.  It then is removed from the storage and the tasks are displayed once again.  A basic UML diagram of all this information is provided here:

![UML Diagram](/UML_Diagram.png "UML")

## Questions 2a

What are two differences and similarities between JavaScript and a previous language you have used (e.g. C++ or Python)? (Think of differences and similarities that are more unique to these 2 languages, not all languages in general.)

Two differnces I noted between JavaScript and other coding languages is that the code is acctually pretty streamlined, often putting mulitple funtions into one condensed line of code unline C++ and python, which often require multpile lines to create a funtion.  The other was that JavaScript was pretty forgiving with formatting unlike C++ and Python.  Two similarities were that the codes funtions were very very similar to those of C++, in that they are formatted the same and call variables in a very similar way, and that functions are called in the same fashion as other codes.

What is the difference between JSON and JavaScript objects?

Javascript objects are directly tied to JavaScript whereas JSON uses strings.

If you open your web page in two different browsers, will changes on one appear on the other? Why or why not?

If I open my webpage in two different browsers, the data will update correctly and that is because the array created is saved over the server and the domain, so when it the page is closed and reopened or updated on another tab all changes are synced.

How long did you spend on this lab?

I spent about 15 hours on this lab, including all debugging.

## Questions 2b

What is the difference between http and https?

HTTPS is different than HTTP because it means that it is secure and has a certificate that encrypts the information and protects the user.

What does the A record do in your DNS domain?

The A record maps a IPv4 address to my reserved domain name.

Which key does the certbot tool send to Let's Encrypt to be embedded in the certificate; the public key or the private key?

The CertBot uses the public key.

What is the TTL setting in DNS, what are the units, and what does it do?

The TTL setting in DNS is how long a packet can exist when passed between two devices, literally meaning Time To Live, before becoming obselete.  The units are seconds, and it makes it so that if a packet is passed but not received it goes away as to not hinder future traffic.

The DNS registrar tool is new this year. What did you like about it? What could we do to improve it? (Any answer gets full credit.)

I really liked how easy it was to use, the instructions were not super clear on what to input beyond the original saved domain, but once figured it was seemlessly used.

How would you incorporate bash scripts in your future?

I would incorporate bash scripts in the future to avoid having to set up a server by hand every time. This would be very handy.

## Skills Aquired
- Advanced coding in:
    - JavaScript
- Modify a series of elements in HTML using JavaScript
- Create a certificate to validate and encrypt information on a site
- Debug code using containers and passes through the code

## Sources

- [HTML Lists](https://markdownguide.offshoot.io/basic-syntax/)
- [Changing Arrays](https://www.geeksforgeeks.org/how-to-creating-html-list-from-javascript-array/)
- [TLS Certificates](https://www.digicert.com/how-tls-ssl-certificates-work)