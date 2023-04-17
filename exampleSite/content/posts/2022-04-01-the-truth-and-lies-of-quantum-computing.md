---
title: "The Truth and Lies of Quantum Computing"
date: "2022-04-01"
categories: 
  - "semiconductor"
  - "software"
  - "start-a-business"
tags: 
  - "cim"
  - "coherent-ising-machine"
  - "d-wave"
  - "google"
  - "honeywell"
  - "ibm"
  - "photons"
  - "psiquantum"
  - "quantum"
  - "quantum-computing"
  - "xanadu"
---

### Epilogue

The protagonist, Professor Robert Langdon (played by Tom Hanks), in "The Da Vinci Code" and "Angels and Demons" is the central character in Dan Brown's series of books. The latest book in this series is called "Origin".

At the beginning of "Origin," billionaire Edmond announces his scientific discovery that will cause the collapse of three major religions. The protagonist, who works with Professor Langdon in the book, is a quantum computer named E-Wave.

In this book, there are embedded advertisements for Tesla Motors. And E-Wave is most likely an advertisement for the Canadian company D-Wave.

In 2011, D-Wave became the first company to offer commercial quantum computers in the world. To this day, D-Wave remains at the forefront of practical quantum computing.

### 1\. Research investment/ funding.

Quantum is probably the Achilles' heel of boasting in the scientific research community. But what's even more miraculous is that sometimes it's hard to tell if they are bragging or lying.

Various media outlets enjoy reporting on who is the hegemon and who surpasses the hegemon. The quantum xxx of certain groups can solve problems that traditional computers would take billions of years to calculate, and the internet is in imminent danger.

However, I feel that many journalists do not know what they are talking about.

Perhaps, obtaining funding is the key factor.

The question of whether research and development funds come from the government or private companies is an intriguing matter.

According to Quantum Insider/Photonics Box statistics, China's financial allocation for quantum technology (100 billion yuan) is nearly equal to the total sum of other countries in the world. However, the number of Chinese quantum technology companies is only 15 (excluding BATH), which is less than 5% of Europe and America's total.

Excluding government contributions, the chart below depicts the distribution of private company investments in quantum technology as seen in the journal "Nature". Although the data is slightly outdated, it indicates that there is still a significant difference between foreign and domestic investment.

![图片](../images/image73.jpeg)

### 2\. Classification of Quantum Technology

The application of quantum technology can be broadly categorized into two main types: quantum computing and non-quantum computing. I believe that this classification is sound and accurate, and you would not be able to find any faults with it.

Western companies tend to focus their research and development efforts on quantum computing, while China and East Asia prefer quantum communication.

Quantum communication is too amazing, and I don't understand it, but that's not the focus of this article. Anyway, they say it is very useful, and the effect is estimated to be at least comparable to Lianhuaqingwen.

![图片](../images/image74.png)

"Nature" Journal: China's quantum patents are concentrated in quantum communication (yellow) and other areas (blue), not so much in quantum computing (deep orange).

Regarding research on quantum computing, although it is extremely complex, it can still be simplified into two categories: hardware and software.

Translation: Among them, the hardware requires many experimental physicists and cutting-edge engineers, as well as many very expensive advanced instruments, with a very high threshold.

The software for quantum computing is very, very different. It requires excellent mathematicians and mediocre programmers. This is because the ideas and algorithms in quantum computing are key, and the traditional methods used in classical computing are largely obsolete.

Next, we will proceed to delve into a few technical aspects.

### Three, quantum algorithms.

The algorithm used for breaking internet public key encryption (RSA or ECC) by factoring large numbers is known as the Shor algorithm. It was originally published by Mr. Shor, but even after nearly 30 years, machines still can't effectively run it.

Currently, research on quantum software is vastly ahead of hardware, and most researchers can only experiment on simulators.

Due to the potential risks posed by quantum algorithms to current asymmetric encryption, the industry has been researching Post-Quantum Cryptography, encryption algorithms that are considered difficult to crack by quantum computers, in recent years.

After two rounds of selection, the US National Institute of Standards and Technology (NIST) has chosen seven main algorithms and eight candidate algorithms, including NTRU. It is said that the winning algorithm will be announced this year. Gossip has it that in the second round, various algorithms such as "Three Bears" and "Tesla" were eliminated, and "Sphincter" made it to the third round.

