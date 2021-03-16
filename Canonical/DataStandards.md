# FSC Data Standards for DDO

This document provides assistance in relation to the data required to implement the Design and Distribution Obligations (DDO) under the _Corporations Act 2001_ (Cth). It is a matter for each user of this guidance to consider their individual situation and to comply with the new regime. Whether a business uses this template, in whole or in part, is a decision for each business. The FSC does not require any business or organisation to use these standards.

## Common data items

**Product identifier**

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| | Product APIR code | The product&#39;s APIR code. Must include if available | | M if available | |
| --- | --- | --- | --- | --- | --- |
| | Product ISIN code | The product&#39;s ISIN code. Must include if available | | M if available | |
| | Listing exchange | Code of exchange the product is listed on, using ISO Market Identifier Code (MIC). Must include if product is listed.If | ISO MIC – 4 character alpha | M if available | |
| | Product exchange code | The product&#39;s exchange code (for listed products). Must include if available. | | M if available | |
| | Product ARSN | Product ARSN. Must include if available | Nine-digit numeric | M if available | |
| | Product name | Financial instrument (Product) name. Note name is subject to change over time – not for machine analysis | Free text | M | |
| | Issuer product code | Issuer determined product code – should be the type of last resort.Don&#39;t reuse industry wide codes. | Combination of code for issuer plus internal issuer determined product code? | M only if previous fields blank | |

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
| | _Contact details (for advice AFSL) – refer standard data items_ |
| | _For each business under above AFSL: (for transactions report, only include businesses involved in transaction)_ |
| | ABN | | | M | |
| | Business Name | Free text. Not for machine analysis | | M | |
| | _For each adviser under each business: (for transactions report, only include advisers involved in transaction)_ |
| | FAR | | | M | |
| | _Contact details (for adviser) – refer standard data items –_ _do we need to include for every adviser?_ |
| | **If distributor is non-Advice AFSL (fund managers, platforms, online stockbrokers, insurance aggregators, mortgage brokers)** |
| | ACL | Australian Credit License (ACL) number of entity included in this subrecord. Must be used if entity holds an ACL | | M if available | |
| | AFSL | AFSL of distributor included in subrecord Must be included | | M | |
| | ABN | ABN of distributor included in subrecord Must be included | | M | |
| | Business Name | Not for machine analysis | | M | |
| | _Contact details (for non-advice AFSL) – refer standard data items_ |
| | _For each promoter under non-advice AFSL (for transactions report, only include promoters involved in transaction)_ |
| | AFSL | | | M | |
| | ABN | | | M | |
| | Business Name | | | M | |
| | _Contact details (for promoter) – refer standard data items_ |

**Contact details**

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| | Contact name | Contact details for this record - name | Free text | M | |
| --- | --- | --- | --- | --- | --- |
| | Contact title | Contact position title (eg Senior Product Manager; Compliance Manager). | Free text | O | |
| | Contact phone | Phone for contact person | Full international number format | M | |
| | Contact email | Email for contact person | XXX@XXX | M | |
| | Contact address | Address for contact person | Free text | O | |

##


## Data standard for DDO – TMDs for Investment Management

This data standard allows product issuers (under the DDO regime) to provide product distributors with the Target Market Determination(s) that issuers are required to make under the DDO regime.

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/conditional** | **Outstanding items** |
 || --- | --- | --- | --- | --- | --- | --- ||
 | Version of standard | Version number of data standard. Can be non-integer. Major versions should increment by 1. Minor changes (backwards compatible) can increment by less than 1. (eg 2.1, 2.2, 2.3) | XXX | M |
 | || | Date approved | Date that this TMD version was approved | Format YYYY-MM-DD | M |
 |
 |
