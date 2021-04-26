**Product identifier**

<table border="1" cellspacing="0" cellpadding="0" width="1086">
    <thead>
        <tr>
            <td width="66" valign="top">
                <p>
                    <strong>#</strong>
                </p>
            </td>
            <td width="170" valign="top">
                <p>
                    <strong>Data Item </strong>
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    <strong>Definition/description</strong>
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    <strong>Comment/coding</strong>
                </p>
            </td>
            <td width="156" valign="top">
                <p>
                    <strong>Mandatory/ optional/conditional</strong>
                </p>
            </td>
            <td width="193" valign="top">
                <p>
                    <strong>Outstanding items</strong>
                </p>
            </td>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Primary product identifier type
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    Which of the following types of IDs has been determined to
                    be the primary ID of the product. The primary ID is used in
                    the rest of the standard to identify the product uniquely.
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    Single choice of {APIR/Exchange code/ISIN/USI/Issuer code}
                </p>
            </td>
            <td width="156" valign="top">
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Product APIR code
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    The product’s APIR code. Must include if available
                </p>
            </td>
            <td width="200" valign="top">
            </td>
            <td width="156" valign="top">
                <p>
                    M if available
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Listing exchange
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    Code of exchange the product is listed on, using ISO Market
                    Identifier Code (MIC). Must include if product is listed.
                </p>
                <p>
                    If a product is listed in Australia and another country,
                    prefer the Australian listing.
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    ISO MIC – 4 character alpha
                </p>
            </td>
            <td width="156" valign="top">
                <p>
                    M if available
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Product exchange code
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    The product’s exchange code (for listed products). Must
                    include if available.
                </p>
            </td>
            <td width="200" valign="top">
            </td>
            <td width="156" valign="top">
                <p>
                    M if available
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Product ISIN code
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    The product’s ISIN code. Must include if available
                </p>
            </td>
            <td width="200" valign="top">
            </td>
            <td width="156" valign="top">
                <p>
                    O if available
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    USI
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    For super funds: 9 digit APIR code or 14 digit numeric code
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    Will be either 9 or 14 digits
                </p>
            </td>
            <td width="156" valign="top">
                <p>
                    M if available
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Issuer product code
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    Issuer determined product code – should be the type of last
                    resort.
                </p>
                <p>
                    Don’t reuse industry wide codes in this field.
                </p>
                <p>
                    (platforms, insurance products)
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    Combination of code for issuer plus internal issuer
                    determined product code?
                </p>
            </td>
            <td width="156" valign="top">
                <p>
                    M only if previous fields blank
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Product name
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    Financial instrument (Product) name. Note name is subject
                    to change over time – not for machine analysis
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    Free text
                </p>
            </td>
            <td width="156" valign="top">
                <p>
                    M
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
        <tr>
            <td width="66" valign="top">
            </td>
            <td width="170" valign="top">
                <p>
                    Product ARSN
                </p>
            </td>
            <td width="302" valign="top">
                <p>
                    Product ARSN. Must include if available.
                </p>
                <p>
                    Do not use this field as primary product identifier
                </p>
            </td>
            <td width="200" valign="top">
                <p>
                    Nine-digit numeric
                </p>
            </td>
            <td width="156" valign="top">
                <p>
                    M if available
                </p>
            </td>
            <td width="193" valign="top">
            </td>
        </tr>
    </tbody>
</table>
## _Copyright &amp; Disclaimer for data standard_

_© 2021 Financial Services Council Limited ABN 82 080 744 163._

_The intellectual property rights in this document, including the copyright in the document, are owned by and retained by the FSC and its licensors. The FSC grants you a non-exclusive non-transferable licence for you and the organisation you represent (the User) to use this document internally within the User&#39;s business, including making copies, reproductions, and modifications of the document, and otherwise as expressly set out in the conditions below for so long as the User licenses this data standard._

_You and the User acknowledge and agree that the information contained in this document has been collated and prepared by the FSC for the sole purpose of assisting Users to manage their compliance with Part 7.8A of the Corporations Act 2001. The information contained in this document is based on current sources and practice as at 2021. The information contained in this document may need to be updated and revised as new sources of information emerge or practices change over time._

_Users should use their own judgment when making use of this material and should carefully evaluate its currency, completeness and relevance for their own purposes as well as the extent to which this material can or should be modified to suit the User&#39;s products._

_While steps have been taken to ensure the accuracy of the information contained in this document, the FSC does not guarantee, and accepts no legal liability whatsoever or howsoever arising from or connected to, the accuracy, currency, completeness of any material contained in this document (including any liability that may flow directly or indirectly from the modification of the information contained in this document) and makes no warranties as to suitability for you or non-infringement or for compliance with the data requirements under Part 7.8A of the Act._

![](RackMultipart20210316-4-8lfz9_html_b01c81e2b01acfb2.jpg)

© 2021 Financial Services Council Limited