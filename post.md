OBS is open Broadcaster Software. It's latest version, OBS-Studio, is in now in version 19.0.3. Installer downloads are available for Mac and Windows, and repositories are available for a variety of Linux flavors.

## What is OBS-Studio

At it's most basic, OBS-Studio is software for recording the desktop. It can be used to make instructional videos or other screencasts. This has been possible in Linux for years using arcane ffmpeg scripts but OBS wraps that in a slick GUI.

Going further, OBS allows the user to record each window of the desktop environment separately. The user can then combine these windows into scenes. A scene can be constructed out of sources: application windows, static images, webcam feeds, and more. Each source can be positioned and layered to give the scene a polished look and feel.  

![Screen Shot of OBS](obs-view-1.png)

Figure 1: A basic scene with four sources, a blue background (bottom layer), a text source for the title, a terminal window being captured, and a webcam source of the author. Note the red control points around the terminal source. Sources can be moved, resized, and layered on top of each other.

This is a very basic scene construction. The tool can be used (especially when combined with other graphics software) to make beautiful and seamless scenes. The scenes can be switched from one to the other at the push of a button.

![Short video/gif clip of using obs to switch scenes](obs-example.gif)

Figure 2: Gif of some basic scene switching. Quality losses are due to the giffing process.

One neat thing about OBS is that desktop recording is no longer tied to the state of the desktop. The windows can be arranged by the user in any way they desire, and OBS will only record the ones it is configured to record and will arrange them according to the scene layout.

OBS can create three kinds of output. It can record video files in a variety of formats. It can stream the video output to a livestreaming service like twitch.tv or facebook live. Or it can push output to a dedicated monitor or projector. All three of these outputs are very useful.

Recording to disk is useful for creating high quality videos. Recordings can be edited later in video editing software and then uploaded to a video hosting service like YouTube or Vimeo.

Streaming to a livestreaming service is probably the most common use case for OBS. A huge percentage of twitch's streaming population uses OBS to stream. OBS (and twitch) use the RTMP protocol to stream video. This is why it is possible to use a completely open toolkit to broadcast on twitch. Because OBS is open source, support for new services is being added all the time.

Displaying the output directly on a monitor(Preview mode) is a less used but very powerful output method of OBS. Scene switching, graphical overlays, smooth transitions and more are all available as hotkeys to whoever is in control of the OBS application. There are many cases where an audience is watching a projector or TV screen and the production could benefit from the professional touch that OBS enables. Examples are an in-person esports tournament or a conference keynote.

## Who uses OBS

Streaming to twitch.tv is extremely popular. Watching these streams is also popular. At any given time, close to a million people are watching live, while thousands are streaming. Mostly, they stream video games. These games aren't just on the computer. Capture cards and capture devices from vendors like Elgato let streamers capture and stream from virtually any device, from the original Nintendo to the Playstation 4 to handhelds. OBS is such a powerful player in the scene that Elgato and other vendors create [excellent doucmentation](https://gaming.help.elgato.com/customer/en/portal/articles/2768069--elgato-stream-deck-%E2%80%93-obs-integration-) on how to integrate their products with OBS.

Chantal "Sylvanas" Frey is a streamer from Germany. She streams to twitch.tv four to five times a week, usually playing the game Overwatch. Asked how many hours she has used OBS for, she can't quantify the number:  "been streaming for 2.5 years now, sooo many hours haha."


![Sylvanas Stream Capture](sylvanas_sc2_cap.png)

Figure 3: Chantal "Sylvanas" Frey playing Overwatch. She adds a webcam feed and some sponsor logos to her stream using OBS.


## Where does OBS come from

OBS is developed by a small team working in the open. Most of the code has been written by jp9000/Jim. Several other people have made serious contributions to the project. The project has two very active IRC channels: '#obsproject' for user chat and support, and '#obs-dev' for developer chatter. Both of these IRC channels are on Quakenet, instead of the more common Freenode network. This illustrates how OBS forms it's identity as a piece of gaming software first and a piece of Free/Open Source software second. OBS has a very active forums on the main website. The forums is where users post plugins that they have created.

![Community chat guidelines](ob-community-chat-agreement.png)

Figure 3: Users who click 'use chat' on the OBS website must agree to be polite before they are joined to quakenet over a web bridge.

## Advanced features

One excellent plugin exposes a websockets server that can be used to control OBS through a webpage. Several clients have been made, and it is common for a streamer to use a second laptop or tablet to control OBS.