| | Date sent | Date that this TMD version report was sent | Format YYYY-MM-DD | OM | | |
| | Issuer AFSL | | | O | |
| --- | --- | --- | --- | --- | --- |
| | Issuer ABN | | Nine-digit numeric | M | |
| --- | --- | --- | --- | --- | --- |
| | Issuer name | | | | |
| --- | --- | --- | --- | --- | --- |
| | _**Product TMD – Allow multiple subrecords, one for each product TMD (one TMD per product)**_ | |
| --- | --- | --- |
| | _Product identifier – see common data items_ | |
| | TMD Version | Version number of the TMD. Can be non-integer. Major versions increment by 1. Minor changes (backwards compatible) increment by less than 1 | XXX | M | | |
| | TMD Status | The status of the TMD which indicates whether it should be distributed. A status of unavailable or closed will be a signal to distributor to stop retail distribution (unless the distribution is excluded dealing). | Single choice of {Available / Under review / Unavailable – stop distribution / closed} | M | Need to check rules about interaction with version number. | |
| | Date approved | Date that this TMD version was approved | Format YYYY-MM-DD | M | | |
| | Mandatory review date | Next mandatory review date for this TMD version. A review can occur before this date. | Format YYYY-MM-DD | M | | |
| | _Contact details (for TMD) – see common data items_ | |

| Data items specific to TMD |
| --- |
| **TMD Characteristic** | **TMD Values** |
| --- | --- |
| **1: Investment Objective** | 1.1: Investment Objective Description | A description of the investment objective of the product, including growth/ defensive split | Free-text field
 | O | Revisit issues with mandatory/optional sections. EG if one part of a section is filled in, all of section must be filled in. |
 |
