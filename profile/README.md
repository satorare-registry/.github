Welcome to SATORARE!

This Github Organaztion will be used for discussion and the repo for the storage of the SATORARE Registry entries before they are pushed onchain (Bitcoin).
Other repos for websites and tooling will also all exist here.

# What does the word SATORARE mean?

"Satorare" (悟られ) is a verb in Japanese.
"Satorare" is a term that describes a state of being understood or realized. In some contexts is is described as sudden, unpredictable moments of enlightenment or realization. In a way, discovering, creating and curating sats of value can have a similar effect.

The word itself is rarely used.

"SAT" and "RARE" seperated by the letter O (Ordinals) make this word quite apropos for this project.

# The Registry

The Satorare Registry compliments the [Ordinals](https://ordinals.com) Protocol and ecosystem. Satorare's purpose is simple. Curate and surface sats of value. While the purpose is simple, the process and depth of criteria that is used to determine sats of value is complex. This is because anything can be anchored to a sat.  

The Satorare Registry will use the Counterparty Bitcoin Asset and Message Protocol. Though not commonly used to organize information, it happens to be an ideal platform for this use case by leveraging subassets to create collections and parent-child hierachies with enough text for values to make it useful like a K/V store. All data is pushed onchain as special Counterparty protocol messages (on Bitcoin Blockchain).

Prior to the entries on Counterparty that get pushed onchain, this Github organization's repo(s) will be used to submit Ordinal sat serial numbers with additional information pertaining to why it should be included in the Satorare Registry and be considered one of the sats of value. 

Github and Counterparty should be sufficient for the process of listing sats in the registry. Details on how Github will be used for this are still under considerations but likely will simply use Issues and maybe Discussions as well. Registry snapshots will also be stored here on Github and published to satorare.org. 

The registry serves as a public utility for the new and future use case of anchoring sats to meaningful events, people, places and anything else that is determined to be well served by having an associated sat as a rich digital artifact. Of course it also will include art and any noteworthy inscriptions associated with a sat. Inscribed data can imbue value onto a sat as much as a sat can imbue value onto an inscription. 

The Satorare Registry is essentially a curated collection of interesting sats and inscriptions. Subcollections and onchain exhibits will also be created from the master collection. These subcollections would be created by a community of curators that may form. Custom curated subcollections and virtual onchain exhibits can be namespaced with custom names that adhere to a simple protocol. 

The data from the Satorare Registry is available to anyone for integration or general perusal. 

*It is on the Bitcoin Blockchain!*

# Inscriptions

The sats submitted to the Satorare Registry do not need to have an inscription associated with it.

# XSAT 

**XSAT** is a special unique Counterparty named asset. XSAT represent actual Bitcoin sats.

This will be the official registry asset and container for the directory structure.

On Counterparty, the minumum characters for named assets is 4. It is common to add an X in front of a 3 character name.

XSAT will represent sats (satoshis) added to the registry by simply creating subassets named using the sat serial number as per Ordinal Theory. 

Examples:

- `XSAT.0`
- `XSAT.1311797500000000`

Each XSAT Subasset will include metadata and chain info related to that Ordinal sat.

# SAT.SN

A short URL for sats that only include the sat serial number (sn) or sat name (sn).
These pages will show all info about the sat as well as tracking the sat as it traverses through the network.
If there is an inscription, the data will be displayed.
If there is available market activity (buys/sells), that info will be included.
User contributed content, blockchain data, known associations such as world events etc are all available on sat pages.

sat serial number format:
- `sat.sn/0`
- `sat.sn/1311797500000000`

sat name format:
- `<name>.sat.sn --> sat.sn/<serial_number>`
- `sat.sn/<name>`

# SATURN

A Uniform Resource Name for sat serial numbers.

see https://en.wikipedia.org/wiki/Uniform_Resource_Name

- `urn:sat:ord:1926444375000000`

**Examples with URL resolver parameter:**

- `urn:sat:ord:1926444375000000?=url=http://saturn.sn/`

- `urn:sat:ord:1926444375000000?=url=http://sat.sn/`

- `urn:sat:ord:1926444375000000?=url=http://ord.io/sat/`

**HTTP URI Examples:**

- `http://saturn.sn/ord/1926444375000000`

- `http://saturn.sn/ord?sn=1926444375000000`

- `http://sat.sn/1926444375000000`

- `http://sat.sn/ord?sn=1926444375000000`

*With fragment specifying associated inscription data to be handled as primary content on resolved document:*

- `http://saturn.sn/ord/1926444375000000#inscription`

^^ not currently resolvable, no dereference.

No current plan to register with IANA. 

# SAT DIDs

TBD

[www.w3.org/TR/did-core/](https://www.w3.org/TR/did-core/)

# Registry Submissions

TBD

# Token Config (XSAT, SATORARE etc)

XSAT subasset tokens will likely all be 0 or 1 supply (non-divisible) and locked.

Collections using subassets under SATORARE may be more flexible with a variety of token issuance settings.
Collection owners (curators) may choose to sell tokens to receive donations for the curatorial work involved and the resulting onchain exhibit which can be considered a form of art itself.
In cases where the curator(s) want to tokenize their collections/exhibits, the asset ownership will be transferred to them. 

Collections using assets other than SATORARE as parent can of course do whatever they want. 

# Subcollections and Exhibits

While all entries in the Satorare Registry are stored as an XSAT subasset named with sat serial numbers, curated subcollections/exhibits can use any Counterparty asset owned by anyone as the organizing parent in a hierarchical structure. Official subcollections/exhibits created by the Satorare curation team will exist under the **SATORARE** Counterparty Asset.

- `SATORARE.<SUBCOLLECTION_NAME><XSAT_SERIAL_NUMBER>`

Associated metadata in each subcollection will include all information about the curated subcollection such as curation criteria, curator(s) statement and list of curator idenitifiers (if desired to be referenced).

All entries in a subcollection/exhibit simply reference the sat serial numbers that are included under XSAT as subassets. There is also an asset ID (numeric) that exists. Any sat serial numbers not in the registry do not qualify to be included in subcollections/exhibits. This applies to any external subcollection as well. If there are discrepencies, the external subcollection will not be considered as part of Satorare but rather a seperate **rogue** collection, which is fine. It is encouraged to create curated Ordinal sats and inscriptions using Counterparty in the way that Satorare does. These collections may be referenced by Satorare as noteworthy and high quality exhibit. The sats that are included in external collections but not in Satorare could be discovered and added and vise versa. No competition. Just curation protocols.

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

# Future

## Satori Wallet

While the Satorare Registry is up and running (managed by team and used by community) there will be an ongoing development project to build a new Wallet and Marketplace that leverages the Satorare Registry data. It is hoped that other wallets, tools and services will also integrate the Satorare Registry.

It is an ambition to also incorporate smart sat handling within the wallet software. This is related to sat hunting (panning) and sat sorting, which is meant to avoid spending sats of value without intent and to get insights into the sats that you own. 

The Wallet will be called Satori and more info will be published to http://satoriwallet.xyz.

> Satori refers to a sudden, intuitive understanding or insight into the nature of reality or the true nature of oneself. It is often described as a moment of enlightenment or awakening, in which one transcends the limitations of the ego and experiences a sense of oneness with the universe. Satori is considered to be a profound and transformative experience, and is often sought after by Zen practitioners through meditation and other spiritual practices.

## Ordinals Envelopes as Counterparty Address Type

Proposed by Joe Looney here:

[forums.counterparty.io/t/ordinal-envelopes/6504](https://forums.counterparty.io/t/ordinal-envelopes/6504)

XSAT could possibly be a relevant asset tree for this model.

## HALPAL

**H**yper**A**ddress **L**ocation **P**rotocol for **A**ttributes and **L**abels

A seperate parallel protocol to Ordinals. 

**XHAL**

Also involves it's own registry on Counterparty using the **XHAL** asset tree.

May have some overlap with above **Ordinals Envelopes** concept. May leverage Counterparty Dispenser tech.

[halpal.org](https://halpal.org) / halpal.io

## HALPAL STAMPS

These two STAMP NFTs may be used as an acceptable currency for the Satorare and HALPAL projects.
Each has 10 divisible tokens.

See this twitter thread:
[twitter.com/sull/status/1643684675376881697](https://twitter.com/sull/status/1643684675376881697)

<img width="403" alt="Screenshot 2023-04-06 at 12 51 51 PM" src="https://user-images.githubusercontent.com/78568138/234727580-781be8aa-5405-464e-a15f-1ea2fb69704a.png"> <img width="402" alt="Screenshot 2023-04-06 at 12 52 11 PM" src="https://user-images.githubusercontent.com/78568138/234727581-c4424211-f59c-4b3c-8277-e918df87326a.png">


## Satorare DAO

lol  ¯\_(ツ)_/¯  

