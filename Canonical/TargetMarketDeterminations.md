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


| **1: Investment Objective** | 1.1: Investment Objective Description | A description of the investment objective of the product, including growth/ defensive split | Free-text field | O | Revisit issues with mandatory/optional sections. EG if one part of a section is filled in, all of section must be filled in. | |
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

## _Copyright &amp; Disclaimer for data standard_

_© 2021 Financial Services Council Limited ABN 82 080 744 163._

_The intellectual property rights in this document, including the copyright in the document, are owned by and retained by the FSC and its licensors. The FSC grants you a non-exclusive non-transferable licence for you and the organisation you represent (the User) to use this document internally within the User&#39;s business, including making copies, reproductions, and modifications of the document, and otherwise as expressly set out in the conditions below for so long as the User licenses this data standard._

_You and the User acknowledge and agree that the information contained in this document has been collated and prepared by the FSC for the sole purpose of assisting Users to manage their compliance with Part 7.8A of the Corporations Act 2001. The information contained in this document is based on current sources and practice as at 2021. The information contained in this document may need to be updated and revised as new sources of information emerge or practices change over time._

_Users should use their own judgment when making use of this material and should carefully evaluate its currency, completeness and relevance for their own purposes as well as the extent to which this material can or should be modified to suit the User&#39;s products._

_While steps have been taken to ensure the accuracy of the information contained in this document, the FSC does not guarantee, and accepts no legal liability whatsoever or howsoever arising from or connected to, the accuracy, currency, completeness of any material contained in this document (including any liability that may flow directly or indirectly from the modification of the information contained in this document) and makes no warranties as to suitability for you or non-infringement or for compliance with the data requirements under Part 7.8A of the Act._

![](RackMultipart20210316-4-8lfz9_html_b01c81e2b01acfb2.jpg)

© 2021 Financial Services Council Limited