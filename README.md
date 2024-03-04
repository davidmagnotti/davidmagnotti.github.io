# David Magnotti

The repository is a collection of short and simple HTML5-based games I've written.

I'm a software developer that works in the cyber security field as a profession. I was inspired after reading an [Ars Technica](https://arstechnica.com/gaming/2024/01/1d-pac-man-is-the-best-game-ive-played-in-2024-so-far/) article about Kenta Cho's 'Paku Paku' to explore game development. I've never been much of a creative, but I've experienced great joy in exploring this area of technology that intersects art and engineering.

There's been many amazing software tools and libraries that have aided in various aspects of these games, including:
 - VS Code (https://code.visualstudio.com/Download)
 - Piskel App for sprite development (https://www.piskelapp.com/).
 - Kenta Cho's crisp-games-lib (https://github.com/abagames/crisp-game-lib)
 - pixi.js (https://pixijs.com/)

## Mobile Ports

I decided to experiment with mobile application development, which led me down a path to porting one of my web app games (Red Light) to Android and iOS:
 - iOS: https://apps.apple.com/us/app/red-light-arcade-edition/id6478185769
 - Android: https://www.amazon.com/Red-Light/dp/B0CVZGDC95

### Background

Back in 2011, I developed a few Android applications, published on the Google Play Store (or 'Android Market' as it was known at the time). I am shocked at the progression of mobile development from 2011 to 2024. Not only has the technology changed substantially (Android Studio instead of Eclipse, Kotlin over Java, among other changes) but the testing and deployment process has changed. I suppose it's a sign of platform maturity. :-)

It seems like there's paradigm shifts in technology every few years that mean you have to constantly be in a state of learning (I think to the .NET framework migrating UX from WinForms to WPF to various XAML implementations). I've found some of the tech stacks have a high learning curb as well. It's discouraging that not only will you spend a significant amount of effort learning something new, but that the skill you learn will only be useful for a few years. With that in mind, I decided to explore if I could simply port web applications directly to mobile platforms, rather than rewrite as I originally thought. My research led me to Apache Cordova (or as we called this more experimental technology back in 2011, 'PhoneGap').

I was pleasantly surprised at the maturity of Cordova, and ease of building for Android and iOS. I actually don't own a Mac, so I rented one from the VPS provider, [MacInCloud](https://www.macincloud.com/). It took me more time learning how to setup my developer box with the right certificates and getting Xcode deployment figured out than it did to write any of the mini-games I've written. But, with a few hours of troubleshooting, I was able to build and test my applications locally in both Android and iOS. I published to the App Store and after a few minor tweaks to address some feedback from the Apple App Store review team, I was published!

Unfortunately, I did not have a positive experience with Google Play. I learned my primary developer account was suspended due to inactivity. I opened a support case with Google to re-activate the account, but I was informed their policy prohibits re-activation of an account suspended due to inactivity. I created a new account and learned that Google had a recent policy change that requires any developer account created after November 2023 to have 20 private testers to test the application. I couldn't tell you 20 people I know that own Android phones, let alone ask them to help me test a game port for my game development hobby. I decided to proceed with publishing my Android application in the Amazon Appstore instead.
