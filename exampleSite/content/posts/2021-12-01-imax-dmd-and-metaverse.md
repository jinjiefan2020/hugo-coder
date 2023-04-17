---
title: "IMAX, DMD, and Metaverse"
date: "2021-12-01"
categories: 
  - "semiconductor"
tags: 
  - "dlp"
  - "dmd"
  - "imax"
  - "metaverse"
  - "oculus"
  - "quest-2"
---

Due to well-known reasons, Canada's image has taken a big hit in our country over the past three years. Having lived there for a few years, I have some insights, and considering that the situation has somewhat improved, today we will explore the complex topic in the headline along an uncommon path.

### 1\. Introduction.

The system in Canada is actually very different from that of the United States, and it resembles that of Northern Europe to a greater extent. Due to the relatively well-established welfare system, the enthusiasm of the working people to work 996 is very weak.

The leisurely and cold life not only leads to laziness, but also brings about a fair amount of innovation. However, with a population of over 30 million, it is quite challenging for us to compete with the United States in the market. Examples include:

- Blackberry vs Apple
    
- Corel vs Adobe
    
- ATI vs Nvidia
    
- Maple vs Mathmetica/MATLAB
    
- Shopify vs Amazon

......

However, when it comes to certain consumer goods that require a certain taste, Canada has some old-fashioned imperialist cultures that are characterized by arrogance, such as:

......

The Four Seasons Hotel is favored by business people.

The Fairmont Hotel is favored by tourists.

The Bombardier Global is favored by winners in life.

Arc'Teryx is favored by men.

Lululemon is favored by women.

The characteristics of the aforementioned brand are that they never compromise on price, but also truly excel in terms of quality.

Another Canadian brand with similar features is our protagonist for today: IMAX.

### Two, IMAX.

Watching a movie in IMAX is typically a distinct experience because IMAX films are produced and screened in a closed, high standard environment. This requires a refined taste and cannot be replaced by simply installing a large screen.

"Large" and "clear" are two relatively contradictory indicators, but if there is a lot of money, then it is not a problem.

The enormous commercial IMAX screen has an area of 800 square meters, and only the IMAX 70mm film (15/70) with a high resolution of 18K can truly meet its requirements. Unfortunately, although IMAX has a complete film screening plan, there are hardly any movie theaters that can afford or sustain it besides science museums and exhibition halls.

At the same time, there are not many directors who can afford to use 15/70 film. In fact, there is no commercial film that is entirely shot on IMAX 70mm film, such as the latest James Bond film "No Time to Die" which only has 40 minutes.

Although I feel that the price of 300 yuan per ticket for IMAX film theaters, which are considered the ceiling for movie watching, is reasonable, it is obvious that most of the audience does not agree and there are not enough movies to show. This has forced IMAX to compromise with the market and its competitors.

IMAX's early mission was to be "big" (Max), but with the advent of the digital wave, IMAX isn't as focused on "big" anymore. Most IMAX digital cinemas have screens that are much smaller (3-6 stories high) than flagship theaters (10 stories high).

IMAX has about 1,600 cinemas worldwide, with nearly half of them located in Greater China. Although IMAX holds less than 5% of the market share in China, various competitors still emerge in the usual fashion. It should be acknowledged that IMAX has indeed made considerable compromises in terms of quality in this environment.

After all, with the digitalization of movies, the technological threshold has significantly lowered. It is not difficult to buy a few projectors and package them. Your IMAX also only has a 4K resolution digital projector.

The gap between 4K digital and 18K film represents one of the rare defeats on mankind's journey towards digitalization.

### 3\. The magical DMD.

As most viewers are satisfied with 4K, the core component manufacturer of commercial projectors, Texas Instruments (TI), has never introduced a native DMD for 8K. This is a great pity for movie fans.

In my articles, I have never talked about a type of chip called MEMS (micro-electro-mechanical systems). Today, let's talk about the king of MEMS - DMD (digital micro-mirror chip).

A 4K LCD has 8.3 million pixels, while a 4K DMD has 8.3 million tiny mirrors that can independently flip on an array measuring less than 2 centimeters on the diagonal.

![图片](../images/image49.jpeg)

The small mirror under the electron microscope can be flipped 12 degrees in two directions.

