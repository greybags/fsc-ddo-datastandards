# TARGET MARKET DETERMINATION - TMD

## DDO machine readable fund data template	


<table>
   <tr>
      <td>DATA</td>
      <td>DEFINITION</td>
      <td>CODIFICATION</td>
      <td>COMMENT</td>
      <td>Mandatory / Optional / Conditional / Indicative - FSC Licensee </td>
      <td>Mandatory / Optional / Conditional / Indicative - Non FSC Licensee </td>
   </tr>
   <tr>
      <td>TMD Data Set Information</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>Product Identifiers</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Primary_Product_Identifier_Type</td>
      <td>Which of the following types of IDs has been determined to be the primary ID of the product. The primary ID is used in the rest of the standard to identify the product uniquely. The issuer code must not be used unless no other codes are available.</td>
      <td>Single choice of {APIR/Exchange code/ISIN/USI/Issuer code}</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_Product_APIR_Code</td>
      <td>The product’s APIR code. Must include if available</td>
      <td></td>
      <td></td>
      <td>M if using as Primary Product identifier type, otherwise optional</td>
      <td>M if using as Primary Product identifier type, otherwise optional</td>
   </tr>
   <tr>
      <td>_Listing_Exchange </td>
      <td>"Code of exchange the product is listed on, using ISO Market Identifier Code (MIC). Must include if product is listed.</td>
   </tr>
   <tr>
      <td>If a product is listed in Australia and another country, prefer the Australian listing."</td>
      <td>ISO MIC – 4 character alpha</td>
      <td></td>
      <td>M if “product exchange code” is used as Primary Product identifier type, otherwise optional</td>
      <td>M if “product exchange code” is used as Primary Product identifier type, otherwise optional</td>
   </tr>
   <tr>
      <td>_Product_Exchange_Code</td>
      <td>The product’s exchange code (for listed products). Must include if “listing exchange” is completed.</td>
      <td></td>
      <td></td>
      <td>M if using as Primary Product identifier type, otherwise optional</td>
      <td>M if using as Primary Product identifier type, otherwise optional</td>
   </tr>
   <tr>
      <td>_Product_ISIN_Code</td>
      <td>The product’s ISIN code. Must include if available</td>
      <td></td>
      <td></td>
      <td>M if using as Primary Product identifier type, otherwise optional</td>
      <td>M if using as Primary Product identifier type, otherwise optional</td>
   </tr>
   <tr>
      <td>_Issuer_Product_Code</td>
      <td>"Issuer determined product code – should be the type of last resort.</td>
   </tr>
   <tr>
      <td>Don’t reuse industry wide codes in this field.</td>
   </tr>
   <tr>
      <td>For products without industry wide codes, can use this field, plus code for issuer, to set an industry-wide code."</td>
      <td>Free text</td>
      <td></td>
      <td>M only if previous fields blank</td>
      <td>M only if previous fields blank</td>
   </tr>
   <tr>
      <td>_Product_Name</td>
      <td>Financial instrument (Product) name. Note name is subject to change over time – not for machine analysis</td>
      <td>Plain text only</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_Product_ARSN</td>
      <td>"Product ARSN. Must include if available.</td>
   </tr>
   <tr>
      <td>Do not use this field as primary product identifier"</td>
      <td>Nine-digit numeric</td>
      <td></td>
      <td>M if available </td>
      <td>M if available </td>
   </tr>
   <tr>
      <td>Entity Type</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Entity_Name</td>
      <td>"The name of the entity/Issuer included in this data item. May or may not be a product distributor. </td>
   </tr>
   <tr>
      <td>Not for machine analysis "</td>
      <td>Plain text only</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_Entity_AFSL</td>
      <td>Entity/Issuer AFSL. </td>
      <td></td>
      <td></td>
      <td>M if using as entity identifier type, otherwise optional</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Entity_ABN</td>
      <td>Entity ABN. Must be used if reporting holds an ABN</td>
      <td></td>
      <td></td>
      <td>M if available </td>
      <td>M</td>
   </tr>
   <tr>
      <td>Report Contact Details</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Contact_Name</td>
      <td>Contact details for this record - name</td>
      <td>Plain text only</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_Contact_Title</td>
      <td>Contact position title (eg Senior Product Manager; Compliance Manager).</td>
      <td>Plain text only</td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Contact_Phone</td>
      <td>Phone for contact person</td>
      <td>Full international number format</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_Contact_Email</td>
      <td>Email for contact person</td>
      <td>XXX@XXX</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_Contact_Address</td>
      <td>Address for contact person</td>
      <td>Plain text only</td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Contact_Company</td>
      <td>The name of the company that this contact represents</td>
      <td>Plain text only</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>TMD Report Header Information</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Version_Of_Data_Standard</td>
      <td>Version number of data standard. Can be non-integer. Major versions should increment by 1. Minor changes (backwards compatible) can increment by less than 1. (eg 2.1, 2.2, 2.3)</td>
      <td>XXX</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Date_Sent</td>
      <td>Date that this report was sent</td>
      <td>DD-MM-YYYY</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>Product TMD </td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_TMD_Version</td>
      <td>Version number of the TMD (integers only). </td>
      <td>1</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_TMD_Status</td>
      <td>The status of the TMD which indicates whether it should be distributed. Available / Under review / Unavailable – stop distribution / Closed</td>
      <td>A / U / US / C</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_TMD_Date</td>
      <td>Date that this TMD data template version was approved</td>
      <td>DD-MM-YYYY</td>
      <td></td>
      <td>M</td>
      <td>M</td>
   </tr>
   <tr>
      <td>_TMD_PDF_Link</td>
      <td>URL link to location of PDF version of the TMD</td>
      <td>www.link/TMD.com.au</td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Data Items Specific to TMD for each product</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Target_Market</td>
      <td>Summary of target market as per TMD template</td>
      <td>Free text</td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Consumer’s investment objective</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Investment_Objective_Description</td>
      <td>The description of the investment objective of the product, including growth/ defensive split. </td>
      <td>Free text</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Capital_Growth</td>
      <td>Do the product investment objectives align with those of an investor seeking Capital Growth </td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Capital_Preservation</td>
      <td>Do the product investment objectives align with those of an investor seeking Capital Preservation </td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Capital_Guaranteed</td>
      <td>Do the product investment objectives align with those of an investor seeking Capital Guaranteed </td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Regular_Income</td>
      <td>Do the product investment objectives align with those of an investor seeking Regular Income</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Consumer’s intended product use</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Product_Use_Description</td>
      <td>The description of the intended product use of the product, including asset allocation and portfolio diversification information</td>
      <td>Free text</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Standalone_More_Than_75_percent</td>
      <td>Is the product intended to be used as a Solution / Standalone product</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Core_Component_25_To_75_percent</td>
      <td>Is the product intended to be used as a core component of a portfolio</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Satellite_Less_Than_25_percent</td>
      <td>Is the product intended to be used as a Satellite component of a portfolio</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Consumer’s investment timeframe</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Investment_Timeframe_Description</td>
      <td>The description of the minimum suggested timeframe for holding the product</td>
      <td>Free text</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Investment_Timeframe_Short_Less_Than_2_years</td>
      <td>Is it appropriate for investors to hold the product for 0-2 years before selling</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Investment_Timeframe_Medium_2_To_6_years</td>
      <td>Is it appropriate for investors to hold the product for 2-6 years before selling</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Investment_Timeframe_Long_More_Than_6_years</td>
      <td>Is it appropriate for investors to hold the product for more than 6 years before selling</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Consumer’s Risk (ability to bear loss) and Return profile </td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Risk_Return_Description </td>
      <td>The description of the product risk and return metrics, include risk band and the return hurdle rate</td>
      <td>Free text</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Return_Objective_Very_High_Risk_And_Return</td>
      <td>Does the product have very high risk and return attributes</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Return_Objective_High_Risk_And_ Return</td>
      <td>Does the product have high risk and return attributes</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Return_Objective_Medium_Risk_And_Return</td>
      <td>Does the product have medium risk and return attributes</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Return_Objective_Low_Risk_And_Return</td>
      <td>Does the product have low risk and return attributes</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Customer’s need to withdraw money</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Redemption_Frequency</td>
      <td>A description of the intended redemption frequency, access constraints and other relevant liquidity considerations.</td>
      <td>Free text</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Redemption_Frequency_Daily</td>
      <td>Product suitable for investors that redeem interests daily</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Redemption_Frequency_Weekly</td>
      <td>Product suitable for investors that redeem interests weekly</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Redemption_Frequency_Monthly</td>
      <td>Product suitable for investors that redeem interests monthly</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Redemption_Frequency_Quarterly</td>
      <td>Product suitable for investors that redeem interests quarterly</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Redemption_Frequency_Annually_Or_Longer</td>
      <td>Product suitable for investors that redeem interests annually or longer</td>
      <td>Y / Neutral / N </td>
      <td>In target market (Y) / Potentially in target market (Neutral) / Not considered in target market (N) </td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Distribution Conditions </td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_No_Distribution_Conditions</td>
      <td>Confirm if there are no distribution conditions</td>
      <td>Y  / N </td>
      <td>Select one of – Y - There are no distribution conditions / N - There are distribution conditions</td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Personal_Advice_Distribution_Only</td>
      <td>Only suitable for distribution to consumers who have received personal advice? Y = distribution only permitted to those who have received personal advice</td>
      <td>Y  / N </td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Personal_Advice_Distribution_Rationale</td>
      <td>Only suitable for distribution to consumers who have received personal advice – set out rationale</td>
      <td>Free Text</td>
      <td></td>
      <td>C</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_Specified_Distributors_Channels</td>
      <td>Only suitable for distribution through specified distributors / specified channels</td>
      <td>Y  / N </td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Specified_Distributors_Channels_Details</td>
      <td>Only suitable for distribution through specified distributors / specified channels - Specify</td>
      <td>Free Text</td>
      <td>[Insert distributor name (including unique ID) or channel name – insert a semicolon between each named distributor or distribution channel]</td>
      <td>M</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_Specified_Distributors_Channels_Rationale </td>
      <td>Only suitable for distribution through specified distributors / specified channels – set out rationale</td>
      <td>Free Text</td>
      <td></td>
      <td>C</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_Other_Distribution_Conditions</td>
      <td>Are there any other distribution conditions (ie sale via use of call script only)</td>
      <td>Y  / N </td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Other_Distribution_Conditions_Details</td>
      <td>Specify and describe any other distribution conditions </td>
      <td>Free Text</td>
      <td></td>
      <td>C</td>
      <td>C</td>
   </tr>
   <tr>
      <td>Review </td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Review_Trigger_Material_Change_FSC</td>
      <td>Align with FSC if applicable </td>
      <td>Free Text</td>
      <td>Material change to key attributes, fund investment objective and/or fees. </td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Review_Trigger_Material_Deviation_FSC</td>
      <td>Align with FSC if applicable </td>
      <td>Free Text</td>
      <td>Material deviation from benchmark / objective over sustained period.</td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Review_Trigger_Not_Performed_As_Disclosed_FSC</td>
      <td>Align with FSC if applicable </td>
      <td>Free Text</td>
      <td>Key attributes have not performed as disclosed by a material degree and for a material period.</td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Review_Trigger_Significant_Dealing_FSC</td>
      <td>Align with FSC if applicable </td>
      <td>Free Text</td>
      <td>Determination by the issuer of an ASIC reportable Significant Dealing</td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Review_Trigger_High_Number_Complaints_FSC</td>
      <td>Align with FSC if applicable </td>
      <td>Free Text</td>
      <td>Material or unexpectedly high number of complaints (as defined in section 994A(1) of the Act) about the product or distribution of the product.</td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Review_Trigger_Product_Intervention_Powers_FSC</td>
      <td>Align with FSC if applicable </td>
      <td>Free Text</td>
      <td>The use of Product Intervention Powers, regulator orders or directions that affects the product.</td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Initial_Review</td>
      <td>X months. For example ‘15 months’. Therefore 15 months after “TMD Date”</td>
      <td></td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Maximum_Subsequent_Review_Period</td>
      <td>X months. For example ‘39 months’. e.g. 3 years plus 3 months</td>
      <td></td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Reporting</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Reporting_Instructions</td>
      <td>Instructions to distributors on how to report to issuers. Exact copy from TMD </td>
      <td>Free text</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Acquisition_Outside_TM</td>
      <td>Does issuer require reporting on transactions outside TMD that the Distributor is aware of?</td>
      <td>Y  / N </td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_FSC_Data_Standard_Transactions_Reporting</td>
      <td>If previous field is answered Y, should report follow FSC DDO data standard for transactions? </td>
      <td>Y  / N </td>
      <td></td>
      <td>C</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_Alternative_Data_Standard_For_Transactions</td>
      <td>If N, Link to alternative data standard if used</td>
      <td>URL</td>
      <td></td>
      <td>C</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_Frequency_Of_Report</td>
      <td>Required frequency of report by distributors on dealings outside target market. </td>
      <td>Select one of: [monthly/quarterly/half yearly/yearly]</td>
      <td></td>
      <td>C</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_FSC_Data_Standard_For_Complaints</td>
      <td>Is complaints reporting required to use FSC complaints standard</td>
      <td>Y  / N </td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Alternative_Data_Standard_For_Complaints</td>
      <td>If N, link to alternative data standard</td>
      <td>Y  / N </td>
      <td></td>
      <td>O</td>
      <td>C</td>
   </tr>
   <tr>
      <td>_Complaints_Reporting_Frequency</td>
      <td>Required frequency of report on complaints. Default is at time of complaint</td>
      <td>Select one of: [monthly/quarterly/half yearly/yearly]</td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Significant dealings distributor guidance</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_FSC_Significant_Dealing_Guidance</td>
      <td>Is issuer using the FSC template for guidance to distributors on significant dealing?</td>
      <td>Y  / N </td>
      <td></td>
      <td>M</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Non_FSC_Significant_Dealing_Distributor_Guidance</td>
      <td>If previous field is “N”, provide alternate guidance. Exact copy from TMD </td>
      <td>Free text</td>
      <td></td>
      <td>C</td>
      <td>M</td>
   </tr>
   <tr>
      <td>APPROPRIATENESS</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Appropriateness</td>
      <td>"Explanation of how Issuer considers TMD performs against appropriateness test as required by ASIC 274.64–66. </td>
   </tr>
   <tr>
      <td>Include here exact copy from TMD "</td>
      <td>Free text</td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>Additional Custom Fields</td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
   </tr>
   <tr>
      <td>_Custom_Data_1</td>
      <td>Additional data used to define the target market not included in the form above</td>
      <td></td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Custom_Data_2</td>
      <td>Additional data used to define the target market not included in the form above</td>
      <td></td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Custom_Data_3</td>
      <td>Additional data used to define the target market not included in the form above</td>
      <td></td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td>_Custom_Data_4</td>
      <td>Additional data used to define the target market not included in the form above</td>
      <td></td>
      <td></td>
      <td>O</td>
      <td>O</td>
   </tr>
   <tr>
      <td></td>
   </tr>
</table>