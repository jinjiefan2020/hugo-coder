---
title: "the Story of Memory(4)-  an update in 2021"
date: "2021-03-22"
categories: 
  - "semiconductor"
tags: 
  - "amd"
  - "dram"
  - "flash"
  - "hbm"
  - "intel"
  - "memory"
  - "nvram"
---

"The Story of Memory" was primarily written three years ago. Taking advantage of this vacation, I will write a short sequel, examining some recent developments in the memory industry over these past few years in a dry and objective manner.

What are the current issues in the field of memory?

"Memory" is a common but not very precise term, which has two main purposes: serving as space for running programs (DRAM, etc.) and space for storing data (NAND, etc.).

After NAND enters the 3D era, its capacity basically has no upper limit, so let's put this discussion aside for the time being.

The main problem at the present stage is DRAM: the slow increase in capacity per unit price and the failure to keep up with CPU speed. This problem is especially noticeable in commercial fields, such as data centers, high-performance computing and operator networks.

In addition, DRAM consumes too much energy because it needs to recharge the small capacitors during every clock cycle.

Electricity cost is the biggest expense for commercial users. On mobile devices, DRAM is also the archenemy of batteries.

In history, to increase bandwidth, DRAM had to continuously increase latency. So, how about increasing cache? The problem is that SRAM and CPU are both expensive and it takes six transistors to store one bit. The cache of the Intel Xeon processor is only one-thousandth of the DRAM.

The unbeatable IBM Power 9 CPU comes with 24 cores and 120MB L3 cache, but at the cost of a die size of nearly 700mm2, which is seven times larger than the Apple A13 processor!

The L2/L3 cache in Power9 occupies such a large area, yet it is only around 100 megabytes.

The main core issue in the memory industry is the increasing demand for capacity speed and power consumption, which cannot be matched by the technological bottleneck of DRAM.

Two, DDR5.

Due to the inherent limitations of DRAM, its technological progress has always been a painful process. The small advancement from DDR3 to DDR4 took five years to achieve. DDR4 was first released in 2012, and DDR5 has yet to be released today (Note: GDDR5 graphics memory is just a variation of DDR3).

The DRAM standard is formulated by the JEDEC JC-42 working group. Although there is a voting mechanism, the pace of DRAM development has actually been led by Intel.

The reason is very simple, Intel has determined the PC roadmap: the CPU or northbridge chip will determine when to support new standard memory.

Thanks to the advancement in semiconductor technology, the core voltage of DDR5 has dropped from 1.2V in DDR4 to 1.1V, which is expected to save 20% power consumption.

The Burst Length and Prefetch of DDR5 have increased from 8n to 16n compared to DDR4, thus doubling the bandwidth in the case of unchanged clock frequency. In order to control various signal interference and jitter problems caused by high speed, DDR5 also introduces various optimized adjustments to the core clock. The new On-die ECC feature is also great news for servers.

However, these will also bring more design, testing, and compatibility challenges, requiring significant changes to the CPU (including memory controller). From the current perspective, it will probably take until year 2022.

1. LPDDR5

LPDDR5 is mentioned separately because it has already diverged from the standard DDR since LPDDR4.

Although there are many common new technologies used in both LPDDR5 and DDR5, their focus points are quite different. LPDDR5 prioritizes power efficiency over speed, while DDR5 prioritizes speed over power efficiency.

Because LPDDR4 already has 16n prefetch, LPDDR5 mainly relies on bank grouping access to achieve speed improvement. Its goal is ultra-low power consumption, so the supply voltage and core voltage are lower than DDR5.

Intel has slowed down the pace of technological progress in the x86 domain, but the situation is different in the mobile field.

Intense competition and annual flagship product releases drive companies to constantly compete with the latest technology.

LPDDR5 is just an example.

The use of LPDDR5 in Xiaomi 10 is indeed a big thing, which shows Qualcomm's aggressive product strategy. The follow-up models of OnePlus 8 and Samsung S20 have basically set the tone for high-end smartphones this year.

Huawei is facing a rather awkward situation, as American company Micron is currently the main supplier of LPDDR5. Samsung is estimated to prioritize its own supply, while Hynix seems to be more focused on standard DDR5. In the case of LPDDR5 supply difficulties, it is a dilemma for Huawei in terms of product planning whether to provide support for the next generation of Kirin.

Three, HBM.

For applications that require high bandwidth urgently, such as gaming and high-performance computing, high-bandwidth memory (HBM) is an excellent solution that bypasses the traditional DRAM IO enhancement mode evolution.

（图：AMD)

(Image: AMD)

The HBM (High Bandwidth Memory) is no longer constrained by the number of chip pins and is no longer restricted by the processor package, thereby breaking the bottleneck of IO bandwidth. Furthermore, the proximity of DRAM to the CPU/GPU physically enables further speed improvements.

"HBM also makes it possible to significantly reduce the overall system design in terms of size."

