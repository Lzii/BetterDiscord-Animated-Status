# BetterDiscord-Animated-Status
Open Discord, go to Settings>Plugins, enable AnimatedStatus and click on Settings.

Enter the required information into the input fields and click save

The value specifies the length of each animation step in milliseconds. Example: With a timeout of 2000, the following animation would take 4 seconds to complete
To prevent the discord server from being spammed with requests, the minimum allowed timeout is hardcoded to be 2.9 seconds.

Logically, the animation timeout should be at least 2900, at best 10000 milliseconds (10 seconds) for the animation to look smooth on other clients.

*Animations are made in a really simple and easy to understand syntax.

"Test (Message)"
"Test (Message)", "👍 (Symbol)"
"Test (Message)", "emoji (Nitro Symbol)", "000000000000000000 (Nitro Symbol ID)"
"eval new String('test') (Javascript)"
"eval new String('test') (Javascript)", "eval new String('👍') (Javascript)"
...

*Custom Javascript

Have the current time as your status:

![image](https://user-images.githubusercontent.com/81039439/118372461-aa86e600-b5a9-11eb-8ad4-2062cee8f22b.png)


"eval let fmt=t=>(t&lt;10?'0':'')+t;let d=new Date();`${fmt(d.getHours())}:${fmt(d.getMinutes())}:${fmt(d.getSeconds())}`;", "eval ['🕛','🕐','🕑','🕒','🕓','🕔','🕕','🕖','🕗','🕘','🕙','🕚'][((new Date()).getHours()%12)];"
