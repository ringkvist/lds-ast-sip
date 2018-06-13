# lds-ast-sip
Creating a webbased softphone, connected to Asterisk, GUI implemented in the Lightning Design System

The ambition is to create a browserbased SIP phone on top of an Asterisk based PBX. The phone GUI is to be implemented in the Lightning Design System (http://www.lightningdesignsystem.com/components/docked-composer/). Try to choose some of the 'Voice' examples in the right side of the screen - from the link above. 

The list of frameworks might not yet be complete - but the following frameworks might come in handy:
 - http://www.doubango.org/sipml5/                (https://wiki.asterisk.org/wiki/display/AST/WebRTC+tutorial+using+SIPML5)
 - http://jssip.net/
 - https://sipjs.com/
 - https://collecttix.github.io/ctxSip/

I see the project in the following steps:

Step 1 - Create PBX test environment
Install Ubuntu based Asterisk server
    - base install (MIR)
        - make sure to make detailed install steps (MIR) 
    - setup two local extensions (MIR)
    - make test calls using a soft phone (MIR)
    
Step 2 - Setup web environment for application test
    - NGINX
    - choose... framework
    - Test 
    - Decide
    - choose... framework
    - Decide 
    ....
    CHOOSE
    
Step 3 - Install web server environment
    - NGINX based webserver
    - React, Node.js... (Help me here Sean :-) )
    - "Insert" chosen framework into the framework
    - Test

Step 4 - Now things get real exciting :-) 