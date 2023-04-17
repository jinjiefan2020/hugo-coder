---
title: "A Short Story about BIOS and PC"
date: "2019-01-01"
categories: 
  - "software"
  - "start-a-business"
tags: 
  - "ami"
  - "bill-gates"
  - "bios"
  - "efi"
  - "insyde"
  - "intel"
  - "microsoft"
  - "phoenix"
---

![图片](../images/image56.png)

Most of the previous reports by Chinese journalists about Bill Gates were inaccurate. They claimed that he dropped out of school and founded Microsoft after his mother, who was a member of IBM's board of directors, secured a collaboration opportunity for him to develop the operating system for IBM PC. However, Gates actually founded Microsoft in 1975, and the collaboration with IBM did not happen until 1980. Furthermore, Gates' mother was not a member of IBM's board of directors.

The truth of things is sometimes not as fun as it seems. Bill Gates studied law at Harvard because his father was also a lawyer, but he truly didn't like studying law and spent all his time on computers. In his spare time, he and his fellow Bostonian Paul Allen developed an interpreter for the BASIC language.

In January 1975, the two individuals were reading a magazine when they saw the advertisement for MITS' Altair 8800 computer and thought they could sell their interpreter to MITS. They were successful, and Allen was even hired by MITS, which was located in Albuquerque. In April, the two individuals registered their briefcase company, Micro-soft (which initially had a hyphen in the name). At this time, Gates had not yet dropped out of school.

Harvard University is not an easy university to fit in. Male societies and female students prefer handsome and athletic men, both of which are absolute weaknesses of Gates. His academic performance was also affected by his involvement in computer, causing him to fall behind on his credits even after completing his junior year. He was unhappy with his studies and life, and dropping out may have been a way of escape.

In 1976, Gates moved to Albuquerque and at the end of the year, Allen resigned from MITS. In 1977, the two officially signed a partnership agreement. In 1979, due to a shortage of talent in Albuquerque, the two moved Microsoft back to their hometown of Seattle.

It is worth gossiping about that in 1977, Ed Roberts, the founder and chief engineer of MITS, sold the company for millions of dollars and bought a large farm. At the age of over 40, he went back to college to study medicine and eventually became a doctor, transforming from an amazing electronic engineer to a doctor. What an incredible life.

In 1980, Bill Gates' mother, Mary, met John Opel, the chairman of IBM, during a meeting for a nonprofit fundraising organization where they both worked part-time. She mentioned her son's company to Opel, who was helpful in introducing them to some executives. Gates then proceeded to discuss a collaboration for a PC operating system.

However, at that time, Microsoft did not have an operating system, only a BASIC interpreter. The most popular and mature microcomputer operating system at the time was CP/M, but when IBM went to negotiate a partnership, they refused to sell. This was a godsend for Microsoft, who quickly bought a CP/M-like operating system called 86-DOS from SCP, also located in Seattle. It was written by a 22-year-old Tim Paterson in assembly language over the course of several months. The earliest version of MS-DOS can currently be downloaded with its source code, which includes a letter from Tim Paterson.

I'm sorry for the long and gossipy introduction, but our protagonist BIOS is finally making an appearance in the story.

### One,

After the release of the IBM PC, it achieved great success. However, at that time, IBM surprisingly did not set any patents on the PC, which led to the appearance of nearly one hundred clone machines claiming compatibility in the first two years. They bought CPUs from Intel and DOS from Microsoft, and ultimately sold at only half the price of IBM's. However, they were missing one thing: BIOS (Basic Input Output System).

BIOS is an assembly program used to arrange power-on self-test and booting to the operating system on PCs. IBM "accidentally" published the entire source code of this program in its technical documentation, thereby enabling compatible machines to plagiarize it. However, due to IBM's copyright ownership of the BIOS, plagiarism is illegal. In 1983, following a similar case of Apple suing Franklin for producing compatible machines, IBM compelled many companies to withdraw from the compatible machine market.

At that time, a relatively unknown company called Phoenix Technologies rescued everyone. Phoenix used a reverse engineering method called "clean room", where Group A engineers studied IBM source code to write development requirements and documents, while Group B engineers, who had never seen IBM source code, developed based on the documents provided by Group A. The two groups were separated by a so-called "Chinese wall" to prevent opposing attorneys from using the word "plagiarism". In May 1984, Phoenix released its own BIOS and began licensing it to compatible computer manufacturers, clearing the final obstacle for the compatible computer market.

![图片](../images/image57.png)

At that time, when AT&T was broken up due to allegations of monopoly, IBM, though unwilling, was afraid of being labeled as a monopolizer, and quickly gave up its crackdown on compatible machines. However, because Phoenix's BIOS was written very well, IBM subsequently handed over the task of writing its own genuine PC BIOS to Phoenix. Until today, the mainstream ThinkPad BIOS is still provided by Phoenix. Some brands, such as Compaq and Toshiba, have their own in-house developed BIOS.

### Two,

In 1985, China also produced the widely popular compatible machine Great Wall 0520CH. Lenovo, founded in 1984, did not release its own compatible machine until 1990.

