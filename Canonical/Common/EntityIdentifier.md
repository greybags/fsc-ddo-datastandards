**Reporting entity identifier**

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/ conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| | Reporting Entity Name | The name of the entity providing the report to the Issuer. May or may not be a product distributor. Not for machine analysis | Free text | ? | |
| --- | --- | --- | --- | --- | --- |
| | Reporting Entity Type | Identifies the type of the entity providing the report to the Issuer | Single choice of {Adviser / Advice AFSL / non-advice AFSL / credit licensee / Other} | M | |
| | Reporting Entity FAR | Financial Advice Register number of reporting entity. Must be used if reporting entity holds a FAR number. | FAR # | M if available/applicable | |
| | Reporting Entity ACL | Australian Credit License (ACL) number of reporting entity. Must be used if reporting entity holds an ACL | | M if available | |
| | Reporting Entity AFSL | Reporting entity AFSL. Must be used if reporting entity holds and AFSL | | M if available | |
| | Reporting Entity ABN | Reporting entity ABN. Must be used if reporting entity holds an ABN | | M if available | |

**Distributor identifier**

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/ conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| | Distributor Type | Identifies the type of distributor included in this subrecord | Single choice of { Advice AFSL / Platform / non-advice AFSL/ACL} | M | |
| --- | --- | --- | --- | --- | --- |
| | **If distributor is advice AFSL:** || | AFSL | AFSL of distributor included in subrecord Must be included | AFSL # | M | |
| | ABN | ABN of distributor included in subrecord Must be included | ABN # | M | |
| | Business Name | Not for machine analysis | Free text | M | |
| | _Contact details (for advice AFSL) � refer standard data items_ |
| | _For each business under above AFSL: (for transactions report, only include businesses involved in transaction)_ |
| | ABN | | | M | |
| | Business Name | Free text. Not for machine analysis | | M | |
| | _For each adviser under each business: (for transactions report, only include advisers involved in transaction)_ |
| | FAR | | | M | |
| | _Contact details (for adviser) � refer standard data items �_ _do we need to include for every adviser?_ |
| | **If distributor is non-Advice AFSL (fund managers, platforms, online stockbrokers, insurance aggregators, mortgage brokers)** |
| | ACL | Australian Credit License (ACL) number of entity included in this subrecord. Must be used if entity holds an ACL | | M if available | |
| | AFSL | AFSL of distributor included in subrecord Must be included | | M | |
| | ABN | ABN of distributor included in subrecord Must be included | | M | |
| | Business Name | Not for machine analysis | | M | |
| | _Contact details (for non-advice AFSL) � refer standard data items_ |
| | _For each promoter under non-advice AFSL (for transactions report, only include promoters involved in transaction)_ |
| | AFSL | | | M | |
| | ABN | | | M | |
| | Business Name | | | M | |
| | _Contact details (for promoter) � refer standard data items_ |



## _Copyright &amp; Disclaimer for data standard_

_� 2021 Financial Services Council Limited ABN 82 080 744 163._

_The intellectual property rights in this document, including the copyright in the document, are owned by and retained by the FSC and its licensors. The FSC grants you a non-exclusive non-transferable licence for you and the organisation you represent (the User) to use this document internally within the User&#39;s business, including making copies, reproductions, and modifications of the document, and otherwise as expressly set out in the conditions below for so long as the User licenses this data standard._

_You and the User acknowledge and agree that the information contained in this document has been collated and prepared by the FSC for the sole purpose of assisting Users to manage their compliance with Part 7.8A of the Corporations Act 2001. The information contained in this document is based on current sources and practice as at 2021. The information contained in this document may need to be updated and revised as new sources of information emerge or practices change over time._

_Users should use their own judgment when making use of this material and should carefully evaluate its currency, completeness and relevance for their own purposes as well as the extent to which this material can or should be modified to suit the User&#39;s products._

_While steps have been taken to ensure the accuracy of the information contained in this document, the FSC does not guarantee, and accepts no legal liability whatsoever or howsoever arising from or connected to, the accuracy, currency, completeness of any material contained in this document (including any liability that may flow directly or indirectly from the modification of the information contained in this document) and makes no warranties as to suitability for you or non-infringement or for compliance with the data requirements under Part 7.8A of the Act._

![](RackMultipart20210316-4-8lfz9_html_b01c81e2b01acfb2.jpg)

� 2021 Financial Services Council Limited