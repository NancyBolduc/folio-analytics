# ACRL Collections Expenditures Reports  (UXPROD-2529)

Table of Contents
=================

  * [Status](#status)
  * [Purpose](#purpose)
  * [Filters](#filters)
  * [Output](#output)
  * [Requests not yet adressed](#requests)


## Status <a name="status"></a>
The ACRL Collection Expenditures comprises three different queries, ACRL Collection Expenditures A, B & C. The different use for each query is defined in this document under ‘Purpose’. As of 01/26/20, these queries are in development. 

## Purpose <a name="purpose"></a>
The ACRL Collection Expenditures comprises three different queries, ACRL Collection Expenditures A, B & C. The different use for each query is defined in this document under ‘Purpose’. As of 01/26/20, these queries are in development.   

<details>
  <summary markdown="span">Click here to read more!</summary>  
  <br>
  
 <p> 
<ins>ACRL Collection Expenditures A:</ins>

<p>
This query provides a total amount of material expenditures, broken down by invoice lines and including any adjustment made at the invoice level. The overall total will be calculated by adding all invoice lines together by downloading your results into an Excel sheet or by using any other reporting tools like Tableau. Please note that the addition of the invoice adjustment is manually calculated, starting with calculating the percentage of each invoice line based on the total of the invoice lines (per invoice), and then added to each invoice line accordingly. For example, if an invoice adjustment is for shipping, the cost will be distributed to each invoice lines according to the percentage calculated. Therefore, the total amount of expenditures will include the cost of shipping. If your institution is recording shipping separately and do not want to add this cost (if entered as an invoice adjustment) to the total amount of material expenditures, then the option would be to use the ACRL Collection Expenditures B and add any invoice adjustments to it as needed. The total of adjustments made at the invoice level will be provided by running the ACRL Collection Expenditures C. 
<br>
<p>
<ins>ACRL Collection Expenditures B:</ins>
This query provides a total amount of material expenditures, broken down by invoice lines. The overall total will be calculated by adding all invoice lines together. This can be achieved by downloading your results into an Excel sheet or by using any other reporting tools like Tableau. Please note that it does not include any adjustment made at the invoice level. If one want to get the total of invoice lines plus the total of invoice adjustment that are ‘Not Prorated’ and ‘In Addition To’ separately, then the ARCL Collection Expenditures B and C queries should be run jointly. 
<br>
<p>
 <ins>ACRL Collection Expenditures C:</ins>
This query will return only the adjustments added at the invoice level when ‘Not Prorated’ and ‘In addition To’ are selected. The overall total will be calculated by adding all invoice adjustments total amount together. This can be achieved by downloading your results into an Excel sheet or by using any other reporting tools like Tableau. For example, if your institution is using the invoice adjustment to record tax and or shipping cost and you don’t want to add this cost to your POs recorded at the invoice lines level, then the ARCL Collection Expenditures C will give you the total amount spent for these invoice adjustments. The ACRL Collection Expenditure B can be used in conjunction with the ACRL Collection Expenditures C to provide the total amount of material spent but keeping the invoice adjustments separate from the invoice lines total, meaning not added to the overall PO cost.
Finally, note that in the ACRL survey, “Operation and Maintenance Expenses” section, “Preservation Services” measure includes costs for binding, which some institutions consider materials expenditures. If one want to record Binding in Preservation Cost and this element was recorded in a specific fund and paid through the FOLIO inventory, a separate query will need to be run to get the total amount of binding cost and subtract it from the ACRL Collection Expenditures total amount.
At this time, we are assuming that “Operations and Maintenance Expenses” are not recorded as a material expense in Folio along with salary and wages.
The annual ACRL Academic Library Trends and Statistics survey asks members to report their total materials expenditures broken into one-time, ongoing, and all other materials/services expenditures.  It also asks, if possible, that members break out: e-book expenditures from within one-time expenditures; and e-book and e-journal expenditures from within ongoing expenditures.
The current (FY20) ACRL survey requests are described briefly below, and fully at  https://acrl.countingopinions.com/  
<br>
<br>
 <h4>Additional information from 2020 survey:</h4>
 
| Material/Services expenses  |  |
| ------------- | ------------- |
| One-time purchase of books, serial backfiles, and other materials  | Include: onetime purchases of books, serials, and all other materials (electronic or 			physical, including locally held e-resources), purchased on a one-time basis.<br>Exclude: expenses for computer software used to support library operations or to link to 	external networks and anything purchased on a subscription basis.
| E-books (20a)<br> (if available)  | Include:  Include expenditures for any e-books purchased on a one-time basis, e-	books 		purchases triggered through a PDA or DDA program. <br>Exclude: Ongoing subscriptions to e-book packages and deposit account as expenditures 	until the library receives access to an e-book   |
| Ongoing commitments to subscriptions:  | Include: Expenses for ongoing commitments for all formats, including serials and any 	other items committed to annually, including annual electronic platform or access 	fees. Expenditures for standing orders if possible  |
| E-books (21a)<br> (if available):  | Include: ongoing subscriptions to ebook packages; include annual fees for e-book 	platforms  |
| E-journals 21b <br> (if available):  | Include: expenses for e-journals purchased in an ongoing basis   | 
| All other material/services cost  | ACRL is not fully prescriptive about what should be included in the category “all other 	materials/services expenditures”; for the most part, it only indicates what these 	expenditures “may” include.  This is possibly because members may not easily break out 	these costs.  It may also be because some institutions do not consider the expenditures 	ACRL recommends materials expenditures, but other operating expenditures, and, 	following local procedures, institutions may need or want to include them as other 	operating expenditures.  ACRL suggests that “all other materials/services” might 	include, e.g.: document delivery/interlibrary loan services; pay-per-view journal articles 	transactions; fees expended for short-term loans as part of a DDA or PDA 	program.  On 	the other hand, ACRL does specifically indicate that it considers expenditures for 	bibliographic management systems (e.g., EndNote, RefWorks) materials expenditures.  	See the ACRL documentation for more info.  Each institution will need to 	decide what is 	correct for them.  It is suggested data notes are provided if local practices differ. 	Services cost may include MARC records, OCLC and HathiTrust.

Note that the ACRL survey is aligned with the NCES Academic Library survey, so these measures can also be used for that survey.
<p>
ACRL requests that expenditures be reported for the most recent 12-month period that corresponds to the institution's fiscal year. All expenses should be reported in whole dollars in the most appropriate category to provide an unduplicated count of expenses. 
 <p>
 <h4>Relevant LDP/FOLIO documentation:</h4> 
 
 * API reference documentation for all modules located at:  https://dev.folio.org/reference/api/
 * Schema Spy has visual representation of tables at https://glintcore.net:8443/ldp/schemaspy/public/relationships.html
 * FOLIO raml parser: https://docs.google.com/spreadsheets/d/1m_Cq_GmZX37gJPEjVWt9eOLXskUjSLUb-8KapWj0SIw/edit#gid=24879874
 * Inventory Beta - Metadata Elements (being kept up to date by Charlotte): https://docs.google.com/spreadsheets/d/1RCZyXUA5rK47wZqfFPbiRM0xnw8WnMCcmlttT7B3VlI/edit#gid=952741439
 * LDP table relationships: https://glintcore.net:8443/ldp/schemaspy/public/relationships.html
 <p>
 The most current U.S. Association of College & Research Libraries (ACRL) survey documentation is available here: https://acrl.countingopinions.com/  Earlier documentation is available here: https://acrl.countingopinions.com/index.php?page_id=5
 p
 <h4>Future: Custom fileds</h4> 
 <p>
 There is JIRA issue created to be able to add custom fields to Purchase Orders and Purchase Order Lines. This could be useful for ACRL reporting in the future.
https://issues.folio.org/plugins/servlet/mobile#issue/UXPROD-2865

  </details>


## Filters <a name="filters"></a>
This is a sub paragraph, formatted in heading 3 style

## Output <a name="output"></a>
The second paragraph text

## Requests not yet adressed <a name="requests"></a>
<br>
ACRL Collection expenditures report by location:
At this time, the location data is only available through the PO lines. Since in many cases the total amount of the PO lines is at $0, using this location data would not return accurate data. A link from the PO lines to Holdings is currently in development, UXPROD-268. An additional report may be created once the issue is resolved and data available.
<br>
Payment date:
The invoice ‘payment date’ is currently in development. This element should be added to the query as soon as it becomes available.

