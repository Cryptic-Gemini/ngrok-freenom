# ngrok-freenom
Guide to use ngrok with freenom




                                                   Ngrok + Freenom




Part:A
------
 

Enter ngrok, a very cool, lightweight tool that creates a secure tunnel on your local machine along with a public URL you can use for browsing your local site.

When ngrok is running, it listens on the same port that you’re local web server is running on and proxies external requests to your local machine. This was the secret sauce I was looking for to allow RemoteIE to be able to test local sites on my Macbook.

it’s a simple step to get it to listen to your web server. Say you’re running your local web server on port 8080. In terminal, you’d type in: ngrok http 8080. This starts ngrok listening on port 8080 and creates the secure tunnel.

It also creates two sets of publicly available URLs that map to your local web server.

Dropping “http://5057493e.ngrok.io” or “https://5057493e.ngrok.io” (SSL) into your browser’s address bar should now bring up your local site. These are unique URLs that are created each time you restart ngrok making it easy to share these out for one-time testing sessions across a team. The benefit to this, of course, is that you’re now able to use RemoteIE with these public URLs to load and test your local site since to the service, your local site now looks like a staged or production website.


Installation ngrok:
-------------------
   
               $ sudo snap install ngrok

Step#1:
------

Make your app live on localhost:port-num e.g localhost:80

Step#2:
------

Open separate terminal and type :

                    $ ngrok http 80


#terminal-screenshot

ngrok by @inconshreveable                                                                                                     (Ctrl+C to quit)
                                                                                                                                              
Session Status                online                                                                                                          

Session Expires               6 hours, 13 minutes                                                                                             

Version                       2.3.35                                                                                                          

Region                        United States (us)                                                                                              

Web Interface                 http://127.0.0.1:4040                                                                                           

Forwarding                    http://e0b1722b.ngrok.io -> http://localhost:80                                                                 

Forwarding                    https://e0b1722b.ngrok.io -> http://localhost:80                                                                
                                                                                                                                              
Connections                   ttl     opn     rt1     rt5     p50     p90                                                                     
                              21      0       0.00    0.00    65.67   82.86                                                                   
                                                                                                                                              
HTTP Requests                                                                                                                                 
-------------                                                                                                                                 
                                                                                                                                              
GET /                                   200 OK                                                                                                

GET /                                   200 OK                                                                                                
 

Step #3:
-------

Open browser and enter :

                  http://e0b1722b.ngrok.io


                  https://e0b1722b.ngrok.io



Part:B
-------

Freenom is the world's first and only free domain provider.Freenom allows you to use your chosen domain name for a period of 1 to 12 months


Freenom: (Custom Domain)
------------------------

1- Go to https://my.freenom.com/domains.php

2- Check the availability of the domain and check out

3- Press continue and use your google account to register

 
How to setup URL Forwarding in Freenom:
--------------------------------------
Any domain, free or paid, can be forwarded to any URL you'd like, by using Freenom's URL Forwarding Service. 

To set up URL forwarding for your domain:

Go to My Domains: https://my.freenom.com/clientarea.php?action=domains

Click on Manage Domain

Click on Management Tools

Click on URL Forwarding

Enter the destination address in the URL Forwarding box.

Press Set URL

DONE!

There are two different URL forwarding modes that you can select:
With the default mode, frame/cloaking, visitors will see your domain name in the address bar instead of the destination address.
The second mode, redirect/301 forwarding, visitors will simply be redirected to the destination address and leave your domain. 

Sometimes it will be necessary to use the redirect mode of forwarding if your destination URL does not accept or allow framed forwards and shows a white screen instead of the destination web page. 

Please note that it can up to 30 minutes before URL changes are distributed within our databases.



--------------------------------------------------------------------------------------------------------------------------------------------


Helping Material:

url forwarding==> https://my.freenom.com/knowledgebase.php?action=displayarticle&id=5 

servername==> https://www.youtube.com/watch?v=S_e4mA3SnOE 

installation gnork==> https://www.youtube.com/watch?v=S_e4mA3SnOE 
