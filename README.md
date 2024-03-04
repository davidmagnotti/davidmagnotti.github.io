# David Magnotti

The repository is a collection of short and simple HTML5-based games I've made.

I'm a software developer that works in the cyber security field. I was inspired after reading an [Ars Technica](https://arstechnica.com/gaming/2024/01/1d-pac-man-is-the-best-game-ive-played-in-2024-so-far/) article about Kenta Cho's 'Paku Paku' to explore game development. I've never been much of a creative, but I've experienced great joy in exploring this area of technology that intersects with art and engineering.

There's been many amazing software tools and libraries that have helped me in creating these games, including:
 - VS Code (https://code.visualstudio.com/Download)
 - Piskel App for sprite development (https://www.piskelapp.com/).
 - Kenta Cho's crisp-games-lib (https://github.com/abagames/crisp-game-lib)
 - pixi.js (https://pixijs.com/)

## Mobile Ports

I decided to experiment with mobile application development, which led me down a path to porting one of my web app games (Red Light) to Android and iOS:
 - iOS: https://apps.apple.com/us/app/red-light-arcade-edition/id6478185769
 - Android: https://www.amazon.com/Red-Light/dp/B0CVZGDC95

### Background

Back in 2011, I developed a few Android applications, published on the Google Play Store (or 'Android Market' as it was known at the time). I wanted to introduce my son to mobile application development, starting with Android. I was *shocked* at the progression of Android development from 2011 to 2024. Not only has the technology for writing code changed substantially (Android Studio instead of Eclipse, Kotlin over Java) but the testing and deployment process have changed significantly, too. I suppose it's a sign of Android becoming mature. :-)

It seems like there's paradigm shifts in technology every few years that mean you have to constantly be in a state of learning. The .NET framework is a great example of this, migrating UX from WinForms to WPF to various XAML implementations. I've found some of the tech stacks have a high learning curb as well. For us hobbyists, it's discouraging that not only will you spend a significant amount of effort learning something new, but that the technology you learn will only be useful for a few years. With that in mind, I decided to explore if I could simply port web applications directly to mobile platforms, rather than rewrite as I originally thought, and then focus on teaching my son core web development concepts. My research led me to Apache Cordova (or as we called this more experimental technology back in 2011, 'PhoneGap').

I was pleasantly surprised at the maturity of Cordova, and ease of building for Android and iOS. Despite owning an iPhone, I actually don't own a Mac, so I rented one from the VPS provider, [MacInCloud](https://www.macincloud.com/). It took me more time learning how to setup my developer box with the right certificates and getting Xcode deployment figured out than it did to write any of the games I've made. But, with a few hours of troubleshooting, I was able to build and test my applications locally in both Android and iOS. I published to the App Store and after a few minor tweaks to address some feedback from the Apple App Store review team, I was published!

Unfortunately, I did not have a positive experience with Google Play. I learned my primary developer account was suspended due to inactivity. I opened a support case with Google to re-activate the account, but I was informed their policy prohibits re-activation of an account suspended due to inactivity. I created a new account and discovered that Google had a recent policy change that requires any developer account created after November 2023 to have 20 private testers to test the application. I couldn't tell you 20 people I know that own Android phones, let alone ask them to help me test a game port for my game development hobby. I decided to proceed with publishing my Android application in the Amazon Appstore instead.

There's some rumblings spanning back to 2022 about Apache Cordova usage declining ([The Sunset of Apache Cordova: Alternatives For Cross Platform Mobile Development in 2022](https://medium.com/codex/the-sunset-of-apache-cordova-alternatives-for-cross-platform-mobile-development-in-2022-9da34234c992)) which I worry means I'll soon have to find an alternative. As I mentioned, technology changes every few years. It seems that most technology companies gravitate toward using Flutter, React Native, or Xamarin for cross-platform mobile development, as they each tend to provide a 'first-class' app experience (performance, layout, UI elements, etc). I find front-end web development frameworks like React and Angular become unnecessarily complex in larger codebases, so I'm not interested in React Native. I'm uneasy with learning Flutter seeing that it uses its own language I would need to learn (Dart). As an experienced C# developer, I could explore using Xamarin, but I would still need to learn other aspects of Xamarin like the actual UI framework. While not one of the major three contenders favored by larger companies, I found a fourth contender in Ionic Capacitor. Capacitor provides a similar Apache Cordova experience for porting HTML5 applications, and was actually based on the same stack at one point. I'll probably end up migrating from Apache Cordova to Ionic Capacitor in future ports.
