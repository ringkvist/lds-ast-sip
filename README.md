# lds-ast-sip
Creating a webbased softphone, connected to Asterisk, GUI implemented in the Lightning Design System

The ambition is to create a browserbased SIP phone. The phone GUI is to be implemented in the Lightning Design System (http://www.lightningdesignsystem.com/components/docked-composer/). Try to choose some of the 'Voice' examples in the screen from the link above. 

The work has not yet been completed but the following frameworks might come in handy:
 - http://www.doubango.org/sipml5/                (https://wiki.asterisk.org/wiki/display/AST/WebRTC+tutorial+using+SIPML5)
 - http://jssip.net/
 - https://sipjs.com/
 - https://collecttix.github.io/ctxSip/

I see the project in the following steps:

Step 1 - Create test environment
Install Ubuntu based Asterisk server
    - base install
        - make sure to make detailed install steps
    - setup two local extensions
    - make test calls using a soft phone
    
Step 2 - Setup web environment for application test
    - NGINX
    - choose... framework