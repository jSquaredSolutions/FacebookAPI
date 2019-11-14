so I was able to get the first iteration of the Facebook API working  however I was only able get it working outside of the EPA network because inside the EPA network I get an "X frame options denied message". I don't think it's the network. I think it's something to do with the Chrome browser settings on the EPA laptop. I tried it on my EPA laptop while off the EPA network and instead on my T-Mobile network. I still got the x-frame error even though I was not on EPA network.  The other kind of tricky thing is that the scripts for the Facebook API need to be in the body tag according to Facebook documentation. 

To test this start the node server "node demo.js", after the page has loaded run:

 FB.getLoginStatus(function (response) {
                    statusChangeCallback(response);
                });

In the console window

once I added the EPA app ID I was then asked to log in (see this screen shot capture.gif)

It also says: This doesn't let the app post to Facebook

