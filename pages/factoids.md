<details>
<summary><h2>⚡ Programming in the Early 90s</h2></summary>
I started programming on a ZX Spectrum clone in the early 90s when I was 7 or 8.
I even remember my father helped me save some of my programs on tape. Needless to say, none of those programs survived.

_Only later did I realize that magnetic tapes and floppies are not the best medium for personal long-term storage._
</details>

<details>
<summary><h2>⚡ My First Source Control System</h2></summary>

My first source control system was slightly different from git. In the early 90s, I had that 8-bit Bulgarian computer based on a cloned Motorola MC6800 with a membrane keyboard and virtually no software.

Since it had no games, I had to create them myself. Thankfully, inside its firmware was a BASIC dialect with decent abilities called UniBASIC (everything was Uni with this machine - UniBIOS, UniBASIC, UniPASCAL, UniDOS, and even UniASM, but that seemed to be all the software in existence).

And even though the machine had a floppy drive, I would type in games from memory. I distinctly remember one of my birthdays, when kids wanted to play on the computer I had in my bedroom; I was like: "just a moment", turned it on, typed in the game, and voilà! 🎮 Kids can play! Unlike the "grown-up" IBM PC in my father's office, where one had to load a game from a floppy.

That was the time I used my brain to remember the source 🤔.
</details>


<details>
<summary><h2>⚡ The time I survived in the game industry</h2></summary>

In the mid 2000s, I tried to develop commercial games for the web and mobile phones and then ended up as a back-end architect on a huge and overly ambitious **Massively Multiplayer Online Game** project.

Meanwhile, my former colleagues found investors and were building a cyberpunk MMORPG. It was a crazy time. Everyone was building an MMO game back then. After the successes of Ultima, Lineage, and WoW, these were the only types of games worth building!

Well, the 2008 crash ended the crazy investment cashflow into triple-As, and all the people around me switched to simple social games, match-3, hidden objects, and that other thing they called "slots," even though I didn't have any clue what they meant by that.

That was a depressing time. Big studios were closing all around the city.

Once, after the crash, I was at a game developers meetup.

Devastated by the crisis and declining industry, gamedev professionals got really drunk and started a fierce bar fight. Needless to say, the party ended prematurely with broken furniture, shattered windows, fractured bones, and ambulances picking up _the survivors of the unfortunate game industry crash_.
</details>


<details>
<summary><h2>⚡ I used containers before it became a thing</h2></summary>

I used containers in production back in the 2000s, way before Docker was invented and containers became mainstream.

Well, they were not called containers back then. They were called _jails_ on _FreeBSD_ and _zones_ on _Solaris_. And we knew they would be good for security. Back then, we had no idea about the impending revolution in software packaging, delivery, and operations.

It was still early and hard to explain. Later, when I was looking for a job, no tech interviewer could understand what I was talking about. Containers? What containers? Why would you want to do such a thing?
</details>

<details>
<summary><h2>⚡ I had to migrate a database from a mainfraim once</h2></summary>

We were migrating a customer database with billing data to our system. The problem was that there were no specs, no documentation, no access to the running software.

The only thing we had were CSV exports of 6 or 8 tables from that mainframe. Each contained like 160 columns. And since there was a limitation on column names that allowed only 8 uppercase letters, they were all named like "DT4PAT11".


Somewhere amongst these columns were user names and sparse data on how much we had to bill each one. And I had to guess where the names were and where the money. I spent months inside SQL scripts randomly picking some columns for import/consolidation, trying to guess what should go where. Then we would run a test billing to see how much we'd missed (usually that was something like $750k).

In the end, we'd minimized the billing gap from below as much as possible, deciding that we'd rather underbill than overbill customers.

We'd finally migrated the database before the deadline. But that was the most ambiguous data project of my life!
</details>

<details>
<summary><h2>⚡ Once I was investigating a case of missing gasoline</h2></summary>
That was early in my career.

There was that cursed central MS SQL Server instance with replication from several regional nodes.
That one time, replication was interrupted, and when we restored it and applied all logged transactions, 4 litres went missing from the gasoline consumption logs in the central DB.

That was a big problem for accounting. They knew perfectly well how to shuffle cash and make millions disappear. But the 4-litre discrepancy between a regional and central server report drove them crazy.

So I was left in the cold data center room to perform a Transact-SQL majik ritual and figure out the exact transaction that went missing.
My ceremony was successful, and I finally identified the culprit. The final transaction was replicated, and the order to Universe was restored!

_The case of missing gasoline was solved!_

</details>











