<details>
<summary><h2>⚡ Programming in the Early 90s</h2></summary>
I started programming on a ZX Spectrum clone in the early 90s when I was 7 or 8.
I even remember my father helped me save some of my programs on tape. Needless to say, none of those programs survived.

_Only later did I realize that magnetic tapes and floppies are not the best medium for personal long-term storage._
</details>

<details>
<summary><h2>⚡ My First Source Control System</h2></summary>

My first source control system was slightly different from git. In the early 90s, I had that 8-bit Bulgarian computer based on a cloned Motorola MC6800 with a membrane keyboard and virtually no software.

Since it had no games, I had to create them myself. Thankfully, its firmware included a BASIC dialect with decent capabilities called UniBASIC (everything was Uni on this machine: UniBIOS, UniBASIC, UniPASCAL, UniDOS, and even UniASM, but that seemed to be all the software in existence).

And even though the machine had a floppy drive, I would type in games from memory. I distinctly remember one of my birthdays, when kids wanted to play on the computer I had in my bedroom; I was like: "just a moment", turned it on, typed in the game, and voilà! 🎮 Kids can play! Unlike the "grown-up" IBM PC in my father's office, where one had to load a game from a floppy.

That was the time I used my brain to remember the source 🤔.
</details>


<details>
<summary><h2>⚡ That time I survived a game industry crash</h2></summary>

The first big video game industry crash happened back in 1983 and didn't affect me, since I was like 1 year old. But the second recession caught me working in game development.

In the mid 2000s, I tried to develop commercial games for the web and mobile phones. My efforts ended up in several failures - I was unable to test my Java midlets on a wide range of phones, so my contract with aggregators ended in nothing. And there was no market for Java applet games whatsoever, especially for complex and deep strategy games. My lack of understanding of the market was astounding.

Eventually I ended up as a back-end architect on a huge and overly ambitious **Massively Multiplayer Online Game** project. So my efforts were not for nothing.

Meanwhile, colleagues from a job I had a couple of years prior found investors and were building a cyberpunk MMORPG.

It was a crazy time. Everyone was building an MMO game back then. After the successes of Ultima, Lineage, and WoW, these were the only types of games worth building!

Well, the 2008 crash ended the crazy investment cashflow into triple-As, and all the people around me switched to simple social games, match-3, hidden objects, and that other thing they called "slots," even though I didn't have any clue what they meant by that.

It was a depressing time. A troubling time.
Big studios were closing all around the city.

Once, after the crash, I was at a local game developers meetup.

Devastated by the crisis and declining state of the industry, gamedev professionals got really drunk and started a fierce bar fight. Needless to say, the party ended prematurely with broken furniture, shattered windows, fractured bones, and ambulances picking up _the survivors of the unfortunate game industry crash_.
</details>


<details>
<summary><h2>⚡ I used containers before it became a thing</h2></summary>

I used containers in production back in the 2000s, way before Docker was invented and containers became mainstream.

Well, they were not called containers back then. They were called _jails_ on _FreeBSD_ and _zones_ on _Solaris_. And we knew they would be good for security. Back then, we had no idea about the impending revolution in software packaging, delivery, and operations, even though we were kind of a part of it.

It was still early and hard to explain. Later, when I was looking for a job, no tech interviewer could understand what I was talking about. Containers? What containers? Such nonsense! Why would you want to do anything like that?
</details>

<details>
<summary><h2>⚡ One day I turned into a data archaeologist and migrated a database from a mainframe</h2></summary>

We were migrating a customer database with billing data to our system. The problem was that there were no specs, no documentation, no access to the running software.

The only thing we had were CSV exports of 6 or 8 tables from that mainframe. Each contained like 160 columns. And since there was a limitation on column names that allowed only 8 uppercase letters, they were all named like "DT4PAT11".

Somewhere amongst these columns were user names and sparse data on how much we had to bill each one. And I had to guess where the names were and where the money. I spent months inside SQL scripts randomly picking some columns for import/consolidation, trying to guess what should go where. Then we would run a test billing to see how much we'd missed (usually that was something like $750k).

In the end, we'd minimized the billing gap from below as much as possible, deciding that we'd rather underbill than overbill customers.

We'd finally migrated the database before the deadline. But that was the most ambiguous data project of my life!
</details>

<details>
<summary><h2>⚡ A case of missing gasoline</h2></summary>
That was early in my career.

There was that cursed central MS SQL Server instance with replication from several regional nodes.
That one time, replication was interrupted, and when we restored it and applied all logged transactions, 4 litres went missing from the gasoline consumption logs in the central DB.

That was a big problem for accounting. They knew perfectly well how to shuffle cash and make millions disappear. But the 4-litre discrepancy between a regional and central server report drove them crazy.

So I was left in the cold data center room to perform a Transact-SQL majik ritual and figure out the exact transaction that went missing.
My ceremony was successful, and I finally identified the culprit. The final transaction was replicated, and the order to Universe was restored!

_The case of missing gasoline was solved!_

</details>

<details>
<summary><h2>⚡ That time I had a technical argument with a CTO of a Fortune 500 company</h2></summary>
I always thought that CTOs of top companies have extraordinary skills, deep technical expertise, and incredible insight into the industry landscape and current trends. After all, their decisions shape the industry.

A few times I was lucky to cross paths with high-ranking tech people (like CTOs or VPs of Engineering at big companies), and I was always impressed with their wisdom and astute decision-making. It felt like they were on a totally different plane of perception, having vision into things I'm not capable to see nor comprehend.

Well, not that time. There was a deeply technical discussion about a new monitoring and profiling tool for a device we were working on. And the CTO had a very strong and established vision for how to build one. A deeply flawed vision. He suggested modifying the original UI to include the monitoring/profiling panel that will show real-time data from the ongoing test.

My education in physics kicked in, cause I knew very well that the act of measuring alone can change the result of an experiment. I heard the profiling stories where the major resource waster turned out to be the printouts used to do the profiling itself.

I spent the next half an hour dancing around the whiteboard, trying to suggest an alternate approach. I was doing my best to visualize the possible impact of telemetry processing and rendering on the box. Effects on CPU, GPU, memory bus... Effects of downscaling the original UI... In the end, our test data would be contaminated with by-products of local profiling.

I proposed minimizing the testing footprint by introducing a lightweight headless telemetry agent instead. It would collect and send test data over the network, and all the heavy post-processing, filtering, and visualization would be done on a powerful tester's workstation.

People around the table started to agree that this is a more reasonable approach, and in the end we managed to persuade the CTO to back it up.

That situation made me reflect on my years in the industry and how many times I succumbed to decisions by authorities, cause they know better. But sometimes they don't.

We're all humans after all. We all hold various misconceptions and occasionally make mistakes in our judgment. Even CTOs and VPs of Engineering.

</details>

















