---
title: "War of Java - Part 1"
date: "2019-04-01"
categories: 
  - "software"
tags: 
  - "google"
  - "java"
  - "larry-ellison"
  - "oracle"
  - "steve-jobs"
---

### Epilogue.

In May 2019, the thoroughly disgruntled Trump administration launched a war against Huawei, resulting in Google being forced to revoke Huawei's Android authorization. The copyright issues surrounding open-source software bring to mind a shocking case in the software industry.

Friends who have watched "The Story of Mobile Baseband Chips" must remember that Steve Jobs had strongly expressed his anger over Google's plagiarism of Apple: "I will use all of Apple's 40 billion US dollars in savings to launch a thermonuclear war to destroy Android, because it's a stolen product."

Do not think for a moment that Joe Boss just says things for fun.

Although he passed away as a immortal many years ago, his best friend, Oracle Chairman Larry Ellison, is still committed to this unfinished business.

The rebellious and unconventional Ellison, when reflecting on the scene of Jobs' death, emotionally stated, "He had been consumed by cancer, he was just too exhausted and in too much pain. Although he was undoubtedly the strongest person I had ever met, in the end he gave up the fight against death. His decision to stop medication shocked everyone, and three days later the founder passed away."

![图片](../images/image60.png)

As fellow heroes who share the same beliefs, Ellison once wanted to buy Apple back and return it to Jobs.

In April of 2009, Oracle announced its acquisition of Sun Microsystems for 7.4 billion US dollars.

Ellison did not hesitate in his bidding war against IBM, ultimately acquiring it at a cost exceeding 30% of Sun's market value.

After the completion of the acquisition in 2010, Ellison immediately declared war on Google and sued Android for infringing on Java.

### One,

James Gosling, the creator of Java, is a Canadian who worked at Sun for 26 years. He decided to leave after Sun was acquired by Oracle.

There is a rumor that Gosling created Java by removing many complex features from C++ because he found it too difficult to learn. This is not believable as Gosling is a computer scientist with a PhD from Carnegie Mellon University, and learning a programming language is a trivial matter for him.

Java was originally designed for small devices such as set-top boxes. However, to everyone's surprise, with the advent of the Internet, the feature of writing Java code once and running it everywhere has been exploited to the fullest by various applications. In enterprise-level software, Java is even more of a tool to integrate various different hardware and operating systems to create distributed applications.

For the past 20 years, Java's unshakable position as the backbone of the Internet remains intact due to its possession of the most mature and stable enterprise application components, despite the challenge posed by .net.

### Two,

Not only does Java dominate the enterprise market, it has also unexpectedly become a popular choice for mobile device development.

Andy Rubin, the father of Android, joined Apple in 1989 as a small engineer. Because he had previously worked in the robotics department of Zeiss, his Apple colleagues gave him a nickname: Android (robot). At that time, no one knew that this robot would become Apple's biggest competitor after many years.

At that time, Steve Jobs had already been expelled from Apple. The CEO John Sculley, who was invited by the late Jobs to "change the world without selling sugary water," was actually far from the later criticized portrayal. He expanded Apple's revenue by ten times and presided over the development of the handheld computer Newton with a large screen.

Sculley split the department that specialized in handheld operating systems into General Magic (what a cool name!), which became the West Point for future smart phones.

Andy Rubin obtained sufficient nutrients from General Magic Corporation and later founded Android Inc. in 2003. The Android system was originally designed for digital cameras, which vary greatly in hardware, hence Java's excellent cross-platform capabilities were selected.

As a result, after this platform was developed, it was found to be very suitable for use on mobile phones. In 2005, Google, which was looking for a mobile operating system, took notice and acquired Android Inc.

### Three,

In January 2007, Steve Jobs released the iPhone, shocking Google greatly. In order to catch up with the times, Google did not have time to change the programming language Java used in Android. This later proved to be a significant issue.

Of course, the ample community of Java programmers and convenient development features are of great assistance to Android itself.

