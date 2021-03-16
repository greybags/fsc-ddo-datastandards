# Xml

This folder defines the technical implementation of the FSC DDO Data Standards in an Xml Representation.   
It consists of three Data Standards
 - TMD distribution
 - Dealings transactions
 - Complaints

 ## Releasing a new version
  - Create a new target branch referencing to the new version
  - increment the version numbers in the schemas
  - complete version consistency checks

## Data Standards
 - Suffix all enum types with *Enum
 - Suffix all Global Complex Types with *Type 
 - Suffix all arrays/lists with "*CollectionType"

 ***
 ## XSD Structure Overview
 ### Dealings Diagram
 ![Dealings Structure](Dealings.png)