In 1985, Subramonian Shankar, a first-generation Indian immigrant, was personally invited by Michael Dell, the founder of Dell Computers, to design the 386 motherboard in Austin. This brilliant engineer not only completed the entire motherboard and BIOS work, but also designed the famous Turbo button, which could increase the CPU frequency from 8MHz to 16MHz with a single press. However, Dell abandoned the first-mover advantage due to concerns about the instability of the 386, which led Shankar to establish American Megatrends Inc (AMI) in Atlanta. And because Phoenix BIOS was too expensive, he used the same "clean room" method to create his own AMI BIOS.

"Afterwards, Phoenix and AMI, this pair of arch-rivals, started a competition that lasted for over 30 years."

Apart from these two companies, there are multiple other enterprises in the BIOS industry, such as Quadtel, Award, General Software, etc. However, they were later acquired one by one by Phoenix. Phoenix is like a sword sect, constantly introducing new and innovative sword techniques, which are then constantly broken. AMI is like an airbender, persevering and diligently training their inner energy for decades, finally standing at the summit of power.

### Three,

Award Software is also one of the earliest independent companies to develop BIOS software. If you have ever built a DIY computer in China, over 80% of you have seen the screen below.

![图片](../images/image57.png)

Award BIOS is as reliable, easy to use, and affordable as AK47, making it a favorite among Taiwan's motherboard manufacturers. In 1993, the Taiwan-based GCH company, founded by Huang Zhao Feng, acquired Award. In 1996, Award went public on Nasdaq. However, although Award BIOS has a significant share of desktop motherboards, it lacks a large PC brand and notebook product line, making it difficult to increase prices and limiting its profitability. Just over a year after going public, Award was acquired by Phoenix.

It can be said that the early 2000s were Phoenix's golden age, with the Award product line controlling the low-end market and Phoenix BIOS dominating the high-end market. At that time, AMI was almost not taken seriously. Phoenix even openly challenged Intel's authority and took an adversarial stance against Intel's introduction of UEFI, attempting to form an alliance with Microsoft to deep-bind BIOS and Windows to implement digital copyright and other security functions. Feeling threatened by Phoenix's market share, Intel began to support AMI (switching from Phoenix to AMI for public BIOS), and invested in a BIOS company specializing in UEFI, Insyde, located in Taiwan. Seeking revenge against Phoenix, Intel spent ten years before finally succeeding.

Compared to privately owned companies like AMI controlled by its founders, the drawbacks of Phoenix being hijacked by public companies and professional managers have gradually become apparent. On the one hand, managers pursue expansion in application software to tell stories on the stock market; on the other hand, in order to pursue temporary performance, they turn copyright fees that should be collected according to the number of shipments into one-time purchases for customers. For example, it is equivalent to selling future revenue at a 50% discount in one quarter. As a result, some managers laugh and take their bonus before running away.

In 2006, this model collapsed leading to huge losses. Phoenix's new CEO and COO/CFO took office. At that time, I was in charge of mainland China business and once accompanied the COO on a visit to customers in Beijing. The COO was a sixty-year-old American man who, upon facing several VP customers, confidently declared, "Let me tell you our amazing story." He then dazzled the customers with his eloquent speech and recommended products that did not actually exist.

It should be said that this tactic has been quite successful. The promotion of these non-existent or highly immature products has driven the stock market to new highs, and then they used high prices to acquire several inexplicable companies, only to leave and search for new targets when the companies entered another round of losses.

### Four,

Let's turn our attention back to Intel's UEFI, which is an architecture designed to replace the old Legacy BIOS. UEFI has many advantages, such as greater functionality and strong extensibility. It is developed using the C language, which is not as difficult as assembly language required by the BIOS. However, due to resistance from Phoenix and a lack of strength in Intel's software department, the early versions of UEFI were very immature. After approximately 8 years, a usable version was finally released, but only after much difficulty.

The field of BIOS is labor-intensive for programmers, and each type of motherboard requires specialized engineers to do porting, which is a very large job. This is the most unprofitable software business model because you cannot simply copy your program to make money. Moreover, programmers in this field are almost unable to work in other fields, such as internet programmers cannot work in BIOS.

In 2008-2009, Intel ordered that new platforms must only use UEFI and could no longer use Legacy BIOS. At this time, Phoenix was already quite weak, having been basically defeated by AMI in the desktop and server fields, and in the traditionally strong notebook field, it was forced out by Insyde's UEFI. In 2009, Phoenix was forced to lay off all of its research and engineering teams in Shanghai and Nanjing.

In 2010, Phoenix was delisted after being acquired by a private equity fund for only 139 million US dollars. Freed from the pressure of disclosing financial reports, Phoenix was revitalized and repaired its relationship with Intel. That year, during a chat with the boss, it was suggested that it might be better if Zhou Hongyi acquired the company, as there was a customer base of several hundred million and it was the most secure bottom layer, with the potential to produce something new.

Today, in the BIOS industry, the three major players are AMI, Insyde, and Phoenix. However, AMI has proclaimed themselves as the number one, which is likely true considering they currently have the largest team (1500 staff, 85% of which are technical personnel) and the founder and CEO who sincerely loves the company.

![图片](../images/image57.png)

### Five,

The story of BIOS has concluded, and the lesson for today's technology companies is this: going public may be a curse. When the company's founders cash out and depart, no one truly loves the company anymore. A strong corporate culture is the key to long-term success.