In the process of pursuing limits, a large part of humanity is engaged in a struggle with light. For digital projection, this means dividing a beam of light into millions of strands and independently controlling each one.

During the research and mass production of DMD, TI experienced intense internal opposition due to the extreme difficulty. According to TI's friends, DMD did not earn much money in the first few decades.

What is difficult about it?

### Four, the great DMD.

Each aluminum alloy small mirror is deposited onto a SRAM cell, which is several times smaller in cross-section than a hair, and is required to flip in two directions. It's hard to imagine anyone being able to make a motor that small, isn't it?

In fact, the small mirror is cleverly designed to be powered by static electricity, relying on extremely small hinge elasticity for reset.

![图片](../images/image50.png)

The two red wires are the reset keys: they generate torque after the electrostatically adhered mirror is flipped.

This step has been roughly taken for 10 years, trying countless materials and techniques, but it is still not mature. The goal is for each mirror to flip 2 trillion times without damage during its 100,000-hour lifetime, but at that time it was difficult to even achieve 500 hours.

![图片](../images/image51.png)

The calculation of the balance between electrostatic torque and mechanical torque is actually much more complex than this, as it also requires the calculation of how much capacitance is needed for those electrostatic forces, and what is the minimum voltage needed to generate that capacitance.

Finally, the total number of flawless rotations for one million mirrors is a terrifying 100 million trillion times. If this task were assigned to me, I estimate that my heart would resign ten thousand times.

TI engineers have spent over 10 years gathering top experts from various disciplines such as electronics, mechanics, materials, and chemical engineering. They conducted repeated experiments to eliminate any design flaws that could cause failure, and ultimately achieved a micro-structure that is as stable as Mount Tai even in high-temperature environments for projectors.

Nevertheless, the task is probably only halfway done.

How can these small mirrors display billions of colors? How can the displayed grayscale be controlled? How can this special chip be economically manufactured?

The innovation of engineers is truly admirable. A small mirror can rotate thousands or even tens of thousands of times per second, while TI's image processing algorithm can modulate various colors through several hundred switches for red and blue, and several thousand switches for green (duty cycle), and also control brightness/grayscale by switching the mirror thousands of times per second.

This is not easy, because the mirror only has a rotation of 12 degrees, and achieving the complete switching of light entering and exiting in such a small area and angle requires extreme precision. In addition, the duty cycle principle appears to be similar to the later OLED control of each pixel's driving chip, but the first to try something new is always more difficult, considering the minimum frequency that the human eye can accept.

This solution is none other than the renowned Digital Light Processing (DLP).

The biggest advantage of DLP projection is that its light does not have huge losses when passing through like liquid crystal, and its contrast is also much higher than that of liquid crystal projection. For high-end three-chip DLP machines, precise color and black levels are unmatched by liquid crystal.

### 5\. How is DMD manufactured?

We have discussed a lot about knowledge regarding semiconductor manufacturing, and now we need to delve even further.

The typical MEMS module consists primarily of sensors, which are coupled by stacking a silicon CMOS unit with a MEMS unit. The input is analog variables such as sound, light, and electricity, while the output is mostly simple numerical values or switches that usually have low precision requirements for processing.

The difficulty of DMD is much, much greater- with inputs of values for millions or even billions of colors every second, and outputs of tens of billions of independent movements of mirrors every second.

![图片](../images/image52.png)

DMD probably requires three additional photolithography steps in addition to producing SRAM:

As a flagship of MEMS, DMD has also strongly promoted the development of various MEMS chips. Later, various highly innovative micro-electromechanical chips emerged one after another, because DMD made everyone realize that there is nothing that cannot be created.

The head of the development team for DMD, Larry Hornbeck, graduated from a second-tier university in the United States called Case Western Reserve University. He spent a total of 13 years in the same field from undergraduate to doctoral studies, finally graduating at the age of 31. It is safe to say that he was not a naturally gifted student.

After graduating, Dr. Hornbeck worked in Dallas for over 40 years, almost exclusively focusing on DMD. In the end, he achieved great success, even receiving an Oscar award.

### Sixth, VR and Metaverse.

After all that has been said, since TI has such a broad moat in DMD, why can't they make big money?

