# rental_book
Rental Book Process Automation

Background: Price Approvals team on-boarded rental books in Apr’20. This process is very critical and unique when compared to existing MKPLs and SOPs. The share value goes down rapidly if prices in queues are not approved in a timely manner. After the launch, Price Approvals team have involved dedicated SPOCs to take approval actions based on the defined SOP steps. During non-peak season, the queues need to be cleared once on daily basis and the frequency increased to 3x times on daily basis. The peak season was from 04th Aug till 24th Sep. 

Situation: I was given the responsibility to check for automation feasibility in rental books since the SOPs were straight forward and for most of the merchants, the approval action was based on recommended price thresholds. For example, Under Cengage merchant, if the recommended price is above $9.98 then the recommendations can be approved without other validation steps. Likewise this was noticed across 7 such merchants which had price thresholds that SPOCs were following before taking approval action. For each time, SPOCs had to spend 15 minutes in manually clearing the queues for straight forward cases.

Behavior: I connected with tenured SPOC from PA team and got the KT on the SOP. Post which I started developing the script in UI VISION browser extension. The script is built to validate the recommended price range were we have certain threshold for each merchant in PA process. This process will pick up listings which are above the price range according to the input data and then approves all the recommendations. The same action is repeated for all the recommendations in the given page. 

Impact: The automation reduces the manual effort of an auditor to approve the recommendations under rental book process.

Before Automation:
•	Opening individual URLs (as many as 7MKPLs)
•	Verifying all the recommendations in each page (100 recommendations per page)
•	SPOCs Approve the recommendations which have recommended prices above the threshold (Based on manual comparison)

After Automation:
•	create a one-time CSV input file with URLs and corresponding threshold values (One time activity)
•	Execute the macro
Because of this automation, we were able to save 1.5 hours each week while also avoiding the risk of manually accepting pricing that were below the threshold.

