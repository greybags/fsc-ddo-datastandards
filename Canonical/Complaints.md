## Data Standard for DDO – Complaints

This data standard allows product distributors to provide reports required under the DDO regime to product issuers relating to the complaints received by product distributors.

### Data Standard

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/ conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| 0.1 | Version of standard | Version number of data standard. Can be non-integer. Major versions should increment by 1. Minor changes (backwards compatible) can increment by less than 1. (eg 2.1, 2.2, 2.3) | XXX | M | |
| --- | --- | --- | --- | --- | --- |
| **0: Report header (Data items common to more than one DDO data standard)** |
| | Report unique ID | Report ID – unique to distributor. Can be combined with distributor ID to have industry-wide unique ID. | Each distributor would choose their own ID | O | |
| | Report date | Date that complaints report was sent. If reissued, the new information replaces any reports within the defined report start and end period. | Format YYYY-MM-DD HH:MM:SS | M | |
| | Report Period Start | Period for which the report starts. Inclusive of day. | YYYY-MM-DD | M | |
| | Report Period End | Period for which the report ends. Inclusive of day. | YYYY-MM-DD | M | |
| **1: Reporting entity (same for all report types) – this entity may be reporting on behalf of multiple distributors. The list of distributors included in the report is included later** |
| | _Reporting entity identifier – refer common data items_ |
| | _Contact details (for this report) – refer common data items_ |
| **2: Distribution entities covered by this report (same for all report types) (expect to see multiple subrecords in this section.-can have multiple subrecords.** |
| | _Distributor identifier – refer common data items_ |
| | List of product IDs | | | | |
| **3: Issuer pProducts covered by this report (same for all report types) – can have multiple subrecords** |
| | _Product identifier – see common data items_ |
| **4: Complaints summary** |
| **For further consideration: what matrix of distributors/products/complaints do we use?** |
| **Complaint details (1 subrecord per complaint)** |
| | Ccomplaint ID | Reporting entity internal code for complaint.Could be used in conjunction with reporting entity ABN/code to create industry wide unique code if needed.If amending a previous complaint, use the previous complaint ID and this record will replace the previous complaint record. | Must be unique within reporting entity. | M? | |
| | _ **Primary product involved in complaint** _ |
| | _Product identifier – refer common data items_ |
| | _**Other products involved in complaint (eg where primary complaint is about a managed fund on a platform, the primary complaint it about the managed fund but the name of the platform should be included below). Can have multiple subrecords**_ |
| | _Product identifier – refer common data items_ |
| | _ **Distributor involved in complaint** _ |
| | Distributor FAR (as above) | Financial Advice Register number of distributor involved in complaint. Must be used if distributor holds a FAR number. | Leave blank if no adviser | M if available | |
| | Distributor ACL | Australian Credit License (ACL) number of distributor involved in complaint. Must be used if reporting entity holds an ACL | | M if available | |
| | Distributor AFSL (as above) | AFSL of distributor involved in complaint. Must be used if reporting entity holds and AFSL | | M if available | |
| | Distributor Product ID (as above) | | Leave blank if no product | | |
| | _ **Details of complaint** _ |
| | Complaint type | See RG 271 | | M | See ASIC CP |
| | Is complaint about product (issuer)? | | Y/N | M? | |
| | Is complaint about distribution/sales (distributor)? | | Y/N | M? | |
| | Financial impact? | Was the complainant impacted financially by the issue that they are complaining about? | Y/N | O? | |
| | Complaint date | | YYYY-MM-DD | M | |
| | Date of complaint resolution | Leave blank if not resolved or unknown | YYYY-MM-DD | M | |
| | Complaint content | This should include all the relevant details so that the issuer can understand the nature of the complaint | Free text | M? | Need to set a length limit on text |
| | AFCA referral? | Has complaint been referred to AFCA? | Y/N | M | |
| | AFCA referral date | Date of referral to AFCA. Only complete if previous is Y | YYYY-MM-DD | C | |
| | AFCA ID | AFCA ID of complaint. Only complete if &quot;AFCA referral?&quot; is Y | | O | |
| | _ **Validation Footer/Check sums** _ |
| | Number nil reports | Number of nil complaint records included in this file. Sum of this field and next field must equal number of complaint records in this file | | M | |
| | Number non-nil reports | Number of non-nil complaint records included in this file. | | M | |


## _Copyright &amp; Disclaimer for data standard_

_© 2021 Financial Services Council Limited ABN 82 080 744 163._

_The intellectual property rights in this document, including the copyright in the document, are owned by and retained by the FSC and its licensors. The FSC grants you a non-exclusive non-transferable licence for you and the organisation you represent (the User) to use this document internally within the User&#39;s business, including making copies, reproductions, and modifications of the document, and otherwise as expressly set out in the conditions below for so long as the User licenses this data standard._

_You and the User acknowledge and agree that the information contained in this document has been collated and prepared by the FSC for the sole purpose of assisting Users to manage their compliance with Part 7.8A of the Corporations Act 2001. The information contained in this document is based on current sources and practice as at 2021. The information contained in this document may need to be updated and revised as new sources of information emerge or practices change over time._

_Users should use their own judgment when making use of this material and should carefully evaluate its currency, completeness and relevance for their own purposes as well as the extent to which this material can or should be modified to suit the User&#39;s products._

_While steps have been taken to ensure the accuracy of the information contained in this document, the FSC does not guarantee, and accepts no legal liability whatsoever or howsoever arising from or connected to, the accuracy, currency, completeness of any material contained in this document (including any liability that may flow directly or indirectly from the modification of the information contained in this document) and makes no warranties as to suitability for you or non-infringement or for compliance with the data requirements under Part 7.8A of the Act._

![](RackMultipart20210316-4-8lfz9_html_b01c81e2b01acfb2.jpg)

© 2021 Financial Services Council Limited