| --- | --- | --- | --- | --- | --- | --- |
| 1.2: Capital Growth | Do the product investment objectives align with those of an investor seeking Capital Growth | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | Use key instead of text | |
| 1.3: Capital Preservation | Do the product investment objectives align with those of an investor seeking Capital Preservation | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M || |
| 1.4: Capital Guaranteed | Do the product investment objectives align with those of an investor seeking Capital Guaranteed | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M || |
| 1.5: Regular Income | Do the product investment objectives align with those of an investor seeking Regular Income? | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 1.6: Specialist | Do the product investment objectives align with those of an investor with Specialist objectives? | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | ||
| **2: Product Use** | 2.1: Product Use Description | A description of the investment objective of the product, including asset allocation and diversification information | Free-text field | M | ||
| 2.2: Solution / Standalone (75% - 100%) | Is the product intended to be used as a Solution / Standalone product | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 2.3: Core Component (25% -75%) | Is the product intended to be used as a core component product | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 2.4: Satellite (0% - 25%) | Is the product intended to be used as a satellite product | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| **3: Investment Timeframe** | 3.1: Investment Timeframe Description | A description of the minimum suggested timeframe for holding the product | Free-text field | M | | |
| 3.2: Short (\&lt; 2 years) | Is it appropriate for investors to hold the product for 0-2 years before selling | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 3.3: Medium (2 – 6 years) | Is it appropriate for investors to hold the product for 2-6 years before selling | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 3.4: Long (\&gt; 6 years) | Is it appropriate for investors to hold the product for more than 6 years before selling | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| **4: Risk and return** | 4.1: Risk and Return description | A description of the product risk and return metrics, include risk band and the return hurdle rate | Free-text field | M | | |
| 4.2: Very high risk &amp; return | Does the product have very high risk and return attributes | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 4.3: High risk &amp; return | Does the product have high risk and return attributes | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 4.4: Medium risk &amp; return | Does the product have medium risk and return attributes | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 4.5: Low risk &amp; return | Does the product have low risk and return attributes | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 4.6: Capital guaranteed | Does the product have capital guaranteed attributes | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| **5: Redemption Frequency** | 5.1: Redemption Frequency description | A description of the intended frequency and mechanism for which investors redeem interests in the product | Free-text field | M | | |
| 5.2: Daily | Product suitable for investors that redeem interests daily | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 5.3: Weekly | Product suitable for investors that redeem interests weekly | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 5.4: Monthly | Product suitable for investors that redeem interests monthly | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 5.5: Quarterly | Product suitable for investors that redeem interests quarterly | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 5.6: Annually or longer | Product suitable for investors that redeem interests annually or longer | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| **6: Liquidity** | 6.1: Liquidity description | A description of the liquidity of the assets held by the fund | Free-text field | M | | |
| 6.2: Low | Are the assets predominantly low liquidity | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 6.3: Moderate | Are the assets predominantly moderate liquidity | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 6.4: High | Are the assets predominantly high liquidity | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| 6.5: Very high | Are the assets predominantly very high liquidity | Single choice of {In Target Market / Potentially in Target Market / Not considered in Target Market} | M | | |
| **Distribution conditions** | Available Direct? | Is product available direct (non intermediated) retail? | Y/N | M | | |
| | Direct conditions | Additional conditions on direct (non intermediated) retail. Only complete if previous is Y. | Free text | C | | |
| | Available on broad based platform? | Is product available on platforms? | Y/N | M | | |
| | Platform conditions | Additional conditions on distribution to platforms. Only complete if previous is Y. | Free text | C | | |
| | Available advised? | Is product available to clients subject to personal advice?[row for general advice?] | Y/N | M | | |
| | Advised distribution conditions | Additional conditions on distribution to clients subject to personal advice. Only complete if previous is Y. | Free text | C | | |
| **Review triggers** | _ **The following one field can be multivalued** _ | |
| | Review triggers | List one trigger per subrecord. As distributors don&#39;t need to action review triggers, there is no need for standardisation/ validation of the text | Free text | OM | | |
| | **Distributor reporting requirements** | |
| | How to send reports | Text indicating how distributors must send reports to issuer. Preference is for a URL link to instructions (must be permanent link) | | M | | |
| | Acquisition outside TM | Is there requirement for distributors to report on ALL dealings outside target market? | Y/N | M | | |
| | | If Y, should report follow FSC DDO data standard for transactions? Only complete if previous is Y | Y/N | C | | |
| | | If N, name of alternative data standard | Free text | C | | |
| | Report on some acquisitions outside TM | If report not required on all dealings outside target market, is a report required on some dealings outside target market other than significant dealings? | Y/N | C | | |
| | _ **Only answer following three fields if a report on some acquisitions outside TM is required** _ | |
| | | If Y, specify type of dealings outside target market requiring report | Free text | C | | |
| | | Should report on some trans follow FSC DDO data standard for transactions? | Y/N | C | | |
| | | If N, name of alternative data standard | Free text | C | | |
| | Frequency of report | Required frequency of report by distributors on dealings outside target market. | Select one of: {point of sale / end of calendar month / end of calendar quarter} | C | | |
| | | Required deadline for dealings report after end of relevant period (see previous field) – in number of days. Default is 10 days | XX | C | | |
| | Use Ccomplaints reporting standard? | Are complaints reporting required to use FSC complaints standard? | Y/N | M | | |
| | Minimum version of complaints standard | Distributor must submit complaints standard in this version of FSC standard or later. If blank, no requirement on version. Only complete if previous is Y. | X.X | O | | |
| | | Required content of complaints report by distributors. | Free text | M | | |
| | | Required frequency of report on complaints. Default is at time of complaint | Select one of: { time of complaint / end of calendar month / end of calendar quartermonthly/quarterly/half yearly/yearly} | M | | |
| | | Required deadline for complaints report after end of relevant period (see previous field) – in number of days. Default is 10 days | XX | M | | |
| | Significant dealing | As per statutory obligations s994F(6) | | M | Reporting on this is compulsory, with mandatory deadlines so unclear what to include in data standard | |
| **Appropriateness** | | Explanation how issuer considers TMD performs against appropriateness test as required by ASIC RG | Free text | M | | |
| **Footer record** | | | | | | |
| | | Count of TMDs in report | | | | |

