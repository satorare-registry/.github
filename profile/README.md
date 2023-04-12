Welcome to SATORARE!

This Github Organaztion will be used for discussion and the repo for the storage of the SATORARE Registry entries before they are pushed onchain (Bitcoin).
Other repos for websites and tooling will also all exist here.

# What does the word SATORARE mean?

"Satorare" (悟られ) is a verb in Japanese.
"Satorare" is a term that describes a state of being understood or realized.
The word itself is rarely used.
The original name for this project was *Satori* but it seems it is being used by a few other projects in crypto space.

Since both "sat" and "rare" are in this word, it is quite apropos for this project.

# The Registry

The Satorare Registry will use the Counterparty Bitcoin Asset and Message Protocol. Though not commonly used to organize information, it happens to be an ideal platform for this use case by leveraging subassets to create collections and parent-child hierachies with enough text for values to make it useful like a K/V store. All data is pushed onchain as special Counterparty protocol messages (on Bitcoin Blockchain).

Prior to the entries on Counterparty that get pushed onchain, this Github organization's repo(s) will be used to submit Ordinal sat serial numbers with additional information pertaining to why it should be included in the Satorare Registry and be considered pne of the sats of value. 

Github and Counterparty should be sufficient for the process of listing sats in the registry. Details on how Github will be used for this are still under considerations but likely will simply use Issues and maybe Discussions as well. Registry snapshots will also be stored here on Github and published to satorare.org. 

# XSAT 

There is a special unique Counterparty named asset - XSAT 
This will be the official registry asset and container for the *directory structure*.

On Counterparty, the minumum characters for named assets is 4. It is common to add an X in front of a 3 character name.

XSAT will represent sats (satoshis) added to the registry by simply creating subassets named using the sat serial number as per Ordinal Theory. 

Examples:

- `XSAT.0`
- `XSAT.1311797500000000`

etc.

Each XSAT Subasset will include metadata and chain info related to that Ordinal sat.
Eventually, a market can form around this database where trustless PSBT trades can be done.
It will also evolve into a hybrid wiki/markketplace/wallet. 

The data from the Satorare Registry is available to anyone for integration or general perusal. 
It is on the Bitcoin Blockchain! 

# Inscriptions

The sats submitted to the Satorare Registry do not need to have an inscription associated with it.

# SAT.SN

A short URL for sats that only include the sat serial number (sn).
These pages will show all info about the sat as well as tracking the sat as it traverses through the network.
If there is an inscription, the data will be displayed.
If there is available market activity (buys/sells) that info will be included.
User contributed content, blockchain data, known associations such as world events etc are all available on sat pages.

- sat.sn/1311797500000000

# Registry Submissions

TBD

# Token Config

TBD