Because of LCD. LCD dominates the vast majority of the display market.

LCD and LED have worked together with dedication, resulting in more grand and rapid technological developments, winning the Nobel Prize for three times.

Personally, I speculate that the biggest opponent for IMAX cinemas will also be liquid crystal: the liquid crystal inside VR goggles.

The biggest differentiation between IMAX and regular films lies in the "immersive experience," and the biggest issue with watching on a large screen TV at home is the difficulty in achieving immersion.

However, VR glasses can solve this problem.

The following video is a recording I made using the Meta/Oculus Quest 2 of the IMAX intro, and the actual experience is almost equivalent to that of a movie theater.

Duration 00:40.

The IMAX intro is carefully crafted and not particularly sensitive to resolution. In fact, although the Quest 2 claims to be almost 4K, it actually only has 2K per eye, which falls short of the clarity we expect from movies.

Technology workers are still striving, such as the so-called fourth-generation semiconductor IGZO applied to the new generation of thin film transistors, making it more feasible to further improve the resolution of compact liquid crystal panels. 8K or even higher VR devices are bound to appear on future roadmaps.

Although there is still controversy over what constitutes the meta-universe, it can be confusing enough to the naked eye to make one forget whether they are in the real world or the digital realm, making it perhaps the most authentic visual meta-universe.

### Translation: 7. Details

The controller for Quest 2 is quite interesting, as it only requires one set of 5th generation dry batteries. Based on my familiarity with motion-sensing games and my years of experience with the Wii controller, I am convinced that lithium batteries would be the superior choice.

However, I was wrong. The power-saving feature of the Quest 2 controller is exaggerated to the point where it can last for six months on a single battery when used at low intensity.

Because its principle is similar to that of a TV remote control, it only needs to emit infrared light with minimal power consumption. The optical tracking technology is difficult because of the four cameras on the VR headset that need to track and accurately locate the controller with almost zero latency. The software and AI algorithms behind this task are extremely challenging. (Note: In addition to the optical tracking, there is also another MEMS chip - TDK Invensense's 6-axis high-precision IMU (accelerometer + gyroscope) - that helps determine the movement of the controller. Its power consumption is also only in the milliwatt or even micro-watt range during sleep mode.)

From the leaked information about Quest Pro, it can accurately capture full body movements, which requires algorithms and computing power that go beyond just capturing hand movements, taking a significant step forward. However, it has been delayed, likely due to the difficulty of the project.

VR is an example, Tesla is another example, and software is becoming increasingly important as a threshold and core competitiveness for host/device manufacturers. Even take a look at ASML that we often mentioned: as early as the early 1990s, a lithography machine had millions of lines of code, and DUV had billions of lines, to EUV with tens of billions of lines.

Many Japanese companies have great hardware, but their software is awful. The lack of attention to detail causes these once-popular products to become outdated. I have mentioned this point before regarding Sony: the remotes with dozens of buttons, the inhuman synchronization tools, and the complicated hierarchical menus.

### Eight, Inward Folding

In the future, the integration of domestic and foreign Metaverse may not be viable, and even the definition of Metaverse may differ from one another. Various virtual reality applications, virtual currencies, and non-fungible tokens (NFTs) have questionable legitimacy and legality in China.

"Coupons" not only involve price cuts to the point of death and labor exhaustion, but also the concept of cutting through utilizing asymmetric information. So, as a consumer or investor, how should one establish their own value judgment?

Many brands and technologies have been mentioned above, most of which have been developed over a decade or even several decades. In the process of internalizing these leading players, we sometimes forget about certain things.

We can see that in the TWS headphones market, numerous overwhelming manufacturers are adopting AirPods.

We can also see that in the electric car market, countless manufacturers are competing with Tesla.

IMAX, DMD, Tesla... even Four Seasons Hotel and Lululemon, they all have some very well thought out details that keep them clear and pure in the midst of chaos and complexity.

In the trend of internal self-inflicted pressure, it is easy to criticize and hurl insults, but appreciating is difficult.

To create details, one must learn to appreciate them.

Recognizing the problems and gaps is the key to establishing a corrective feedback loop.

Finally, lying down and listening to beautiful music, looking at the smiles on children's faces, and finding healing power in the details.