## Data Standard for DDO – Complaints

This data standard allows product distributors to provide reports required under the DDO regime to product issuers relating to the complaints received by product distributors.

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/ conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
| 0.1 | Version of standard
 | Version number of data standard. Can be non-integer. Major versions should increment by 1. Minor changes (backwards compatible) can increment by less than 1. (eg 2.1, 2.2, 2.3) | XXX | M |
 |
| --- | --- | --- | --- | --- | --- |
| **0: Report header (Data items common to more than one DDO data standard)** |
|
 | Report unique ID | Report ID – unique to distributor. Can be combined with distributor ID to have industry-wide unique ID. | Each distributor would choose their own ID | O |
 |
|
 | Report date | Date that complaints report was sent.
If reissued, the new information replaces any reports within the defined report start and end period. | Format YYYY-MM-DD HH:MM:SS | M |
 |
|
 | Report Period Start | Period for which the report starts. Inclusive of day. | YYYY-MM-DD
 | M |
 |
|
 | Report Period End | Period for which the report ends. Inclusive of day. | YYYY-MM-DD | M |
 |
| **1: Reporting entity (same for all report types) – this entity may be reporting on behalf of multiple distributors. The list of distributors included in the report is included later** |
|
 | _Reporting entity identifier – refer common data items_ |
|
 | _Contact details (for this report) – refer common data items_ |