In November 2007, just four months after the first generation iPhone was released, Google hastily open-sourced Android and established the Open Handset Alliance (OHA). At this time, Android could not even be considered a half-finished product, but the position of Java was firmly established.

Unlike the machine code compiled by native Objective C on Apple iOS, Java must run on a virtual machine. This naturally poses a speed problem for Android. In order to increase speed as much as possible, Google created the Dalvik virtual machine (DVM) themselves.

DVM has adopted many "cheating" acceleration methods, such as preloading many apps (APKs) installed by users and storing them in the cache, and replacing Java bytecode with DVM instructions. One of the side effects of these methods is that Android requires much more memory than iPhone, and the more time used on the phone and the more apps installed, the slower the system becomes.

These "cheating" methods also make Google's Java Virtual Machine completely incompatible with Sun's original virtual machine. Sun cannot tolerate this behavior that splits Java.

### Four,

Google did apply for a Java license from Sun, but was refused when Sun requested control over the Android branch. Google also declined Sun's proposal of paying around 50 million USD for three years, and after Sun was acquired by Ellison, the final settlement exceeded 5 billion USD, over 100 times the initial proposal.

Without obtaining authorization from Java, Google used a reverse engineering method called "clean room" (as can be seen in the stories of BIOS and PC) to develop its own Java library. This is a method similar to plagiarism, but not obviously illegal.

However, Google still retained some of the original programming interfaces (APIs) of Sun Java, which later became a handle for Oracle.

Oracle's Chief Corporate Architect for their Database programs, Edward Screven, testified in court stating that he talked with Ellison and affirmed that acquiring Java was the sole important objective for buying out Sun.

Although Java's creator Gosling briefly joined Google after leaving Oracle, he stated in an interview that he believes Google did trick Sun in the past.

### Five,

Open source software simply means that you can see all the source code, but it does not mean that you can use it freely. For Java, programmers can use it for free, but enterprises still need to obtain authorization.

There has been a great deal of controversy within the legal community in the United States over whether APIs are protected by copyright law. Just as the recipe for a dish can be protected by copyright, does the menu for ordering that dish also enjoy protection?

The prolonged legal battle between two giants, Oracle and Google, over the use of Java code in Android, has been ongoing for 9 years now without a final verdict. Throughout this time, both parties have won and lost in various courts, and there seems to be no consensus among judges and juries regarding this case.

Larry Page and Sergey Brin personally testified in court, which is extremely rare in large corporate litigation in the United States, and each time, Ericsson refused to settle.

In March 2018, the Federal Appeals Court ruled in favor of Oracle, which means that Google should compensate up to nearly $10 billion.

Google has submitted this case to the United States Supreme Court for the second time. Four years ago, when the Supreme Court refused to review it, these nine justices seem to be forced to make a ruling this time.

As is well known, the United States is a country where judges make laws. The rulings of the Federal Supreme Court will have a far-reaching impact on many unresolved cases in the software industry.

Judges also have to decide whether Google's plagiarism was intentional infringement or fair use. Oracle has presented evidence that Android has generated over $42 billion in revenue for Google over the past decade.

The disadvantage for the oracle bone script is that Android has become too big to fail, and no judge will support a ban on the sale of Android phones. It is precisely for this reason that Google has been dragging the case on for nine years.

With sufficient time available, Google has migrated the Android Java library to OpenJDK, the DVM to ART, and the Java language to Kotlin.

### Six,

At the end of April 2019, the Federal Supreme Court officially issued a statement to the US Department of Justice, requesting that federal prosecutors assist in the case. This seems to be a loophole in the separation of powers in the United States, but it also shows that the difficulty of this case is extremely high.

It seems that most programmers detest Oracle's dominant behavior towards open source, but Ellison's move to avenge Jobs is truly touching. After all, it is true that Google has committed acts of "copying" Apple and Java and has thus gained enormous profits.

Considering my feelings towards Joe and the situation with Huawei, deep down I still hope that Google will ultimately pay the price.
