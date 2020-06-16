# WWDC20-Wotagei-x-Music-Game

## About

A visual simulator for Japanese glowstick dancing ("Wotagei"), plus a partial "rhythm game" built on top of it, and a very minimalistic/incomplete chart editor for the "rhythm game".

## Update June 16, 2020

idk how the fuck they accepted this highly incomplete submission but they did

## Original Comment

WWDC20 Swift Student Challenge Submission - Swift PlaygroundBook "Wotagei x Music Game"

This project is very rushed but I tried.

I didn't do ARKit again because both of my previous two ARKit submissions were rejected.

The header comments were not converted into Markup because Markup & iCloud syncing bugs made me lose all my previous Markup comments near the last moment; I restored everything I could but did not have enough time to test Markup again (and risk losing all those comments again) so I just kept them in the normal comments form. (I wrote about this in the "Comments" section of the written essay responses too)

The core functionalities of this playground is completed and largely without problems (unlike the two previous years). However, I did not have enough time to make important features such as sound ("music"), score-keeping systems, more content, etc.

Overall I think my chances of winning are very slight. I'll be expecting yet another "Your WWDC Scholarship Status Update" (or "Your WWDC Swift Student Challenge Status Update") email lol.

## Written Responses

### "Tell us about the features and technologies you used in your Swift playground."

The simulator/game itself is done entirely in SpriteKit. The visual effects utilize SpriteKit’s particle system and lighting system (for the glowsticks), action system (especially custom actions, for the chart nodes), and shader system (I had to look up how to use GLSL, to write a gradient for the curve that connects visible nodes on the chart).

The creation of some of the effects were math-intensive as in requiring a lot of mathematical problem solving, but the level of mathematics don’t really go beyond trigonometry and vectors since higher level concepts weren’t necessary for my implementations. 

A mathematical accomplishment I’m very proud of is the moving legs effect in the background of the game, where the angle between the upper leg and lower leg is calculated using trig and **worked perfectly on first try**.

The chart editor also uses SwiftUI for user interaction and displaying data (beats, location, etc.). I’m a SwiftUI beginner and SwiftUI seemed hard at first, but once I got used to it I found it really efficient and concise.

I also incorporated good programming habits (especially ones for Swift) that I learned over the years. I try to isolate as many features as possible and put them into separate modules so that they can be better tested and organized. I also used generics and closures extensively to adhere to the protocol-oriented programming philosophy that Swift programmers treasure. 

### "Beyond WWDC20 (optional): If you've shared or considered sharing your coding knowledge and enthusiasm for computer science with others, let us know. (500 words or less)"

Currently I’m a freshman in a very STEM-intensive college and we were all busy transitioning and keeping up with classes so I didn’t accomplish much extra-curricular things over the past year. It was only during the coronavirus lockdown did I finally have time working on things like an awesome new update to my keyboard app packed with features, community-suggested improvements, and bug-fixes. I’m looking forward to turning more of my (long list of) app ideas and game ideas into reality during the rest of the school year and summer; unfortunately none of those ideas made it to my Swift Student Challenge because of the short time window and the fact that a lot of them just aren’t suitable for the playground format. My friends and I also have plans on reaching out to other Apple-platform developers on campus to build a community next school year after (hopefully) the pandemic ends.

Despite the all-in on transition and computer science courses this year, I do have a long history of sharing cool home-made programs and building programmer communities in our school when I was younger. 

Ever since middle school I have loved sharing my programming projects with other kids around me, especially the Swift projects I made after the language came out in June 2014. 

One peculiar incident was in eighth grade, when we were required to do class-wide activities consisting of minute-long challenges every Wednesday morning. Students take turns designing the challenges, usually requiring the student to bring snacks and items as materials. The night before my turn, I realized that I had forgotten to purchase any materials, so I rush-coded a simple 3-lane flight-and-dodging game (https://github.com/Vince14Genius/App-Flight) in four hours. It was a huge success. Words spread and from then on, the grade knew me as the “programming guy”.

I also helped create Codelympians, the first major programming club in our high school along with 4 friends, and served as a high-contribution board member until we graduated. The club is still alive today. It had a peak membership of around 30 students, average membership of more than 20 students, and was in a growing trend during the years we managed the club. I was responsible for advanced-level teaching, initiating many project ideas, all the graphics design, and participated a lot in major discussions about the development of the club. 

I hope to replicate that success in college, and expand upon it. 

### "Apps on the App Store (optional): If you have one or more apps on the App Store created entirely by you as an individual, tell us about them. (500 words or less)"

My first and by far only app on the App Store is “IPA Phonetic Keyboard” (https://itunes.apple.com/us/app/ipa-phonetic-keyboard/id1440241497). It is a keyboard for typing IPA (International Phonetic Alphabet) symbols, designed to be convenient and delightful to use for linguistic hobbyists and language learners. 

My keyboard is now the top result in the App Store that comes up when people search for “IPA keyboard”. It now has over 20,000 downloads, has a global average rating of 4.6 stars, and is well-received (“At the moment, IPA Phonetic Keyboard is the only iOS option I’m aware of that meets my criteria for a good IPA keyboard app, so it’s now my top pick.” https://allthingslinguistic.com/post/108388734856/how-to-type-the-international-phonetic-alphabet-on) in many online linguistics communities (of different languages; the ones I know of are in English, Chinese, Japanese, and Esperanto). All these facts make me confident enough to say that I have completely conquered the niche market of IPA keyboards for iOS.

Successes aside, there is also a lot of story behind this simple keyboard app. 

Linguistics (the study of how languages work) is one of my top passions, in addition to programming, design, and Otaku culture. A key component of languages is vocal speech, so the IPA - a standard set of symbols that can accurately describe pronunciations in any language - is very important in linguistics discussions. However, there were no good keyboards for IPA input on the iPhone: they either aren't free, are poorly-designed, or have an incomplete IPA set. My friends in online linguistics chat groups complained, occasionally and passively, but did not expect nor seek any change to the situation. 

I set out to right this wrong. What comes first is the design, and designing a keyboard is mostly about the layout. There are two tasks at hand: I must fit the entire IPA table into this keyboard with all the IPA symbols organized by either place or method of articulation, and I must make each key large enough to be tapped. Ultimately, I decided to imitate the system emoji keyboard, but add linguistic twists to the organization of the keys so that every linguist can intuitively find the key they’re looking for

This design sets my keyboard apart from traditional QWERTY-styled IPA keyboards (which are actually very unintuitive) and keyboards that just slap in an IPA chart (which looks ugly and makes everything hard to tap on). Within mere weeks after the release of my keyboard, those online chat groups are already becoming filled with phonological discussions and happy linguists.

### "Comments (optional): Is there anything else you would like us to know? (500 words or less)"

N/A
