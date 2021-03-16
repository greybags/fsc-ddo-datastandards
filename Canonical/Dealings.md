## Data standard for DDO – Transactions/Dealings

This data standard relates to reports by product distributors to product issuers (under the DDO regime) relating to product transactions/dealings, including dealings that are outside the target market.

### Data standard

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/ conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| | **0: Report Header (Data items common to more than one DDO data standard)** | |
| --- | --- | --- |
| | Version of standard | Version number of data standard Can be non-integer. Major versions should increment by 1. Minor changes (backwards compatible) can increment by less than 1. (eg 2.1, 2.2, 2.3) | XXX | M | |
| | Report Type | Is report Aall transactions by date range or transactions by unique identifier?.If transactions by date range, then expectation is there will only be one report for the particular date range.If transactions by unique ID, then there may be any number of reports for a date range | Single choice of: 1 = transactions by date range2 = transactions by unique identifier | M | |
| | Report unique ID | Report ID – unique to distributor. Can be combined with distributor ID to have industry-wide unique ID | Each distributor would choose their own ID | M | |
| | Is this report new or amendment? | Is this a new transaction report or a replacement to a previous report? Only use if report type is transactions by unique ID.If this is a replacement report, this should replace the previous report in full. | Y/N | M | |
| | ID of original report | If amendment, ID of original/previous report that is being amended. Only complete if previous field is Y | Same format as next itemreport unique ID | C | |
| 0.1 | Report date | Date that transaction report was made. If report is reissued, the new information replaces any reports within the defined report start and end period. | Format YYYY-MM-DD HH:MM:SS | M | |
| | Report period start | Initial date the extract report covers. Inclusive of day. Only complete if Report Type is &quot;transactions by date range&quot;. | Inclusive of the day. | MC | |
| | Report period end | Final date the extract report covers. Inclusive of day. Only complete if Report Type is &quot;transactions by date range&quot;. | Inclusive of the day. | MC | |
| | **Reporting entity – this entity may be reporting on behalf of multiple distributors. The list of distributors included in the report is included later** |
| | _Reporting entity identifier _ | refer [Entity Identifier](Common/EntityIdentifier.md) |
| | _Contact details (for this report) _ | refer [Contact Details](Common/ContactDetails.md) |
| | **2: Intermediaries / Distributors covered by this report – can be multiple subrecords – only include entities/distributors involved in transactions** |
| | _Distributor identifier _ | refer [Entity Identifier](Common/EntityIdentifier.md) |
| | **3: Reporting Dealings (Transactions)** | |
| _**If the report relates to multiple dealings, then the following rows need one subrecord for each dealing (within the main record)**_ |
| | Distributor type | The type of the distributor that was involved in the relevant dealing. This is the lowest level entity involved in distribution | Single choice of {adviser, platform, aggregator, promoter} | M | |
| | Distributor unique identifier | For adviser, FAR # of adviser.For all other types, AFSL # | FAR # or AFSL # | M | |
| 3.1 | Dealing inside TM? | Is this dealing inside the target market? | Y or N | M | Do we want an assessment of &quot;how far outside&quot; TM? |
| | Personal advice? | Is dealing an excluded dealing due to personal advice exemption? | Y/N | M | |
| | If personal advice and outside TM, outside TM reason | If dealing is outside target market, why did dealing proceed despite this? Field is mandatory if previous field is N and &quot;dealing inside TM&quot; is N. | Free text | C | |
| 3.3 | Transaction dDate of dealing | Date the dealing occurred | YYYY-MM-DD | M | |
| 3.4 | Transaction sSize of dealing | The $ value of the dealing included within the report should be sum insured for life, TPD and trauma and monthly benefit for IP. to &#39;match&#39; value of managed funds etc | ### | M if available | |
| | Number | Number of units, shares etc involved in dealing | ### | O | |
| | _Product identifier _ | refer [Product Identifier](Common/ProductIdentifier.md) |
| | _ **Following is mandatory for dealings not subject to personal advice** _ |
| | TMD version | The version of the TMD for the product that the customer was assessed against. | ### | M | |
| | TMD data standard type | The type of the TMD data standard that is used for the following fields | Select one out of {Funds management/superannuation/life insurance} | | |
| | TMD data standard version | The version of the TMD data standard that is used for the following fields | ### | M | |
| | _**TMD assessment for dealing – one subrecord for each characteristic in the TMD (refer relevant TMD data standard)**_ |
| | TMD characteristic | The ID of the TMD characteristic. | Data validation as per the relevant TMD data standard | As per TMD data standard | |
| 3.6 | TMD Value | The value of the TMD characteristic for the investor(s) the subject of the report. One value per characteristic.This must be the assessment of the customer against the TMD, not a copy of the TMD. Need to explain difference between Not assessed and Unable to be assessed. | Data validation as per the relevant TMD data standardCoding as per data standard (In target market, potentially in target market or not in target market). Add additional codes: Not assessed and Unable to be assessed | as per TMD data standard | |
| | _ **Validation Footer/Check sums** _ |
| | # dealings | Count of number of dealings included in overall record | | M | |
| | Sum of $ | Sum of $ values included in overall record under data item &quot;size of dealing&quot; | | M | |

## _Copyright &amp; Disclaimer for data standard_

_© 2021 Financial Services Council Limited ABN 82 080 744 163._

_The intellectual property rights in this document, including the copyright in the document, are owned by and retained by the FSC and its licensors. The FSC grants you a non-exclusive non-transferable licence for you and the organisation you represent (the User) to use this document internally within the User&#39;s business, including making copies, reproductions, and modifications of the document, and otherwise as expressly set out in the conditions below for so long as the User licenses this data standard._

_You and the User acknowledge and agree that the information contained in this document has been collated and prepared by the FSC for the sole purpose of assisting Users to manage their compliance with Part 7.8A of the Corporations Act 2001. The information contained in this document is based on current sources and practice as at 2021. The information contained in this document may need to be updated and revised as new sources of information emerge or practices change over time._

_Users should use their own judgment when making use of this material and should carefully evaluate its currency, completeness and relevance for their own purposes as well as the extent to which this material can or should be modified to suit the User&#39;s products._

_While steps have been taken to ensure the accuracy of the information contained in this document, the FSC does not guarantee, and accepts no legal liability whatsoever or howsoever arising from or connected to, the accuracy, currency, completeness of any material contained in this document (including any liability that may flow directly or indirectly from the modification of the information contained in this document) and makes no warranties as to suitability for you or non-infringement or for compliance with the data requirements under Part 7.8A of the Act._

![](RackMultipart20210316-4-8lfz9_html_b01c81e2b01acfb2.jpg)

© 2021 Financial Services Council Limited