OBS is ready for real-time. OBS can render web resources directly onto the stream (called a "browser source") or read files from disk. This enables streamers to overlay recent tweets, channel chat, currently playing music, scores in games, the weather, and other notifications. Most advanced animations are implemented via browser sources.

Caroline "omgVandi" Vani is a freelance graphic designer and streamer on Twitch. As part of her graphic design business she designs graphics and overlays for streamers. Streamers use OBS combined with staic grahpics and animated browser sources to create good looking streams.

OmgVandi says that most OBS scenes are constructed out of a few baics sources. 

* Webcam video source: "A lot of people will have a greenscreen. Some people have the straight camera box, but if they do, they have a real life background that fits the style of the stream. The background of the camera becomes a relevant part of the stream." 
* Game capture
* A browser source that displays new followers, new donations, and subscriptions.
* Static or animated graphics to provide borders and branding: "My job as a graphic designer is to ... create the visuals that go into browser sources, or to create a static PNG overlay that goes on top". "Static PNG overlays are pretty standard for people that don't have a ton of money to spend on custom designs. They look really good, they're clean, most of them can be nice and simple."

![OmgVandi Stream Capture](omgvandi_screenshot.png)

Figure 5: Stream screenshot from omgvandi. Note the box around her webcam and twitter and instagram tags. The border and social boxes(overlay assests) are created in graphics editing sotfware separately. Then OBS is used to layer the game, then the webcam source, then the overlay assets. Most webcams do not shoot in the widescreen format omgVandi is using, OBS can be used to crop the live video feed to a better looking aspect ratio.

![Brotatoe Stream Capture](brotato_screenshot.png)

Figure 6: Stream screenshot from brotatoe. Advanced streamers usually have several OBS scenes. This is a screnshot from the 'Out of game' or 'Webcam focus' scene from popular streamer Brotato. The effort and quality put into the border graphics is plain to see. At the bottom of the scene, the graphics create (with the brown background) windows for dynamic content to be displayed. Brotato is using dynamic web content to display the names and values of his most rescent supporters: 200 bits is a one time donation and 25 months is the length of subscription to montly donations. The cup in the upper right is an animated browser source and visualizes for the viewers how many donations the streamer has gotten that day, a virtual tip cup.

## What is different about OBS

OBS has a huge and engaged user base. It might be the highest for a project of it's size in FLOSS. This is a project with one main developer, a few other volunteers, and no one getting paid for their work. The windows version of 19.0.2 has been downloaded from github 2.3 million times in 26 days since it's release. The 19.0.3 version has been downloaded 133 thousand times in less than two days. The official twitter account has 90,000 followers.

When DD-WRT first came out, one of the lines was 'turn you $50 router into a $5000 router.' The explanation was that with this piece of software you could get features that were only available in professional, expensive devices. This is essentially what OBS is doing. OBS gives the streamer tons of control over the broadcast. Control that until now hasn't been seen outside a professional TV network or sports broadcast.

OBS is exciting for three reasons. 

One: Technically, it is really cool. What it can do and what the user can do with it is flat out impressive.

Two: In this age of corporations throwing dozens of developers at OpenStack, Docker and kubernetes; startups with open core products; and declining support for core FLOSS software, it is encouraging to see a small, self-sustaining, and successful project - let alone a desktop app project.

Three: OBS is, as the gamers would put it, hype. 90k twitter followers, companies putting 'Works with OBS' in their product marketing, antivirus companies working with OBS on whitelisting, etc. This project has a large excited userbase, most of whom aren't selecting it based on license.  Just look at some of these tweets. We asked Sylvanas "Did you know OBS is Open Source? What does that mean to you?" Her response: "never thought about it."

https://twitter.com/laserring/status/873037202862645256

https://twitter.com/OGBUSTA/status/866085482945490945

https://twitter.com/kayosgirl86/status/859529074984792065

https://twitter.com/Omega6ixx/status/843966705185443840

https://twitter.com/FragManSaul/status/836489151679709185

https://twitter.com/nathaniastv/status/865264972456108033


omgvandi stream - Twitch.tv/omgvandi
omgvandi stream - Twitch.tv/brotatoe
sylvanas stream - Twitch.tv/sylvanas_sc2
Overwatch is a registered trademark of Blizzard Entertainment

If you'd like to contract omgVandi to create some graphics for your stream, you can DM her over Twitter at @omgvandi, or send an email at cvani@rogers.com.

