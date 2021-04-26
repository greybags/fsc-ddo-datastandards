# Canonical Data Standard

This folder will contain the documentation of the logical/canonical data standards.      

The Canonical form of the Data Standards is agnostic to the "language" used to
represent the data.

There are three data standards:
 - [Complaints Data Standard](Complaints.md)
 - [Dealings Data Standard](Dealings.md)
 - [Target Market Determinations Data Standard](TargetMarketDeterminations.md)

To improve the quality of the Data Standards, some common data items 
have been identified and separated for reuse.
These are:
 - [Contact Details](Common/ContactDetails.md)
 - [Entity Identifiers](Common/EntityIdentifier.md)
 - [Product Identifier](Common/ProductIdentifier.md) 

The Logical/canonical data standards are required to be implemented 
in a representational format.   

The current supported implementations are:
 ### XML (Complete)
- Target Market Determinations
    - [Target Market Determination Schema Documentation](https://financialservicescouncilau.github.io/fsc-ddo-datastandards/xml/TargetMarketDeterminations.html)
    - [Schema Definition](/Implementations/Xml/TargetMarketDeterminations.xsd)
- Complaints
    - [Complaints Schema Documentation](https://financialservicescouncilau.github.io/fsc-ddo-datastandards/xml/Complaints.html)
    - [Complaints Schema Definition](/Implementations/Xml/Complaints.xsd)
- Dealings
    - [Dealings Schema Documentation](https://financialservicescouncilau.github.io/fsc-ddo-datastandards/xml/Dealings.html)
    - [Dealings Schema Definition](/Implementations/Xml/Dealings.xsd)
- Common Data Items (Shared by all Data Standards)
    - [Common Schema Documentation](https://financialservicescouncilau.github.io/fsc-ddo-datastandards/xml/Common.html)
    - [Common Schema Definition](/Implementations/Xml/Common.xsd)
 ### CSV (Target Market Determinations only)
- Target Market Determinations
    - [Target Market Determination CSV Documentation](/ImplementationsCSV/TargetMarketDeterminations.md)
 


