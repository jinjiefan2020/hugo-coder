---
title: "The Mystery of HarmonyOS"
date: "2021-06-01"
categories: 
  - "software"
  - "telecom"
tags: 
  - "arc-compiler"
  - "compiler"
  - "harmonyos"
  - "huawei"
  - "javascript"
  - "lvm"
---

Afraid of being accused of capitalizing on a trend, I waited a whole month before publishing this article. During that time, countless media outlets hyped and inflated the information, but valuable content was scarce.

This article explores the evolution of HarmonyOS to its current state of being a "last resort" option through investigating its origins and rumors, focusing on its pure technical aspects.

### One, 2012 Laboratory.

"HarmonyOS is a brand, which is a combination of multiple sets of core systems."

The key to HarmonyOS used to be the Ark compiler, which was also the development codename for HarmonyOS. Thanks to some former leaders of the Ark team who have posted their memoirs online, we can piece together what happened back then.

In 2012, Huawei had an impressive organizational structure for their laboratories, which involved setting up research and development labs all around the world. This allowed talented individuals who didn't want to work in Shenzhen to stay in their own communities without having to uproot their families.

Of course, headhunting is also more convenient, with many laboratories located near other giants.

From the DSP on the base station to the later Kirin and Kunpeng, it has become increasingly necessary for Huawei to have its own compiler team to achieve performance optimization and proprietary instruction set, and so on.

The beacon of the world's software is in Silicon Valley, which is why Huawei's compiler team is based at its US research facility. One of the beacons of China's software industry is located in Hangzhou, where the country's compiler teams are concentrated at its research facility.

In 2014, Meiyen Institute invited the chief architect of Open64 compiler, Mr. Zhou Zhidé, to visit. Perhaps due to the decline of Open64 and the rise of LLVM supported by Apple, Mr. Zhou and his team created the predecessor of the Ark compiler, the Maple compiler, in defiance.

There are various opinions online regarding why Maple was renamed to "Fangzhou". One theory is that "Fangzhou" sounds similar to the English name of the CEO, Zhou, which is Fred Chow. Another theory is that it is in line with the name of the 2012 laboratory, as it was believed that a great disaster was approaching and an ark (Fangzhou) was needed to save lives.

After Meng Wanzhou was detained by the Maple country(Canada), changing the name has become a trend. However, even today, a large number of file names in Fangzhou still retain Maple or Mpl.

Futurewei, a subsidiary of Huawei based in the United States, has faced a legal paradox following sanctions imposed by the US government. Although Futurewei is an American company and thus immune to sanctions from the US government, restrictions have been placed on its ability to transfer technology to its parent company. Additionally, Huawei employees have reportedly been prohibited from entering Futurewei.

Perhaps for this reason, Huawei is very cautious about compliance with open source modules, after all, even external contributions from the United States must be considered for deletion or modification. If this is one of the reasons for "secured open source", I believe it is particularly understandable.

### 2\. The direction of the compiler's attack.

Most modern advanced compilers are structured into three layers: front-end, middle-end, and back-end. The front-end translates various languages, the middle-end optimizes the code, and the back-end generates machine code corresponding to different types of CPUs. Intermediate optimization often uses an intermediate representation (IR), such as MapleIR.

The original text is in Chinese. Here is the translation in English: It is said that Chow designed Maple with the intention of using JavaScript for the front-end, namely MapleJS, in order to achieve cross-platform capabilities and optimize its performance on lightweight smart IoT devices.

By chance, Huawei's Consumer Business Group (CBG) came up with the idea of using static compilation of Java to achieve a speed advantage over rival Android manufacturers while striving for differentiation. They collaborated with several teams and embarked on a project to tackle MapleJava in 2012.

Although everyone knows that the Java Virtual Machine is resource-intensive and Android code can be cumbersome, the idea of challenging Google's top experts in the field and optimising the virtual machine (ART) for 10 consecutive years, is undeniably bold.

Subsequent facts proved that the idea of MapleJava was a bit naive.

### 3\. MapleJava's setback.

MapleJava 1.0 (or Ark 1.0) can be considered a success, as it proves that certain statically compiled apps can run faster than on Google's virtual machine.

At this time, coinciding with the unwarranted sanctions imposed by the United States, President Yu made a high-profile announcement about HarmonyOS and Ark Compiler. However, MapleJava was still just a laboratory product at that time.

