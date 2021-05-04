# TARGET MARKET DETERMINATION - TMD

## DDO machine readable fund data template	


<table border="0" cellspacing="0" cellpadding="0">
    <tbody>
        <tr>
            <td>
                <p align="center">
                    <strong>NUM</strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>DATA</strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>DEFINITION</strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>CODIFICATION</strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>COMMENT</strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>
                        Mandatory / Optional / Conditional / Indicative
                    </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>TMD Data Set Information</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Product Idenifitiers </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Primary_Product_Identifier_Type</strong>
                </p>
            </td>
            <td>
                <p>
                    Which of the following types of IDs has been determined to
                    be the primary ID of the product. The primary ID is used in
                    the rest of the standard to identify the product uniquely.
                </p>
            </td>
            <td>
                <p>
                    APIR/Exchange code/ISIN/USI/Issuer code
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Product_APIR_Code</strong>
                </p>
            </td>
            <td>
                <p>
                    The product’s APIR code. Must include if available
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M if available </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Listing_Exchange </strong>
                </p>
            </td>
            <td>
                <p>
                    Code of exchange the product is listed on, using ISO Market
                    Identifier Code (MIC). Must include if product is listed.
                    <br/>
                    If a product is listed in Australia and another country,
                    prefer the Australian listing.
                </p>
            </td>
            <td>
                <p>
                    ISO MIC – 4 character alpha
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M if available </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Product_Exchange_Code</strong>
                </p>
            </td>
            <td>
                <p>
                    The product’s exchange code (for listed products). Must
                    include if available
                </p>
            </td>
            <td>
                <p>
                    Alphanumeric
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M if available </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Product_ISIN_Code</strong>
                </p>
            </td>
            <td>
                <p>
                    The product’s ISIN code. Must include if available
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O if avaibable</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00060
                </p>
            </td>
            <td>
                <p>
                    <strong>_Issuer_Product_Code</strong>
                </p>
            </td>
            <td>
                <p>
                    Issuer determined product code – should be the type of last
                    resort. Don’t reuse industry wide codes in this field.
                    <br/>
                    (platforms, insurance products)
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M only if previous fields blank</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00070
                </p>
            </td>
            <td>
                <p>
                    <strong>_Product_Name</strong>
                </p>
            </td>
            <td>
                <p>
                    Financial instrument (Product) name
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    00080
                </p>
            </td>
            <td>
                <p>
                    <strong>_Product_ARSN</strong>
                </p>
            </td>
            <td>
                <p>
                    Product ARSN. Must include if available.
                    <br/>
                    Do not use this field as primary product identifier
                </p>
            </td>
            <td>
                <p>
                    Nine-digit numeric
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M if available </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Contact Details</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    01010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Contact_Name</strong>
                </p>
            </td>
            <td>
                <p>
                    Contact details for this record - name
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    01020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Contact_Title</strong>
                </p>
            </td>
            <td>
                <p>
                    Contact position title (eg Senior Product Manager;
                    Compliance Manager).
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    01030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Contact_Phone</strong>
                </p>
            </td>
            <td>
                <p>
                    Phone for contact person
                </p>
            </td>
            <td>
                <p>
                    Full international number format
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    01040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Contact_Email</strong>
                </p>
            </td>
            <td>
                <p>
                    Email for contact person
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    01050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Contact_Address</strong>
                </p>
            </td>
            <td>
                <p>
                    Address for contact person
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>
                        Data standard for DDO – TMDs for Investment Management
                    </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Version_Of_Data_Standard</strong>
                </p>
            </td>
            <td>
                <p>
                    Version number of data standard. Can be non-integer. Major
                    versions should increment by 1. Minor changes (backwards
                    compatible) can increment by less than 1. (eg 2.1, 2.2,
                    2.3)
                </p>
            </td>
            <td>
                <p>
                    1.0
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Date_Sent</strong>
                </p>
            </td>
            <td>
                <p>
                    Date that this TMD data template version was sent
                </p>
            </td>
            <td>
                <p>
                    DD-MM-YYYY
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Issuer_AFSL</strong>
                </p>
            </td>
            <td>
                <p>
                    Issuer AFSL
                </p>
            </td>
            <td>
                <p>
                    Nine-digit numeric
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Issuer_ABN</strong>
                </p>
            </td>
            <td>
                <p>
                    Issuer ABN
                </p>
            </td>
            <td>
                <p>
                    Nine-digit numeric
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Issuers_Name</strong>
                </p>
            </td>
            <td>
                <p>
                    Name of product issuer
                </p>
            </td>
            <td>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong> </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02060
                </p>
            </td>
            <td>
                <p>
                    <strong>_TMD_Version</strong>
                </p>
            </td>
            <td>
                <p>
                    Version number of the TMD (integers only).
                </p>
            </td>
            <td>
                <p>
                    1.0
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02070
                </p>
            </td>
            <td>
                <p>
                    <strong>_TMD_Status</strong>
                </p>
            </td>
            <td>
                <p>
                    The status of the TMD which indicates whether it should be
                    distributed. Available / Under review / Unavailable – stop
                    distribution / Closed
                </p>
            </td>
            <td>
                <p>
                    A / U / US / C
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02080
                </p>
            </td>
            <td>
                <p>
                    <strong>_Date_Approved</strong>
                </p>
            </td>
            <td>
                <p>
                    Date that this TMD data template version was approved
                </p>
            </td>
            <td>
                <p>
                    DD-MM-YYYY
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02090
                </p>
            </td>
            <td>
                <p>
                    <strong>_TMD_PDF_Link</strong>
                </p>
            </td>
            <td>
                <p>
                    URL link to location of PDF version of the TMD
                </p>
            </td>
            <td>
                <p>
                    www.link/TMD.com.au
                </p>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    02100
                </p>
            </td>
            <td>
                <p>
                    <strong>_Mandatory_Review_Date</strong>
                </p>
            </td>
            <td>
                <p>
                    Next mandatory review date for this TMD version. A review
                    can occur before this date.
                </p>
            </td>
            <td>
                <p>
                    DD-MM-YYYY
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>TMD Characteristics</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Investment objective</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    03010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Investment_Objective_Discription</strong>
                </p>
            </td>
            <td>
                <p>
                    The description of the investment objective of the product,
                    including growth/ defensive split.
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    03020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Capital_Growth</strong>
                </p>
            </td>
            <td>
                <p>
                    Do the product investment objectives align with those of an
                    investor seeking Capital Growth
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    03030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Capital_Preservation</strong>
                </p>
            </td>
            <td>
                <p>
                    Do the product investment objectives align with those of an
                    investor seeking Capital Preservation
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    03040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Capital_Guaranteed</strong>
                </p>
            </td>
            <td>
                <p>
                    Do the product investment objectives align with those of an
                    investor seeking Capital Guaranteed
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    03050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Regular_Income</strong>
                </p>
            </td>
            <td>
                <p>
                    Do the product investment objectives align with those of an
                    investor seeking Regular Income
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Product Use</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    04010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Product_Use_Description</strong>
                </p>
            </td>
            <td>
                <p>
                    The description of the minimum suggested timeframe for
                    holding the product
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    04020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Standalone_more_than_75_percent</strong>
                </p>
            </td>
            <td>
                <p>
                    Is the product intended to be used as a Solution /
                    Standalone product
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    04030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Core_Component_25_to_75_percent</strong>
                </p>
            </td>
            <td>
                <p>
                    Is the product intended to be used as a core component of a
                    portfolio
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    04040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Satellite_less_than_25_percent</strong>
                </p>
            </td>
            <td>
                <p>
                    Is the product intended to be used as a Satellite component
                    of a portfolio
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Investment Timeframe</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    05010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Investment_Timframe_Description</strong>
                </p>
            </td>
            <td>
                <p>
                    The description of the minimum suggested timeframe for
                    holding the product
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
                <p align="center">
                    <strong> </strong>
                    <strong></strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                    <strong></strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    05020
                </p>
            </td>
            <td>
                <p>
                    <strong>
                        _Investment_Timeframe_Short_less_than_2_years
                    </strong>
                </p>
            </td>
            <td>
                <p>
                    Is it appropriate for investors to hold the product for 0-2
                    years before selling
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                    <strong></strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    05030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Investment_Timeframe_Medium_2_to_6_years</strong>
                </p>
            </td>
            <td>
                <p>
                    Is it appropriate for investors to hold the product for 2-6
                    years before selling
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                    <strong></strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    05040
                </p>
            </td>
            <td>
                <p>
                    <strong>
                        _Investment_Timeframe_Long_more_than_6_years
                    </strong>
                </p>
            </td>
            <td>
                <p>
                    Is it appropriate for investors to hold the product for
                    more than 6 years before selling
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                    <strong></strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Risk and Return</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    06010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Risk_Return_Description </strong>
                </p>
            </td>
            <td>
                <p>
                    The description of the product risk and return metrics,
                    include risk band and the return hurdle rate
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    06020
                </p>
            </td>
            <td>
                <p>
                    <strong>
                        _Return_Objective_Very_High_Risk_and_ Return
                    </strong>
                </p>
            </td>
            <td>
                <p>
                    Does the product have very high risk and return attributes
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    06030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Return_Objective_High_Risk_and_ Return</strong>
                </p>
            </td>
            <td>
                <p>
                    Does the product have high risk and return attributes
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    06040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Return_Objective_Medium_Risk_and_Return</strong>
                </p>
            </td>
            <td>
                <p>
                    Does the product have medium risk and return attributes
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    06050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Return_Objective_Low_Risk_and_Return</strong>
                </p>
            </td>
            <td>
                <p>
                    Does the product have low risk and return attributes
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Redemption frequency</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    07010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Redemption_Frequency</strong>
                </p>
            </td>
            <td>
                <p>
                    A description of the intended redemption frequency, access
                    constraints and other relevant liquidity considerations.
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    07020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Redemption_Frequency_Daily</strong>
                </p>
            </td>
            <td>
                <p>
                    Product suitable for investors that redeem interests daily
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    07030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Redemption_Frequency_Weekly</strong>
                </p>
            </td>
            <td>
                <p>
                    Product suitable for investors that redeem interests weekly
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    07040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Redemption_Frequency_Monthly</strong>
                </p>
            </td>
            <td>
                <p>
                    Product suitable for investors that redeem interests
                    monthly
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    07050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Redemption_Frequency_Quarterly</strong>
                </p>
            </td>
            <td>
                <p>
                    Product suitable for investors that redeem interests
                    quarterly
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    07060
                </p>
            </td>
            <td>
                <p>
                    <strong>_Redemption_Frequency_Annually_or_Longer</strong>
                </p>
            </td>
            <td>
                <p>
                    Product suitable for investors that redeem interests
                    annually or longer
                </p>
            </td>
            <td>
                <p>
                    Y / Neutral / N / Negative
                </p>
            </td>
            <td>
                <p>
                    In target market (Y) / Potentially in target market
                    (Neutral) / Not considered in target market (N)
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>DISTRIBUTION INFORMATION</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Distribution Conditions / Restrictions</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08010
                </p>
            </td>
            <td>
                <p>
                    <strong>_No_Distribution_Conditions</strong>
                </p>
            </td>
            <td>
                <p>
                    Confirm if there are no distribution conditions
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
                <p>
                    Select one of – Y - There are no distribution conditions /
                    N - There are distribution conditions
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Personal_Advice_Distribution_Only_1</strong>
                </p>
            </td>
            <td>
                <p>
                    Only suitable for distribution to consumers who have
                    received personal advice – Confirm
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Personal_Advice_Distribution_Only_2</strong>
                </p>
            </td>
            <td>
                <p>
                    Only suitable for distribution to consumers who have
                    received personal advice – set out rationale
                </p>
            </td>
            <td>
                <p>
                    Free Text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Specified_Distributor_Channels_Only_1</strong>
                </p>
            </td>
            <td>
                <p>
                    Only suitable for distribution through specified
                    distributors / specified channels - Confirm
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Specified_Distributor_Channels_Only_2</strong>
                </p>
            </td>
            <td>
                <p>
                    Only suitable for distribution through specified
                    distributors / specified channels - Specify
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08060
                </p>
            </td>
            <td>
                <p>
                    <strong>_Specified_Distributor_Channels_Only_3</strong>
                </p>
            </td>
            <td>
                <p>
                    Only suitable for distribution through specified
                    distributors / specified channels – set out rationale
                </p>
            </td>
            <td>
                <p>
                    Free Text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08070
                </p>
            </td>
            <td>
                <p>
                    <strong>_Other_Distributions_Conditions</strong>
                </p>
            </td>
            <td>
                <p>
                    Are there any other distribution conditions (ie sale via
                    use of call script only)
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    08080
                </p>
            </td>
            <td>
                <p>
                    <strong>_Other_Distributions_Conditions_1</strong>
                </p>
            </td>
            <td>
                <p>
                    Specify and describe any other distribution conditions
                </p>
            </td>
            <td>
                <p>
                    Free Text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Review Triggers</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    09010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Review_Triggers</strong>
                </p>
            </td>
            <td>
                <p>
                    List one trigger per subrecord. As distributors don’t need
                    to action review triggers, there is no need for
                    standardisation/ validation of the text
                </p>
            </td>
            <td>
                <p>
                    Free Text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    09020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Initial_Review</strong>
                </p>
            </td>
            <td>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    09030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Maximum_Initial_Review_Date</strong>
                </p>
            </td>
            <td>
            </td>
            <td>
                <p>
                    DD-MM-YYYY
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    09040
                </p>
            </td>
            <td>
                <p>
                    <strong>_Subsequent_Reviews</strong>
                </p>
            </td>
            <td>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td nowrap="" valign="bottom">
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    09050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Maximum_Subsequent_Review_Date</strong>
                </p>
            </td>
            <td>
            </td>
            <td>
                <p>
                    DD-MM-YYYY
                </p>
            </td>
            <td nowrap="" valign="bottom">
            </td>
            <td>
                <p align="center">
                    <strong>O</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Distributor Reporting Requirement</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10010
                </p>
            </td>
            <td>
                <p>
                    <strong>_How_to_Send_Reports</strong>
                </p>
            </td>
            <td>
                <p>
                    URL link to instructions (must be permanent link)
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Acquisition_Outside_TMD</strong>
                </p>
            </td>
            <td>
                <p>
                    Does issuer require reporting on transactions outside TMD
                    that the Distributor is aware of?
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10030
                </p>
            </td>
            <td>
                <p>
                    <strong>_FSC_Data_Standard_Transactions</strong>
                </p>
            </td>
            <td>
                <p>
                    If previous field is answered Y, should report follow FSC
                    DDO data standard for transactions?
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10040
                </p>
            </td>
            <td>
                <p>
                    <strong>
                        _Alternative_Data_Standard_for_Transactions
                    </strong>
                </p>
            </td>
            <td>
                <p>
                    If N, Link to alternative data standard if used
                </p>
            </td>
            <td>
                <p>
                    URL
                </p>
            </td>
            <td>
                <p>
                    <strong> </strong>
                </p>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10050
                </p>
            </td>
            <td>
                <p>
                    <strong>_Frequency_of_Report</strong>
                </p>
            </td>
            <td>
                <p>
                    Required frequency of report by distributors on dealings
                    outside target market.
                </p>
            </td>
            <td>
                <p>
                    Select one of: [end of calendar month / end of calendar
                    quarter]
                </p>
            </td>
            <td nowrap="" valign="bottom">
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10060
                </p>
            </td>
            <td>
                <p>
                    <strong>_FSC_Data_Standard_for_Complaints</strong>
                </p>
            </td>
            <td>
                <p>
                    Is complaints reporting required to use FSC complaints
                    standard
                </p>
            </td>
            <td>
                <p>
                    Y / N
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10070
                </p>
            </td>
            <td>
                <p>
                    <strong>_Alternative_Data_Standard_for_Complaints</strong>
                </p>
            </td>
            <td>
                <p>
                    If N, link to alternative data standard
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>C</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10080
                </p>
            </td>
            <td>
                <p>
                    <strong>_Complaint_Reporting_Frequency</strong>
                </p>
            </td>
            <td>
                <p>
                    Required frequency of report on complaints. Default is at
                    time of complaint
                </p>
            </td>
            <td>
                <p>
                    Select one of: [monthly/quarterly/half yearly/yearly]
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    10090
                </p>
            </td>
            <td>
                <p>
                    <strong>_Significant_Dealings</strong>
                </p>
            </td>
            <td>
                <p>
                    As per statutory obligations s994F(6)
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td nowrap="" valign="bottom">
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>APPROPRIATENESS</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    11010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Appropriateness</strong>
                </p>
            </td>
            <td>
                <p>
                    Explanation of how issuer considers TMD performs against
                    appropriateness test as required by ASIC RG
                </p>
            </td>
            <td>
                <p>
                    Free text
                </p>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong>M</strong>
                    <strong></strong>
                </p>
            </td>
        </tr>
        <tr>
            <td colspan="6">
                <p>
                    <strong>Additional Custom Fields</strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    12010
                </p>
            </td>
            <td>
                <p>
                    <strong>_Custom_Data_1</strong>
                </p>
            </td>
            <td>
                <p>
                    Additional data used to define the target market not
                    included in the form above
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong> </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    12020
                </p>
            </td>
            <td>
                <p>
                    <strong>_Custom_Data_2</strong>
                </p>
            </td>
            <td>
                <p>
                    Additional data used to define the target market not
                    included in the form above
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong> </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    12030
                </p>
            </td>
            <td>
                <p>
                    <strong>_Custom_Data_3</strong>
                </p>
            </td>
            <td>
                <p>
                    Additional data used to define the target market not
                    included in the form above
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong> </strong>
                </p>
            </td>
        </tr>
        <tr>
            <td>
                <p align="center">
                    12040
                </p>
            </td>
            <td >
                <p>
                    <strong>_Custom_Data_4</strong>
                </p>
            </td>
            <td>
                <p>
                    Additional data used to define the target market not
                    included in the form above
                </p>
            </td>
            <td>
            </td>
            <td>
            </td>
            <td>
                <p align="center">
                    <strong> </strong>
                </p>
            </td>
        </tr>
    </tbody>
</table>