According to NIST, symmetric algorithms such as AES do not need to consider being broken by quantum computing. The Grover algorithm, which is popularized in science education, actually poses little threat.

### Four, Superconducting Quantum.

So, what kind of machine can run the Shor algorithm?

There are many paths to achieving quantum computing, but currently the most advanced approaches for general-purpose computing involve superconducting and ion trap technologies.

Quantum entanglement is too easily disturbed by external factors. Even in the vicinity of absolute zero where all things are motionless, the survival time of a superconducting qubit is only on the order of microseconds (a few millionths of a second). Any computation in the presence of noise can result in errors, and scientists often need to use five qubits to correct for one, leaving fewer precious qubits available for other purposes.

According to IBM's roadmap, the number of qubits doubles each year. In another 10 years, we will reach a million qubits that can perform Shor's algorithm. This is the legendary quantum Moore's Law.

![图片](../images/image75.jpeg)

Superconducting loop images are like works of art (Credit: IBM)

"A refrigerator with 100 qubits is as big as a room. How big of a refrigerator is needed for 1 million qubits?" - A fool asked.

The expert chuckled and said, "Do you know how big semiconductors were initially?"

### 5\. Ion traps and angel particles.

There are two major bottlenecks in the implementation of universal quantum computing technology, one is the stability issue which was mentioned earlier (noise and error correction), and the other is scalability (from 100 qubits to 1 million).

To tackle these two major obstacles, ion trapping is another pathway attempted. Honeywell and IonQ are the leaders in ion trapping.

The technology of ion trap is not new, many atomic clocks use this technology, and its quantum stability is much better than superconductivity. Another small advantage of ion trap is that the working temperature can be slightly higher than superconductivity, which can save a lot of money.

Ion trapping is a fascinating experiment where laser is used to ionize ytterbium atoms (Yb) by knocking off their electrons to create ions (don't ask me how it's done :-). These positively charged ions are then trapped in a 3D space using an array of electric potentials, known as a "trap".

![图片](../images/image75.jpeg)

The style of the ionized hydrazine machine is very robust. Credit: Honeywell.

Ions trapped in the same area are easily correlated, with very high fidelity, but the downside is that their computational speed is much slower than that of superconductors, and requires a super-vacuum environment. The measurement of their quantum state also depends on extremely precise resonant laser pulses.

Overall, ionized hydrazine is by no means a cost-saving option. The engineering difficulty is extremely high, and it is not something that small companies can afford to handle.

In the field of universal quantum computing, Intel's silicon-based quantum and Microsoft's "topological particle" technologies seem to be progressing slower and may still belong to the next generation of technology.

Topological particles are called Majorana fermions. Using them as quantum bits can sustain for 100 seconds with extremely strong resistance to interference. The fidelity is four nines higher than that of superconducting qubits, making it nearly perfect like an angel.

Unfortunately, these angel particles have been playing hide and seek with humans all along.

### Sixth, the genius D-Wave.

So, what exactly is D-Wave that we mentioned in the introduction? And why were they able to sell their products over 10 years before other companies?

Because D-Wave does not make a universal quantum computer: it cannot perform the Shor algorithm, so it cannot be used to break encryption.

However, the idea of D-Wave absolutely comes from genius, and explaining its principles in a short article poses great challenges.

D-Wave has completely abandoned the idea of using quantum bits to construct operation gates, as well as the use of strange quantum entanglement. It believes that nature and the laws of the universe are smarter than anyone.

The laws of physics automatically seek the state of minimum energy: water flows from snow-capped mountains to the sea, and hot things will always cool down.

D-Wave decomposes problems into constants and variables which are assigned to quantum bits, and then the quantum bits automatically find the optimal solution and display it through natural superposition because the optimal solution is to reach the state with the lowest energy as quickly as possible.

After all, the universe itself operates completely according to the laws of quantum mechanics.

In "Origin", E-Wave tells us that the universe likes to see humans destroy each other through hatred and war, in order to consume energy faster.

### 6\. Unorthodox Methods or Secret Techniques

The idea of D-Wave is too mystical, so the Wudang and Shaolin in the quantum community consider it to be an unorthodox method: D-Wave doesn't contain any quantum circuits with various gates, and is not even a quantum computer.

However, in scenarios with numerous variables where selecting the optimal solution is crucial, D-Wave has demonstrated overwhelming superiority over classical computers, and has successfully developed a software and algorithm ecosystem revolving around its own machine.