Currently, HBM2 is largely seen as a competitor to GDDR6. However, according to the latest news, both the Xbox Series X and Sony PS5 have opted for GDDR6, perhaps due to the high cost of HBM2.

However, in the long run, there is still a strong demand for 3D integration in DRAM. This is because 2D manufacturing has reached its limits, particularly with the expensive 10nm bottleneck.

Four, NVDIMM.

Nowadays, cloud computing virtual machines and various in-memory databases are prevalent, and servers are very thirsty for large capacity memory. However, due to the difficulty of further decreasing the cost of DRAM, how to configure high-capacity memory at low cost has become a problem.

The mixed NVDIMM was mentioned.

NVDIMM-F is a memory module made by replacing DRAM with NAND chips. The advantage of this is that it is extremely inexpensive, but its speed is too slow and it cannot exceed the system's access limit to DRAM's total capacity.

NVDIMM-N is a mirrored storage technology that adds NAND to DRAM on memory sticks to prevent memory data loss in case of unexpected power failure. However, NAND cannot expand memory and occupies some channel bandwidth.

The ultimate solution is NVDIMM-P, which allows for massive capacity such as 1TB of memory, and enables the use of various new chip technologies, like NAND, RRAM, and MRAM, as replacements for DRAM.

Currently, the JEDEC NVDIMM-P standard has not been released yet. However, Intel has already released Optane DIMM based on 3D-Xpoint, which is a huge advantage to support their own platform and also a major hurdle for competitors.

1. 3D-Xpoint and Other NV Memory

3D-Xpoint is a very interesting topic, claiming to be 1000 times faster than NAND in terms of speed.

Intel and Micron have always kept the technical principles of 3D-Xpoint a closely guarded secret, disclosing no details whatsoever. Initially, some speculated that it was 3D NOR technology, while later on, many believed it to be phase change memory (PCM) or RRAM.

No one has been seen to peel open the chip and analyze its internals on the market.

Until one case file revealed that contemporary Edison Stanford Ovshinsky was the inventor, the liquidating company believed that Intel and Micron had concealed crucial information during the bankruptcy proceedings following Ovshinsky's death.

After the split with Micron, Intel's 3D-Xpoint technology will be exclusively manufactured at the Dalian factory. It remains to be seen whether there will be any further insider information about the future.

The growth potential of 3D-Xpoint technology in the server field is significant, but reducing manufacturing costs is key.

MRAM, FRAM, and other NV memory types are seeking opportunities in fields such as the Internet of Things, automotive, and industrial sectors.

The process of MRAM is similar to traditional MOS semiconductor processes, which helps to expand production and reduce costs, ultimately providing an opportunity to replace some NOR, SRAM, or DRAM in certain embedded applications.

So can the faster PCM and RRAM replace NAND? It seems unlikely in the short term, because the speed requirements for storing data are generally not that high, and the low-cost, high-capacity explosion of 3D NAND has been extremely successful.

V. 3D NAND

For 3D NAND, shrinking a single cell no longer makes sense, so the most advanced semiconductor process technology is no longer needed. Hynix recently stated that 3D NAND can be stacked up to 800 layers in the future.

The process of building construction has reduced the photolithography step, while increasing significantly the processes of deposition and etching. The etching master, Lam Research, became the biggest winner.

Another impact of this is that the DRAM and NAND production lines and capacities can no longer be flexibly complementary.

Etching a staircase like this to reach a hundred levels and etching long holes is challenging. The staircase connects the bit lines, while the long holes are famous charge traps.

Remember that Infineon/Qimonda was the first to mass-produce Charge Trap flash memory using technology from Israeli company Saifun. However, at that time, the technology was not mature and the erase lifespan was only 1/10 of Floating Gate. Jim Handy stated that the process of etching holes for Charge Trap came from Trench technology.

In "The Story of Memory", it is mentioned that IBM, Infineon, Toshiba, and AMD formed an early alliance in semiconductor technology. Later, Qimonda battled alone with Trench technology and eventually lost. However, Charge Trap etching technology has continued to be used: AMD's successor Spansion applied it to NOR Flash, and Toshiba developed the leading BiCS 3D NAND.

Currently, only Intel remains committed to the Floating Gate technology. From my understanding, FG requires special itching technologies, which may make the manufacturing process more complex and may result in loss of competitiveness. Exiting the market may be unavoidable.

A few days ago, I found Jiangsu Changjiang Electronics Technology Co. Ltd's 128-layer Xtacking technology very interesting, as it separates the storage array and control circuitry. This can greatly reduce development and innovation cycles, but poses significant challenges for mass production. Specific technical details were limited, but if wafer-to-wafer bonding is used, even without considering bonding yield, the yield of the finished product is the product of the yield of two wafers.

The continuation of 3D NAND and the difficulty in establishing the DDR5 standard present a very good opportunity for the emerging Chinese memory industry to catch up.

Staying grounded while maintaining lofty aspirations is likely the key to success in the memory industry.