Next, the task of Ark 2.0 is clear, to compile and adapt various commercial apps and optimize Ark runtime.

With the abundance of compatibility issues, it is obvious that Android's ecosystem cannot be easily disrupted by a single compiler after a decade of development. Even if we replace ART with Ark runtime, we are unable to entirely circumvent Android's core services.

As a result, the political significance of this whole matter has greatly diminished due to the inability to fully eliminate Android.

More importantly, putting aside various negative factors such as bugs and compatibility issues, the speed difference between apps compiled by Ark and standard Android apps is not as large as expected. So what is the significance when both are sufficiently smooth?

Starting today, MapleJava's plan has been put on hold. This may be one of the reasons why many of the members in this team of a hundred have resigned.

Objectively speaking, MapleJava is a very impressive attempt that at least circumvents the Google virtual machine. Unfortunately, the corresponding runtime of MapleJava has not been fully open sourced, which prevents developers from continuing to tap into the potential of statically compiling Java apps.

Just a few days ago, Microsoft announced that its latest Windows 11 will natively support Android apps on x86 using the Intel Bridge compiler.

### 4\. Who does HarmonyOS benchmark against?

The setbacks faced by MapleJava led to a series of publicity challenges later on, causing many misunderstandings in society regarding the overall strategy of HarmonyOS.

Huawei insists that there is a connection between the open source LiteOS (later renamed Open Harmony) and the mobile HarmonyOS, even though their kernels are different. We believe that this association may refer to the Ark compiler and communication protocols.

Early open source of Ark may be more important as it practically demonstrates the courage to challenge giants. Ark's open source includes MapleC, which could be viewed as a path that competes with Clang-LLVM->Apple Swift. If HarmonyOS chooses this path, it should be the only option for HarmonyOS to catch up with Apple's iOS performance.

Apple is statically compiled, and when combined with their in-house compiler optimized for their self-designed CPU/GPU/NPU, the performance far surpasses that of Android. Additionally, the hardware overhead is minimal.

However, there is still a gap of many years for the MapleC route. Convincing developers to use the low-efficiency C/C++ language to develop native Harmony OS programs is an impossible challenge.

Therefore, there are rumors that Huawei will introduce its own language, "Maple+ Cangjie," to truly compete with Apple's Swift. However, the learning cycle and ecosystem development for this new language require a very long time and investment.

Related to this, if Huawei cannot obtain the authorization for ARMv9 in the long term, the optimization of Cangjie may need to switch from ARM to RISC-V. However, the ecological gap of RISC-V is still too large, making it a dilemma on how to proceed with the choice.

So after MapleJava, what is Huawei's choice?

Although the latest HarmonyOS architecture diagram refers to Ark runtime as "multi-language" runtime, many people believe that Javascript (MapleJS) is the main player.

### 5\. JavaScript Selection

Javascript is the hottest full-stack language in recent years, with the highest development efficiency and cross-platform support. It can even be embedded as a sub-platform within a platform, as demonstrated by the typical example of WeChat mini-programs.

The pioneer of using JS to make mobile apps is Palm's WebOS. The design philosophy of WebOS and Palm Pre mobile phones was very advanced: multitasking cards, full-screen gestures, wireless charging, and so on were all copied by Apple and Android many years later.

The forward-looking architecture of WebOS, which utilizes a standard Linux+JS front-end, surpasses its time. However, during that period, hardware support for JS apps was still somewhat inadequate, and even programmers did not regard JS as a language.

After the failure of WebOS, Samsung's Tizen/JS took over to fight again, but it also ended in failure.

Years later, JS has achieved unprecedented development. With the resurgence of JS ecosystem such as KaiOS and PWA, coupled with the redundancy of hardware performance, the chances of successful implementation of native JS applications on HarmonyOS have increased. Applications such as online banking and e-commerce, which originally did not require high performance and were implemented using Webview technology, have encountered no obstacles.

Google's ChromeOS and powerful V8 engine also endorse the feasibility of expanding HarmonyOS to the desktop field with JS.

Of course, there are significant challenges to developing a native JS app for mobile phones. Adapting existing frameworks such as RN, Weex, or Webview can be quite cumbersome, and it is difficult to call upon underlying hardware and utilize GPU features, resulting in a negative impact on gaming performance. In this regard, I am eagerly anticipating technological breakthroughs from MapleJS.

