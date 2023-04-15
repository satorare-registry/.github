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

The registry serves as a public utility for the new and future use case of anchoring sats to meaningful events, people, places and anything else that is determined to be well served by having an associated sat as a rich digital artifact. Of course it also will include art and any noteworthy inscriptions associated with a sat. Inscribed data can imbue value onto a sat as much as a sat can imbue value onto an inscription. 

The Satorare Registry is essentially a curated collection of interestings sats and inscriptions. Subcollections and onchain exhibits will also be created from the master collection. These subcollections would be created by a community of curators that may form. Custom curated subcollections and virtual onchain exhibits can be namespaced with custom names that adhere to a simple protocol. 

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

- `sat.sn/0`
- `sat.sn/1311797500000000`

# Registry Submissions

TBD

# Token Config (XSAT, SATORARE etc)

TBD

# Subcollections and Exhibits

While all entries in the Satorare Registry are stored as an XSAT subasset named with sat serial numbers, curated subcollections/exhibits can use any Counterparty asset owned by anyone as the organizing parent in a hierarchical structure. Official subcollections/exhibits created by the Satorare curation team will exist under the **SATORARE** Counterparty Asset.

- `SATORARE.<SUBCOLLECTION_NAME>`

Associated metadata in each subcollection will include all information about the curated subcollection such as curation criteria, curator(s) statement and list of curator idenitifiers (if desired to be referenced).

- `SATORARE.<SUBCOLLECTION_NAME>.<XSAT_SERIAL_NUMBER>`

All entries in a subcollection/exhibit simply reference the sat serial numbers that are included under XSAT as subassets. Any sat serial numbers not in the registry do not qualify to be included in subcollections/exhibits. This applies to any external subcollection as well. If there is discrepencies, the external subcollection will not be considered as part of Satorare but rather a seperate rogue collection, which is fine. It is encouraged to create curated Ordinal sats and inscriptions using Counterparty in the way that Satorare does. If these collections are referenced as curated curated collections, it will just be noted that it is not a strictly Satorare Protocol conforming collection. 

There may be cases where there are more complex organizing structures for subcollections. One example could be to support curator groups within groups or individual curators with their own curated subcollections but still associated with a larger group the individual is a part of.

- `SATORARE.<SUBCOLLECTION_NAME>.<CURATOR_NAME>.<SUBCOLLECTION_NAME>.<XSAT_SERIAL_NUMBER>`
- `<EXTERNAL_ASSET_NAME>.<SUBCOLLECTION_NAME>.<CURATOR_NAME>.<SUBCOLLECTION_NAME>.<XSAT_SERIAL_NUMBER>`

Satorare is both exclusive and inclusive. Curation is the top-level motivation and that runs down into all subsets of data and people.

# STAMPS

STAMPS is a recent addition to onchain Bitcoin data storage via Counterparty. 
It caters mostly to 8-bit art with a 24x24 dimension and very small filesize.
SVG is also popular. 
Compared to Inscriptions, STAMPS is more expensive but the data onchain is **stickier** (less prunable).

See https://stampchain.io and https://tokenstamps.io.

STAMPS is a simple protocol that looks like this:

`STAMP:<base64>`

STAMPS Protocol will be used within Satorare Registry to store metadata (with or without an image file).

The metadata standard that Satorare will use is TBD. 




