---
title: "Monkey King and the Battle for Web Dominance"
date: "2021-08-01"
categories: 
  - "software"
tags: 
  - "delphi"
  - "electron"
  - "firemonkey"
  - "vs-code"
---

Li Huai, the grandson of Xiao Li Fei Dao Li Xunhuan, is a top-notch expert. However, one night, he gazed foolishly as a flying knife plunged into his left chest, resembling a beautiful moonlight. - "Flying Daggers, Seeing Daggers Again."

In our previous discussion on HarmonyOS, we spent a considerable amount of time discussing Ark Compiler. So is this approach actually the right one? As those with academic experience know, being the first to come up with an idea is very difficult. Let's take a look at any similar attempts in the industry.

There is a thing called FireMonkey that has implemented a concept similar to Ark, and it supports Win/Mac/iOS/Android altogether. This can be translated as the "Monkey King" thing, which is now part of Delphi.

Looking at Windows 11, Microsoft not only supports traditional Win32, .NET programs, but also supports web-based PWA and Android apps. Turning to the latest release of Windows 365, the entire operating system can function as a SaaS solution within a web browser.

The boundaries of various platforms are beginning to blur, and the divide in hardware architecture is gradually being bridged by various compilers and translators.

As is customary, this article will digress a bit and continue on with the stories of the other gods in addition to Anders Hejlsberg in "The Gods of Programmers" (link). The prerequisite for continuing to read is to know who Anders is - the god who never misses with his code throwing knife. We will talk about "Monkey King" later in the article.

### One: Rise and Fall of Delphi

Many people say that Anders' departure was the reason for Borland's decline, but this is definitely an exaggeration. Anders did not play a major role in the development of the heavyweight Delphi 3. He left for Microsoft in 1996, just one year after Delphi was released. Delphi was led by his most important comrade Chuck Jazdzewski until 2004, so Chuck should be considered the main contributor.

For the seven or eight years after 1995, Delphi has continuously put pressure on Microsoft's Visual Studio. During that time, Zhang Xiaolong gained fame by developing Foxmail using Delphi. Later, he utilized web technology to create email, WeChat, as well as mini-programs and various other applications. We won't delve into that for now. As a little piece of gossip, it is said that "Fox" is a tribute to Linghu Chong.

New versions of Microsoft Windows always deal a heavy blow to Borland. Just as OLE caused the downfall of Borland C++, .NET makes it difficult for Delphi to keep up, since Borland simply does not have the resources to undertake complex upgrades.

Especially at that time, the importance of Java had already surpassed that of Windows native program development, and Delphi had gradually fallen out of favor within Borland.

### 2\. Blake, Chuck, and Danny (BCD)

At the end of the last century, Borland focused its efforts on JBuilder, with Java genius Blake Stone serving as CTO. It was said that this caused Chuck to leave the company to join Microsoft. Danny Thorpe took over as Chief Architect for Delphi.

Danny himself is an inspirational story. When he joined Borland, he was just an assistant tester and had been doing testing for 5 years. But fortunately, he was testing for Anders and Chuck.

This tells us that the position is not important, but who we are with is more important.

Danny, who enjoys making his own porcelain bowls, said he only started looking at the compiler during his time with Delphi 5. It was rumored that nobody dared to touch Anders' code at that time. Meanwhile, Chuck's early main work focused on VCL components, which were the killer feature that shook the world of Delphi and also inspired later development tools such as Java and C#.

### 3\. From JBuilder to VS Code.

Thanks to Blake Stone's courage, JBuilder is essentially a Java re-write of Delphi, making Java programs more pure and compatible. In the case of Microsoft Visual J++ being out of the game early, Borland JBuilder lived up to expectations and defeated almost all competitors, including IBM VisualAge for Java.

In 2001, IBM failed and transferred VisualAge for Java to the open-source project Eclipse. An exceptional software engineering expert, Erich Gamma from Switzerland, joined the Eclipse team, and later they turned the tables and overcame JBuilder.

The clever Microsoft poached Blake Stone, and the dispassionate Borland later sold off their IDE product line.

IntelliJ, based in the Czech Republic, took the opportunity to succeed in the commercial IDE market by focusing on continuously improving products such as IDEA. IntelliJ, now called JetBrains, was created by three Russian programmers during the dot-com bubble. Impressive is the fact that these founders have consistently rejected external investment and going public, avoiding the fate of Borland.

Microsoft, with its wealth and power, once again poached Erich Gamma from IBM (have they collected all five Dragon Balls?). They promised Erich that he could continue working in Switzerland and build his own team. Erich has once again achieved a self-transformation, creating another masterpiece, VS Code, using web technology (Electron) as its foundation.

We previously mentioned how Bezos allowed Chris Pinkham to develop AWS EC2 in South Africa, Anders worked for Philippe Kahn from Denmark, and Zhang Xiaolong kept his distance from Pony Ma. These stories tell us that if you are truly talented, you can bravely ask your boss to let you work in Lijiang during the summer and Sanya during the winter.

### 4\. Web Reunion