### Sixth, Practical Approach.

Prior to the establishment of the JS ecosystem mentioned above, the practical approach of HarmonyOS mobile was to support both Android AOSP and native JS applications. However, the HarmonyOS mobile system has not been fully open sourced and the development framework of MapleJS application remains unclear. Therefore, most of us only see AOSP and there have been voices outside saying "wrapped Android".

In the context of AOSP being open-source, it is indeed confusing as to what value lies in creating another set of non-open source phone ecosystems.

If the chip fabrication issue can be ultimately resolved and various IP cores that have been trimmed down are still available for purchase, it would be a highly courageous and commendable move for Huawei to return to the integrated software and hardware path of HarmonyOS, Cangjie input method, and Kirin chips. Here, we first give a thumbs up to the HiSilicon team at Huawei.

The open-source HarmonyOS (LiteOS) for smart devices has its own intellectual property rights in China, and its value in the thriving open-source IoT ecosystem is beyond the scope of this article.

Currently, we can see that the communication mechanism (distributed software bus, also known as "Internet of Everything") among various HarmonyOS devices has become the biggest selling point of HarmonyOS.

### 7\. Google's Fuchsia.

Coincidentally, before the release of HarmonyOS 2.0, Google officially announced Fuchsia. Contrary to what many had speculated, Google kept a low profile and did not describe the future prospects of Fuchsia. It only said that it is a brand new, secure operating system suitable for "connected devices".

From an architectural point of view, Fuchsia is highly modular and suitable for rapid development through assembly. It seems to be patiently waiting for various modules (wheels) to be built, and encourages developers to try new technologies like Rust, Dart and Flutter... This indicates that Google is not in a hurry this time.

No one knows the future relationship between Fuchsia and Android, including Google itself. For Google, getting rid of Linux GPL and outdated JDK has always been a dream, but it knows it takes a long time and opportunity, so it can only keep a low profile.

Attempting to compare open source HarmonyOS 2.0 and Fuchsia is probably pointless as they have very few similarities, except for both claiming to have a microkernel.

### 8\. Vision.

It is worth gossiping about that Chris Lattner, the father of LLVM and Swift, jumped ship from Apple to become the head of Autopilot at Tesla, and still wanted to introduce Swift to Tesla. However, due to differences in his philosophy with Elon Musk, he resigned after only six months.

This appears to be a failure to switch from a mindset of tools to applications. The obsession with creating sharp knives has surpassed the purpose of cooking.

Of course, to hastily evaluate a master shows my own foolishness to some extent. Here, I only want to offer my sincere blessings to HarmonyOS and not forget the original intention due to an infatuation with so-called tools.

From my personal narrow viewpoint, the vision of HarmonyOS is still not clear enough: what it ultimately brings to users and industries; how different is "Internet of Things" for users compared to current industrial control and smart home systems.

If HarmonyOS abandons the ultimate goal of benchmarking with Apple's performance, and instead focuses on emotional and usage differentiation compared to Android, choosing a practical and helpless approach in the situation where chip issues remain unresolved, it may disappoint some developers.

### Nine, Challenges of the Future.

Although Huawei has accomplished a significant shift from CT to IT in its product line, it must be candidly admitted that there still exists a gap in its core IT technologies such as CPU, GPU, OS, and vital software. Moreover, Huawei also needs to divert its resources to construct a chip production system that can compete with those of the United States, which makes the overall challenge enormous.

Even in this small field of cross-platform programming, we have seen the impressive capabilities of Intel's Bridge and Apple's Rosetta. While emotionally we hope to see a Chinese company dominate the global technology giants in all aspects, we still need to stay grounded and approach it with a practical and realistic mindset.

If Huawei can fully leverage its leading advantages in CT, it may become the dominant player in the core CT by combining patented components and software IP components, which is perhaps more in line with CEO Ren's "software-focused" strategy this year. A perhaps inappropriate small example is the "multi-screen collaboration" feature from last year, which is quite good.

Taking cues from Microsoft's shift from criticizing open source to embracing it, I believe that Huawei should reconsider leading the Open RAN movement.

In extremely difficult situations, Huawei has demonstrated extraordinary bravery and resilience. "Softwareization and IP patentization" may be the "golden armor forged in a hundred battles" before the company's rebirth from the flames.