Just to mention, the popular science explanations about quantum on the internet are a heavily misleading area. Quantum computing itself is not the large-scale parallel computing that they claim it to be. In fact, quantum bits cannot appear in multiple states simultaneously, nor can they store multiple states. Its state should be understood as a probability, and the probabilities of different states of multiple quantum bits can be superimposed.

Take a look at Schrödinger's equation. The superpositions are the superposition of waves, and the final probability is one result, not n results. For example, whether your community will be sealed off tomorrow is a probability (wave) that is highly variable: a few days ago, an infected person who was uncomfortable with their throat from a neighboring community wanted to eat radishes in oden and happened to meet your neighbor who was starving after working 996 hours in a convenience store. And your community happened to encounter a nucleic acid test.

The wave amplitudes of different variables are different. Using the example above, the variable of the city leaders has the largest amplitude, and can instantly offset countless small waves. When they decided to lock down the city, the probability of your community being locked down tomorrow suddenly approached 100%.

Quantum bits can represent countless states and are not just combinations of 0s and 1s, as popular science suggests. Each wave function has a unique amplitude, with probabilities ranging from 21.526253% to 0.000312% (for example). As a result, quantum bits can better simulate our world, and the solution can be achieved more quickly using algorithms that are better suited for quantum mechanics (wave interference).

Now do you understand the meaning of Wave? D-Wave's machine is called a "quantum annealer".

Although the algorithms available for D-Wave are very limited, the industry has gradually begun to try using it to solve specific industrial problems, such as supply chain logistics path selection, stock portfolio selection, and material or drug molecule composition selection, which are the key points that each company promotes in quantum computing.

### 7\. Photons.

The success of D-Wave to some extent has inspired similar conceptual machines, of which the most famous representative is the "Coherent Ising Machine" (CIM). The CIM is somewhat like a neural network made of light, coupling photons through light pulses and calculating the results of its coherent degradation using FPGA.

Photons are a perfect quantum entity that exhibit stability at room temperature and have numerous mature optical devices available for functions such as polarization modulation, superposition, and measurement.

In the past two years, photons as a candidate solution for quantum computing have suddenly accelerated. Many companies have received venture capital, including PsiQuantum in California and Xanadu in Toronto. China has also seen the emergence of several photon quantum companies.

It seems that quantum computing using light is well-suited to be a track for small startups, as there are no steps requiring massive investments such as ultra-low temperatures or ultra-short survival times, and the production of light semiconductor devices is relatively mature.

However, due to the low threshold for using quantum computing, various institutions often exaggerate their progress: some only perform simple "sampling" and "measurement", while others intentionally do not specify whether they are working on CIM or general quantum computing, which causes great confusion for outsiders.

Some even directly call optical experiments quantum experiments, and this kind of promotion is as deceptive as quantum weight loss. There is no legal or physical fault to be found in this.

PsiQuantum and Xanadu both claim to achieve a machine with one million qubits within five years. If they are both universal quantum computers, IBM and Honeywell will be crying.

I did not say they were lying; the PPT and papers on these light quantum topics do seem quite plausible. However, engineering implementation is not pure science, and there is currently no good way to determine which boasts may ultimately come true.

### 8\. Which is the most powerful?

Several major companies have introduced the concept of quantum volume to measure the computing power of quantum computers, but this is only an immature and simplistic weighted scoring system that cannot fairly evaluate the different architectures of various machines.

Almost all companies or institutions exaggerate their achievements, but it is difficult to find details. The majority of machines do not allow you to tinker with them and many of the quantum computers hidden behind various clouds are just simulators.

Perhaps in the distant future, there will be third-party evaluations like Awesome Wang, which will test the speed of each quantum computer running every algorithm.

At present, no one can afford to make unboxing videos, so it is estimated that they are mostly small advertorials sponsored by manufacturers.

However, all manufacturers acknowledge that quantum computing will never replace traditional silicon-based computers, but will only be used for specific purposes in areas where quantum algorithms have absolute supremacy.

There seems to be very few instances where the quantum community reveals each other's shortcomings, as quantum computing is still a research field with very few participants. Even highly respected individuals try to save face and work together to expand the field for the benefit of the community.

Everyone is saying:

The era of silicon-based Moore's Law has come to an end, coincidentally coinciding with the rise of quantum computing.