The design concept of VS Code is completely different from Visual Studio, with a focus on Web technology as its core. We can also see Web technology becoming an arena for top-notch developers to collide once again.

Chuck and Danny had collaborated on the Windows Live team after joining Microsoft, but the company's social products were not successful, and the two later left.

Chuck is currently working at Google. Prior to transitioning to the Android frontend to work on Jetpack Compose, he was involved in working with Anders in developing Angular 2 with TypeScript.

Angular, in turn, has also promoted the development of TypeScript.

Angular's competitors include React from the Facebook camp and Vue, which is now dominated by the Chinese camp. Along with VS Code, the great minds of programmers are coming together again.

The creator of Vue, Evan You, also comes from Google. He is a shining example that demonstrates China's strength in producing coding legends among the new generation who are well-provided for, just like in Europe.

The four great talents of Borland, ABCD, were all poached by Microsoft, and eventually Delphi was also sold off.

Danny once answered on Quora why Borland failed: He believed that Borland's management wanted to shift from million-level programmer clients to fewer numbers of high-income enterprise clients, which was a wrong direction. However, Borland's legendary founder Philippe Kahn, who was kicked out by the board of directors, gave a thumbs up and believed that Borland should focus on desktop applications for billions of users.

Kahn is from a Jewish family who fled to France. When he came to America to seek his fortune, he had no green card or job and was essentially an undocumented immigrant. He started his own company and employed himself. While studying at ETH in Switzerland, Kahn had a teacher named Niklaus Wirth who invented the Pascal programming language. This led him to recognize the value of Anders' Pascal compiler.

Kahn was an entrepreneur who pioneered the strategy of using high-quality software priced very affordably, and most of Borland's products quickly captured market share. Before the birth of Delphi, Borland had engaged in battles on multiple fronts with industry giants.

Borland's dBase database directly challenged Microsoft's Access and ForPro. Borland's legal battle with Quattro Pro and Lotus 1-2-3 went all the way to the federal Supreme Court and resulted in a rare 4:4 deadlock, with Microsoft's Excel ultimately benefiting from the situation.

As a generation of heroes who once dueled with Bill Gates, Kahn remained devoted to reaching end users through applications and drifted away from the web gradually, ultimately falling into mediocrity.

### 6\. Monkey King and Xamarin

After selling development tools such as Delphi to Embarcadero, Borland's new owner actually achieved annual updates for the following thirteen years.

Ten years ago, FireMonkey (Monkey King) appeared in Delphi XE2, which implemented cross-platform native code. It means that with one set of Pascal code, you can compile and run it on Apple, Android, and even Windows platforms. However, each app needs to embed a set of FireMonkey runtime.

Just like Ark, FireMonkey has proven that static compilation is technically feasible. However, whether FireMonkey can flexibly handle different screen sizes and various compatibility issues, and whether static compilation is meaningful, is still controversial. Ark, on the other hand, has an advantage that FireMonkey cannot have, which is that it can embed runtime into HarmonyOS in advance, so the startup speed of the app can be much faster.

Microsoft has a tool called Xamarin, which is similar to FireMonkey, in order to make .NET compatible with Android, iOS, and Linux. With Xamarin, Java knowledge is not required and Android apps can be developed with only knowledge of C#. The difference between Xamarin and FireMonkey or Ark is that it resembles an instant language translator.

Xamarin was created by Nat Friedman and a Mexican brother Miguel de Icaza, formerly known as Mono. These two gentlemen are not ordinary people, as Nat Friedman is currently the CEO of GitHub; while Miguel is one of the founding members of the well-known GNOME, and in 2014, when Anders announced the open source of .NET Core, Miguel stood at his side and was appointed as the first director of the .NET Foundation.

Last year during the 25th anniversary celebration of Delphi, several of the original creators and present leaders of Delphi had a virtual gathering. Chuck (on the left) and Anders (on the right) and other elderly developers over 50 years old who are still writing code happily reminisced about the passionate and exhilarating years.

### Seven, Fusion

"The situation in the world is that things that are united for a long time must eventually split, and things that are split for a long time must eventually come together. After various languages and platforms have blossomed, the Web technology has gradually become a gathering place for many gods, and it has also brought us more specialized fields: PWA, AMP, SPA, WebAssembly..."

Especially WebAssembly, due to its significant improvement in implementation speed, is gradually penetrating into fields previously considered impossible, making it possible for the browser to become the center of everything.

The use of web technology in mobile apps has been a topic of debate among many people. Web technology is inherently open, but native apps have better performance and are more important, as they can be very rogue and make it easier to control permissions and traffic.

At present, neither native nor web apps possess the ability to overpower the other. Many web apps are equipped with a native shell, integrating and deceiving one another.

### 8\. Conclusion.

In this article, we mentioned Danish, Swiss, French, South African, Mexican, Russian, and of course Chinese people. For friends who have no interest in the history of software, I imagine these names have been a painful experience.

The life of a programmer is a bit like a polytheistic religion: endless scriptures to study, countless gods to worship.

Li Huai in Delphi was struck by a flying knife, and although he survived, no one in the martial arts world speaks his name again.