| **2: Distribution entities covered by this report (same for all report types) (expect to see multiple subrecords in this section.-can have multiple subrecords.** |
|
 | _Distributor identifier – refer common data items_ |
|
 | List of product IDs |
 |
 |
 |
 |
| **3: Issuer pProducts covered by this report (same for all report types) – can have multiple subrecords** |
|
 | _Product identifier – see common data items_ |
| **4: Complaints summary** |
| **For further consideration: what matrix of distributors/products/complaints do we use?** |
| **Complaint details (1 subrecord per complaint)** |
|
 | Ccomplaint ID | Reporting entity internal code for complaint.Could be used in conjunction with reporting entity ABN/code to create industry wide unique code if needed.If amending a previous complaint, use the previous complaint ID and this record will replace the previous complaint record. | Must be unique within reporting entity. | M? |
 |
|
 | _ **Primary product involved in complaint** _ |
|
 | _Product identifier – refer common data items_ |
|
 | _**Other products involved in complaint (eg where primary complaint is about a managed fund on a platform, the primary complaint it about the managed fund but the name of the platform should be included below). Can have multiple subrecords**_ |
|
 | _Product identifier – refer common data items_ |
|
 | _ **Distributor involved in complaint** _ |
|
 | Distributor FAR (as above) | Financial Advice Register number of distributor involved in complaint. Must be used if distributor holds a FAR number. | Leave blank if no adviser | M if available |
 |
|
 | Distributor ACL | Australian Credit License (ACL) number of distributor involved in complaint. Must be used if reporting entity holds an ACL |
 | M if available |
 |
|
 | Distributor AFSL (as above) | AFSL of distributor involved in complaint. Must be used if reporting entity holds and AFSL |
 | M if available |
 |
|
 | Distributor Product ID (as above) |
 | Leave blank if no product |
 |
 |
|
 | _ **Details of complaint** _ |
|
 | Complaint type | See RG 271 |
 | M | See ASIC CP |
|
 | Is complaint about product (issuer)? |
 | Y/N | M? |
 |
|
 | Is complaint about distribution/sales (distributor)? |
 | Y/N | M? |
 |
|
 | Financial impact? | Was the complainant impacted financially by the issue that they are complaining about? | Y/N | O? |
 |
|
 | Complaint date |
 | YYYY-MM-DD | M |
 |
|
 | Date of complaint resolution
 | Leave blank if not resolved or unknown | YYYY-MM-DD | M |
 |
|
 | Complaint content | This should include all the relevant details so that the issuer can understand the nature of the complaint | Free text | M? | Need to set a length limit on text |
|
 | AFCA referral? | Has complaint been referred to AFCA? | Y/N | M |
 |
|
 | AFCA referral date | Date of referral to AFCA. Only complete if previous is Y | YYYY-MM-DD | C |
 |
|
 | AFCA ID | AFCA ID of complaint. Only complete if &quot;AFCA referral?&quot; is Y |
 | O |
 |
|
 | _ **Validation Footer/Check sums** _ |
|
 | Number nil reports | Number of nil complaint records included in this file. Sum of this field and next field must equal number of complaint records in this file |
 | M |
 |
|
 | Number non-nil reports | Number of non-nil complaint records included in this file. |
 | M |
 |

## Data standard for DDO – Transactions/Dealings

This data standard relates to reports by product distributors to product issuers (under the DDO regime) relating to product transactions/dealings, including dealings that are outside the target market.

## Data standard

| **#** | **Data Item** | **Definition/description** | **Comment/coding** | **Mandatory/ optional/ conditional** | **Outstanding items** |
| --- | --- | --- | --- | --- | --- |
|
 | **0: Report Header (Data items common to more than one DDO data standard)** |
 |
| --- | --- | --- |
|
 | Version of standard | Version number of data standard Can be non-integer. Major versions should increment by 1. Minor changes (backwards compatible) can increment by less than 1. (eg 2.1, 2.2, 2.3) | XXX | M |
 |
|
 | Report Type | Is report Aall transactions by date range or transactions by unique identifier?.If transactions by date range, then expectation is there will only be one report for the particular date range.If transactions by unique ID, then there may be any number of reports for a date range | Single choice of: 1 = transactions by date range2 = transactions by unique identifier | M |
 |
|
 | Report unique ID | Report ID – unique to distributor. Can be combined with distributor ID to have industry-wide unique ID | Each distributor would choose their own ID | M |
 |
|
 | Is this report new or amendment? | Is this a new transaction report or a replacement to a previous report? Only use if report type is transactions by unique ID.If this is a replacement report, this should replace the previous report in full. | Y/N
 | M |
 |
|
 | ID of original report | If amendment, ID of original/previous report that is being amended. Only complete if previous field is Y | Same format as next itemreport unique ID | C |
 |
| 0.1 | Report date | Date that transaction report was made. If report is reissued, the new information replaces any reports within the defined report start and end period. | Format YYYY-MM-DD HH:MM:SS | M |
 |
|
 | Report period start | Initial date the extract report covers. Inclusive of day. Only complete if Report Type is &quot;transactions by date range&quot;. | Inclusive of the day. | MC |
 |
|
 | Report period end | Final date the extract report covers. Inclusive of day. Only complete if Report Type is &quot;transactions by date range&quot;. | Inclusive of the day. | MC |
 |
|
 | **Reporting entity – this entity may be reporting on behalf of multiple distributors. The list of distributors included in the report is included later** |
|
 | _Reporting entity identifier – refer common data items_ |
|
 | _Contact details (for this report) – refer common data items_ |
|
 | **2: Intermediaries / Distributors covered by this report – can be multiple subrecords – only include entities/distributors involved in transactions** |
|
 | _Distributor identifier – refer common data items_ |
|
 | **3: Reporting Dealings (Transactions)** |
 |
| _**If the report relates to multiple dealings, then the following rows need one subrecord for each dealing (within the main record)**_ |
|
 | Distributor type | The type of the distributor that was involved in the relevant dealing. This is the lowest level entity involved in distribution | Single choice of {adviser, platform, aggregator, promoter} | M |
 |
|
 | Distributor unique identifier | For adviser, FAR # of adviser.For all other types, AFSL # | FAR # or AFSL # | M |
 |
| 3.1 | Dealing inside TM? | Is this dealing inside the target market? | Y or N | M | Do we want an assessment of &quot;how far outside&quot; TM? |
|
 | Personal advice? | Is dealing an excluded dealing due to personal advice exemption? | Y/N | M |
 |
|
 | If personal advice and outside TM, outside TM reason | If dealing is outside target market, why did dealing proceed despite this? Field is mandatory if previous field is N and &quot;dealing inside TM&quot; is N. | Free text | C |
 |
| 3.3 | Transaction dDate of dealing | Date the dealing occurred | YYYY-MM-DD | M |
 |
| 3.4 | Transaction sSize of dealing | The $ value of the dealing included within the report should be sum insured for life, TPD and trauma and monthly benefit for IP. to &#39;match&#39; value of managed funds etc | ### | M if available |
 |
|
 | Number | Number of units, shares etc involved in dealing | ### | O |
 |
|
 | _Product identifier – see common data items_ |
|
 | _ **Following is mandatory for dealings not subject to personal advice** _ |
|
 | TMD version | The version of the TMD for the product that the customer was assessed against. | ### | M |
 |
|
 | TMD data standard type | The type of the TMD data standard that is used for the following fields | Select one out of {Funds management/superannuation/life insurance} |
 |
 |
|
 | TMD data standard version | The version of the TMD data standard that is used for the following fields | ### | M |
 |
|
 | _**TMD assessment for dealing – one subrecord for each characteristic in the TMD (refer relevant TMD data standard)**_ |
|
 | TMD characteristic | The ID of the TMD characteristic. | Data validation as per the relevant TMD data standard | As per TMD data standard |
 |
| 3.6 | TMD Value | The value of the TMD characteristic for the investor(s) the subject of the report. One value per characteristic.This must be the assessment of the customer against the TMD, not a copy of the TMD.
Need to explain difference between Not assessed and Unable to be assessed. | Data validation as per the relevant TMD data standardCoding as per data standard (In target market, potentially in target market or not in target market). Add additional codes: Not assessed and Unable to be assessed | as per TMD data standard |
 |
|
 | _ **Validation Footer/Check sums** _ |
|
 | # dealings | Count of number of dealings included in overall record |
 | M |
 |
|
 | Sum of $ | Sum of $ values included in overall record under data item &quot;size of dealing&quot; |
 | M |
 |

## _Copyright &amp; Disclaimer for data standard_

_© 2021 Financial Services Council Limited ABN 82 080 744 163._

_The intellectual property rights in this document, including the copyright in the document, are owned by and retained by the FSC and its licensors. The FSC grants you a non-exclusive non-transferable licence for you and the organisation you represent (the User) to use this document internally within the User&#39;s business, including making copies, reproductions, and modifications of the document, and otherwise as expressly set out in the conditions below for so long as the User licenses this data standard._

_You and the User acknowledge and agree that the information contained in this document has been collated and prepared by the FSC for the sole purpose of assisting Users to manage their compliance with Part 7.8A of the Corporations Act 2001. The information contained in this document is based on current sources and practice as at 2021. The information contained in this document may need to be updated and revised as new sources of information emerge or practices change over time._

_Users should use their own judgment when making use of this material and should carefully evaluate its currency, completeness and relevance for their own purposes as well as the extent to which this material can or should be modified to suit the User&#39;s products._

_While steps have been taken to ensure the accuracy of the information contained in this document, the FSC does not guarantee, and accepts no legal liability whatsoever or howsoever arising from or connected to, the accuracy, currency, completeness of any material contained in this document (including any liability that may flow directly or indirectly from the modification of the information contained in this document) and makes no warranties as to suitability for you or non-infringement or for compliance with the data requirements under Part 7.8A of the Act._

![](RackMultipart20210316-4-8lfz9_html_b01c81e2b01acfb2.jpg)

© 2021 Financial Services Council Limited Page 1