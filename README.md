# ESSA
This is speaking game demo for kids that are learning English

# Intro about step
Dear sir.

Let me introduce about this project.

Word War game was developed to improve kid's English pronunciation.
At first , I divided this project as four main parts like milestone so first part is speech recognition and I could get speech recognition sample project from Google so that I added Unity Speech Engine to project. It worked well on Unity Editor and PC so I built it for mobile but critical error was detected on mobile phone. Speech recognition function didn't work on mobile so I was trying to find the correct solution. 2 days later from at that time , I found solution about it. I was using unityengine.windows.speech in C# script but it was not available for mobile. I started to find the correct speech recognition engine for mobile and 3 days later , I became to see one thing on Github. I got it instantly and applied it to project so it works well on mobile but anybody knew what error can be detected on test. I tested speech recognition system on several mobile phones with variety types and I confirmed speech recognition availability on mobile. So I sent demo project to my client and was waiting his feedback about speech recognition. 1day later, client sent me screen shot about demo project and I found another critical error about it.
Speech recognition didn't work on client's mobile phone. So I tested it on my mobile phone and on my friends' phone. It worked well there but didn't work on client continuously. So I started to find the way to solve this problem and worked for it around the clock. A week later , finally  I found the answer.
I tested speech recognition on variety mobile phone types but they are Android5.0 ~ Android 9.0.  But my client was using OPPO with Android10.
Android10 or more higher level has protection about access phone device so speech recognition couldn't access to microphone on Android10+. And I added some text on manifest.xml so finally speech recognition could work on Android10+.So that  I finished first part of game project and continued project. Second part is for single player about whole game project.
Before start second part , client asked me some questions following below.
"How can you identify user?", "How can you save user data?" , "How can player continue game on other device?"
I answered for first question like this. "I'm going to use device unique identify number called IMEI and we can know who is player".
And I answered for second question like this . "I'm going to save user data into Database and player can get his data whenever user play game".
At the end I answered for third question like this. "Player can register or log in to play game for the first time. So if user type his previous data on log in form ,user can continue game on other device. And to avoid multiple log in , user only can register on game at first time".
Client listened to me carefully and he was in total agreement with my suggestion.
So I started development for second part but there is simple problem on design.
At first , client provided me UI design as draft but it was classic.  I didn't mind that UI so I suggested to client about updating UI and client approved my idea so that I changed it with my idea . 
Second part was easy for me so I have done it for 5 days.
And third part is about multiplayer. I had to choose multiplayer engine and I choosed Photon for Unity Online Multiplayer.
Photon is very light and easy SDK so anybody can make unity multiplayer game using it.
So I started develop multiplayer using Photon.  But there were so many errors and bugs on it.
First error was very strange. I was using self-hosted server SDK for LAN but if I build into app , app doesn't work.
Exactly , on multiplayer , app can't create room and shown error like this "refused from server" and "removed from master server".
I was trying to find solution for 15 days and finally , I found it.
It's about port so photon was using ports 5055 , 5056 , 5058 but on my side , those ports were not available.
So I developed on other PC and app works well on multiplayer.
And next problem is about using photon chat. So Photon could connect to Photon Cloud on my side but couldn't connnect to Photon Chat.
I lost 5 days to find this solution and 7 days later finally I found it so self-host SDK server didn't support Photon chat and only Photon Cloud supported it. So I used Photon Cloud from at that time.
And I have done IAP on this game project.
Client wanted IAP for apple store so at first I made IAP demo using test IAP link and after that , I type app ID on Apple Store and complete it on time.
Finally I reached last part of game project and I had to complete game and find bugs and fix it.
So totally on 4 months I have done almost and I have made prototype almost 95% more.


