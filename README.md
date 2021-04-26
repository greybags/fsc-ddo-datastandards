# fsc-ddo-datastandards
This Repository contains the definitions of the Australian Financial Services Council's Design And Distribution Obligations (DDO) Data Standards.
   
The DDO Data Standards are an industry response to the ASIC Regulatory Guide (RG 274) - "Product Design and Distribution Obligations".   
The intent of these standards is to provide FSC members and the wider Australian Financial Services industry 
a common definition of the information needed to satisfy the obligations, and a common, well defined format to transmit 
and disseminate the required data between associated entities.  

To assist with industry acceptance of these Data Standards, they are being released under an [open source licence](/LICENCE).

## Defined Data Standards
This repository defines three Data Standards:
 - [Target Market Determinataion (TMD)](Canonical/TargetMarketDeterminations.md)
 - [Dealings (Transactions)](Canonical/Dealings.md)
 - [Complaints](Canonical/Complaints.md)

## Repo Structure
 - The "Canonical" Folder contains the logical data definitions:
     - [Target Market Determinataion (TMD)](Canonical/TargetMarketDeterminations.md)
     - [Dealings (Transactions)](Canonical/Dealings.md)
     - [Complaints](Canonical/Complaints.md)
 - The "Implementation" Folder contains the format specific implementations of the logical data definition:
   - [XML (Comprehensive)](Implementations/Xml/README.md)
   - [CSV (TMD Only)](Implementations/CSV/README.md)
   - [JSON (Not yet started)](Implementations/JSON/README.md)

### Version control, branching and releases
To support the standards development process, this repository will define a branch per future version.   
All future standard version will be commited to this banch, until ratified, upon which they will be merged into the Main branch. 
