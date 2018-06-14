# lds-ast-sip
Creating a webbased softphone, connected to Asterisk, GUI implemented in the Lightning Design System

The ambition is to create a browserbased SIP phone on top of an Asterisk based PBX. The phone GUI is to be implemented in the Lightning Design System (http://www.lightningdesignsystem.com/components/docked-composer/). Try to choose some of the 'Voice' examples in the right side of the screen - from the link above. 

The list of frameworks might not yet be complete - but the following frameworks might come in handy:
 - http://www.doubango.org/sipml5/                (https://wiki.asterisk.org/wiki/display/AST/WebRTC+tutorial+using+SIPML5)
 - http://jssip.net/
 - https://sipjs.com/
 - https://collecttix.github.io/ctxSip/

I see the project in the following steps:

Step 1 - Create PBX test environment (DONE)
Install Ubuntu based Asterisk server

    a. base install
	  I installed an Ubuntu 16.04 as a virtual machine using vmware
	  
    b. setting up Asterisk 
	  The setup was done by the help from Mike42: https://mike42.me/blog/2015-01-02-how-to-set-up-asterisk-in-10-minutes The only issue I encountered was and apparently old issue with res_pjsip.so, therefore I inserted the following in the '/etc/asterisk/modules.conf' file:
	  
	  [modules]
	  autoload=yes
	  noload => res_pjsip.so
	  
    c. setup two local extensions 
	  I had two spare Cisco SPA504G phones laying around - which I used for extension 6001 and 6002. A softphone could obviously be used instead.
	  
    d. make test calls using 
	  It worked like a charm :-)
    
Step 2 - Setup test environment for application/framework test
    - NGINX
    - choose... framework
    - Test 
    - Decide
    - choose... framework
    - Decide 
    ....
    CHOOSE (a node.js based framework would be preferred)
    
Step 3 - Test and extend the chosen framework
    - Make sure there is APIs for all situations (transfer calls, in/out of queue... etc.)
	- The result must be a complete API for all the needed functions - which will be used for the development of the GUI.

Step 4 - Now things get real exciting :-) 
	- Develop the GUI in the LDS.