# TestsThe below issues were uncovered while component testing this enhancement. For additional information and screenshots, please see the testing below for each of the Business Deliverables included for this enhancement.
1.	Exporting the ACH Audit Report to Excel works, but no data is included in the Excel export. An example is attached to this note.
2.	The ACH Audit Report includes reporting for Manual submissions of ACH files via the ACH Transmission folders but there is no “Channel” in the descriptions. -- done
3.	When a name is removed from the OFACE whitelist, the original row for adding the person to the whitelist disappears. –  done
4.	The row for ignoring an OFAC suspect includes Tomcat7” instead of the actual user. – need to review the logging code
5.	When an ACH Limit is deleted, the original row for adding the ACH Limit disappears from the report. done 
6.	When an ACH Limit is deleted, the description includes “Limit xxx” instead of what user input for description. update audit, need to test
7.	When an ACH Limit is added, the description includes “Limit xxx” instead of what user input for description. update audit, need to test
8.	When a SEC Code is enabled, a Timestamp of 00:00:00 is included instead of actual time. update audit, cannot reproduce
9.	When a SEC Code is disabled, a Timestamp of 00:00:00 is included instead of actual time. update audit, cannot reproduce
10.	When a SEC Code is disabled, the original row for enabling the SEC Code disappears from the report. add audit
11.	Could not test if the report includes reversals of entire files or individual entries due to errors with the reversal screen in ACH Manager. debug
12.	Could not test if the report includes single transaction files due to an error with the Single Transaction Screen in ACH Manager. debug
13.	Adding an ACH Approver is not captured in the ACH Audit Report. add audit
14.	Editing an ACH Approver is not captured in the ACH Audit Report. add audit
15.	Reassigning an ACH Approver is not captured in the ACH Audit Report. add audit
16.	The only field to edit for a regular customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. add audit
17.	When the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report. add audit
18.	Removing an agreement is not captured in the ACH Audit Report. add audit
19.	When an agreement is removed, the original row for adding the agreement disappears from the report. add audit
20.	Changing the Chargeback Account Field of an agreement is not captured in the ACH Audit Report. add audit
21.	Changing the Multi-Day Limit Field of an agreement is not captured in the ACH Audit Report. add audit
22.	Changing the Days Field of an agreement is not captured in the ACH Audit Report. add audit
23.	Changing the Customer’s Email Field of an agreement is not captured in the ACH Audit Report. add audit
24.	Changing the Channel Field of an agreement is not captured in the ACH Audit Report. add audit
25.	Checking the Unbalanced Box of an agreement is not captured in the ACH Audit Report. add audit
26.	The only field to edit for a Third Party Customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. add audit
27.	When the “Service Charge Account” Field is edited for a Third Party Customer, the Add Customer row disappears from the ACH Audit Report. add audit  
Business Deliverables for ITS 114011:

1.	Manual submissions of ACH files via the ACH Transmission folders.
BOLB: 
 
PASS: 
 
AP: 
 
TPV: 
 
FED:
 
   - No “Channel” in description.

2.	Approval or Declining of an ACH over the limit file. 
Approved:
 
Declined:
 

3.	OFAC whitelist removal. 
 
-Row for addition to whitelist disappears when name is removed.

4.	OFAC whitelist addition. 
 

5.	OFAC alert suspect ignore. 
 
-Username of “Tomcat7” included instead of actual user.

6.	Add or deleting an ACH Limit
Adding:
 
- Description includes “Limit 3” instead of what user input for description:
 
Deleting:
 
- Description includes “Limit 3” instead of what user input for description (see above example)
-Row for adding ACH Limit disappears when ACH Limit is deleted. 
7.	Enabling or Disabling SEC Codes (user must hit save). 
Enable:
 
-A Timestamp of 00:00:00 is included instead of actual time
Disable:
 
-A Timestamp of 00:00:00 is included instead of actual time
-Row for enabling SEC Code disappears when SEC code is disabled.

8.	ACH Reversals (entries or full files)
Entry:
Cannot test due to current error:
 
File:
Cannot test due to current error:
 

9.	“Process Transaction” of the Singe Transaction feature. 
Cannot test because “Tran Type” Dropdown will not populate:
  
10.	Create Loan
 

11.	Add/Edit/Delete/Reassign an approver in the approver’s manager.
Add:
   Not captured in ACH Audit Report:
 
Edit:
   Not captured in ACH Audit Report:
 
Delete:
 
Reassign:
   Not captured in ACH Audit Report:
 

12.	Add/Edit Customers
Add Customer:
 
Edit Customer:
The only field to edit for a regular customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. 
Also when the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report.
 

13.	Add/Remove/Suspend/Activate/Sync agreements.
Add Agreement:
 
Remove Agreement:
Removing an agreement is not captured in the ACH Audit Report.
- Row for adding Agreement disappears when Agreement is removed.
Suspend Agreement:
 
Activate Agreement:
 
Sync Agreement:
 
 
14.	Editing fields, enabling check boxes, or updating drop downs within the agreements (user must submit the changes in the agreement and click save on the main agreement page for the changes to take affect).
Change Account Field:
 
Change Chargeback Account Field:
   Changing the Chargeback Account Field is not captured in the ACH Audit Report. 
Change SEC Field:
 
Change Tran Type Field:
 
Change Multi-Day Limit Field:
   Changing the Multi-Day Limit Field is not captured in the ACH Audit Report.
Change Days Field:
   Changing the Days Field is not captured in the ACH Audit Report.
Change Frequency Field:
 
Change Customer’s Email Field:
   Changing the Customer’s Email Field is not captured in the ACH Audit Report.
Change Prefunding Field:
 
Change Channel Field:
   Changing the Channel Field is not captured in the ACH Audit Report.
Check Same Day ACH Box:
 
Check Unbalanced Box:
   Checking the Unbalanced Box is not captured in the ACH Audit Report.
Check Enable Box (Prefunding):
 
Check ACH Emails Box:
 
Check NOC Emails Box:
 
Check Return Emails Box:
 

15.	Resubmit and Archiving Exceptions
Resubmit:
 
Archive:
 
 
16.	Add/Edit/Removal of bypass company IDs from the new front end (ITS 112767).
Add:
 
Edit:
The only field to edit for a Third Party Customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report.
Also when the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report.
 
Remove:
It is not possible to remove a Third Party Customer via the user interface.
The below issues were uncovered while component testing this enhancement. For additional information and screenshots, please see the testing below for each of the Business Deliverables included for this enhancement.
1.	Exporting the ACH Audit Report to Excel works, but no data is included in the Excel export. An example is attached to this note.
2.	The ACH Audit Report includes reporting for Manual submissions of ACH files via the ACH Transmission folders but there is no “Channel” in the descriptions. -- done
3.	When a name is removed from the OFACE whitelist, the original row for adding the person to the whitelist disappears. –  done
4.	The row for ignoring an OFAC suspect includes Tomcat7” instead of the actual user. – need to review the logging code
5.	When an ACH Limit is deleted, the original row for adding the ACH Limit disappears from the report. done 
6.	When an ACH Limit is deleted, the description includes “Limit xxx” instead of what user input for description. update audit, need to test
7.	When an ACH Limit is added, the description includes “Limit xxx” instead of what user input for description. update audit, need to test
8.	When a SEC Code is enabled, a Timestamp of 00:00:00 is included instead of actual time. update audit, cannot reproduce
9.	When a SEC Code is disabled, a Timestamp of 00:00:00 is included instead of actual time. update audit, cannot reproduce
10.	When a SEC Code is disabled, the original row for enabling the SEC Code disappears from the report. add audit
11.	Could not test if the report includes reversals of entire files or individual entries due to errors with the reversal screen in ACH Manager. debug
12.	Could not test if the report includes single transaction files due to an error with the Single Transaction Screen in ACH Manager. debug
13.	Adding an ACH Approver is not captured in the ACH Audit Report. add audit
14.	Editing an ACH Approver is not captured in the ACH Audit Report. add audit
15.	Reassigning an ACH Approver is not captured in the ACH Audit Report. add audit
16.	The only field to edit for a regular customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. add audit
17.	When the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report. add audit
18.	Removing an agreement is not captured in the ACH Audit Report. add audit
19.	When an agreement is removed, the original row for adding the agreement disappears from the report. add audit
20.	Changing the Chargeback Account Field of an agreement is not captured in the ACH Audit Report. add audit
21.	Changing the Multi-Day Limit Field of an agreement is not captured in the ACH Audit Report. add audit
22.	Changing the Days Field of an agreement is not captured in the ACH Audit Report. add audit
23.	Changing the Customer’s Email Field of an agreement is not captured in the ACH Audit Report. add audit
24.	Changing the Channel Field of an agreement is not captured in the ACH Audit Report. add audit
25.	Checking the Unbalanced Box of an agreement is not captured in the ACH Audit Report. add audit
26.	The only field to edit for a Third Party Customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. add audit
27.	When the “Service Charge Account” Field is edited for a Third Party Customer, the Add Customer row disappears from the ACH Audit Report. add audit  
Business Deliverables for ITS 114011:

1.	Manual submissions of ACH files via the ACH Transmission folders.
BOLB: 
 
PASS: 
 
AP: 
 
TPV: 
 
FED:
 
   - No “Channel” in description.

2.	Approval or Declining of an ACH over the limit file. 
Approved:
 
Declined:
 

3.	OFAC whitelist removal. 
 
-Row for addition to whitelist disappears when name is removed.

4.	OFAC whitelist addition. 
 

5.	OFAC alert suspect ignore. 
 
-Username of “Tomcat7” included instead of actual user.

6.	Add or deleting an ACH Limit
Adding:
 
- Description includes “Limit 3” instead of what user input for description:
 
Deleting:
 
- Description includes “Limit 3” instead of what user input for description (see above example)
-Row for adding ACH Limit disappears when ACH Limit is deleted. 
7.	Enabling or Disabling SEC Codes (user must hit save). 
Enable:
 
-A Timestamp of 00:00:00 is included instead of actual time
Disable:
 
-A Timestamp of 00:00:00 is included instead of actual time
-Row for enabling SEC Code disappears when SEC code is disabled.

8.	ACH Reversals (entries or full files)
Entry:
Cannot test due to current error:
 
File:
Cannot test due to current error:
 

9.	“Process Transaction” of the Singe Transaction feature. 
Cannot test because “Tran Type” Dropdown will not populate:
  
10.	Create Loan
 

11.	Add/Edit/Delete/Reassign an approver in the approver’s manager.
Add:
   Not captured in ACH Audit Report:
 
Edit:
   Not captured in ACH Audit Report:
 
Delete:
 
Reassign:
   Not captured in ACH Audit Report:
 

12.	Add/Edit Customers
Add Customer:
 
Edit Customer:
The only field to edit for a regular customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. 
Also when the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report.
 

13.	Add/Remove/Suspend/Activate/Sync agreements.
Add Agreement:
 
Remove Agreement:
Removing an agreement is not captured in the ACH Audit Report.
- Row for adding Agreement disappears when Agreement is removed.
Suspend Agreement:
 
Activate Agreement:
 
Sync Agreement:
 
 
14.	Editing fields, enabling check boxes, or updating drop downs within the agreements (user must submit the changes in the agreement and click save on the main agreement page for the changes to take affect).
Change Account Field:
 
Change Chargeback Account Field:
   Changing the Chargeback Account Field is not captured in the ACH Audit Report. 
Change SEC Field:
 
Change Tran Type Field:
 
Change Multi-Day Limit Field:
   Changing the Multi-Day Limit Field is not captured in the ACH Audit Report.
Change Days Field:
   Changing the Days Field is not captured in the ACH Audit Report.
Change Frequency Field:
 
Change Customer’s Email Field:
   Changing the Customer’s Email Field is not captured in the ACH Audit Report.
Change Prefunding Field:
 
Change Channel Field:
   Changing the Channel Field is not captured in the ACH Audit Report.
Check Same Day ACH Box:
 
Check Unbalanced Box:
   Checking the Unbalanced Box is not captured in the ACH Audit Report.
Check Enable Box (Prefunding):
 
Check ACH Emails Box:
 
Check NOC Emails Box:
 
Check Return Emails Box:
 

15.	Resubmit and Archiving Exceptions
Resubmit:
 
Archive:
 
 
16.	Add/Edit/Removal of bypass company IDs from the new front end (ITS 112767).
Add:
 
Edit:
The only field to edit for a Third Party Customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report.
Also when the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report.
 
Remove:
It is not possible to remove a Third Party Customer via the user interface.
The below issues were uncovered while component testing this enhancement. For additional information and screenshots, please see the testing below for each of the Business Deliverables included for this enhancement.
1.	Exporting the ACH Audit Report to Excel works, but no data is included in the Excel export. An example is attached to this note.
2.	The ACH Audit Report includes reporting for Manual submissions of ACH files via the ACH Transmission folders but there is no “Channel” in the descriptions. -- done
3.	When a name is removed from the OFACE whitelist, the original row for adding the person to the whitelist disappears. –  done
4.	The row for ignoring an OFAC suspect includes Tomcat7” instead of the actual user. – need to review the logging code
5.	When an ACH Limit is deleted, the original row for adding the ACH Limit disappears from the report. done 
6.	When an ACH Limit is deleted, the description includes “Limit xxx” instead of what user input for description. update audit, need to test
7.	When an ACH Limit is added, the description includes “Limit xxx” instead of what user input for description. update audit, need to test
8.	When a SEC Code is enabled, a Timestamp of 00:00:00 is included instead of actual time. update audit, cannot reproduce
9.	When a SEC Code is disabled, a Timestamp of 00:00:00 is included instead of actual time. update audit, cannot reproduce
10.	When a SEC Code is disabled, the original row for enabling the SEC Code disappears from the report. add audit
11.	Could not test if the report includes reversals of entire files or individual entries due to errors with the reversal screen in ACH Manager. debug
12.	Could not test if the report includes single transaction files due to an error with the Single Transaction Screen in ACH Manager. debug
13.	Adding an ACH Approver is not captured in the ACH Audit Report. add audit
14.	Editing an ACH Approver is not captured in the ACH Audit Report. add audit
15.	Reassigning an ACH Approver is not captured in the ACH Audit Report. add audit
16.	The only field to edit for a regular customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. add audit
17.	When the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report. add audit
18.	Removing an agreement is not captured in the ACH Audit Report. add audit
19.	When an agreement is removed, the original row for adding the agreement disappears from the report. add audit
20.	Changing the Chargeback Account Field of an agreement is not captured in the ACH Audit Report. add audit
21.	Changing the Multi-Day Limit Field of an agreement is not captured in the ACH Audit Report. add audit
22.	Changing the Days Field of an agreement is not captured in the ACH Audit Report. add audit
23.	Changing the Customer’s Email Field of an agreement is not captured in the ACH Audit Report. add audit
24.	Changing the Channel Field of an agreement is not captured in the ACH Audit Report. add audit
25.	Checking the Unbalanced Box of an agreement is not captured in the ACH Audit Report. add audit
26.	The only field to edit for a Third Party Customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. add audit
27.	When the “Service Charge Account” Field is edited for a Third Party Customer, the Add Customer row disappears from the ACH Audit Report. add audit  
Business Deliverables for ITS 114011:

1.	Manual submissions of ACH files via the ACH Transmission folders.
BOLB: 
 
PASS: 
 
AP: 
 
TPV: 
 
FED:
 
   - No “Channel” in description.

2.	Approval or Declining of an ACH over the limit file. 
Approved:
 
Declined:
 

3.	OFAC whitelist removal. 
 
-Row for addition to whitelist disappears when name is removed.

4.	OFAC whitelist addition. 
 

5.	OFAC alert suspect ignore. 
 
-Username of “Tomcat7” included instead of actual user.

6.	Add or deleting an ACH Limit
Adding:
 
- Description includes “Limit 3” instead of what user input for description:
 
Deleting:
 
- Description includes “Limit 3” instead of what user input for description (see above example)
-Row for adding ACH Limit disappears when ACH Limit is deleted. 
7.	Enabling or Disabling SEC Codes (user must hit save). 
Enable:
 
-A Timestamp of 00:00:00 is included instead of actual time
Disable:
 
-A Timestamp of 00:00:00 is included instead of actual time
-Row for enabling SEC Code disappears when SEC code is disabled.

8.	ACH Reversals (entries or full files)
Entry:
Cannot test due to current error:
 
File:
Cannot test due to current error:
 

9.	“Process Transaction” of the Singe Transaction feature. 
Cannot test because “Tran Type” Dropdown will not populate:
  
10.	Create Loan
 

11.	Add/Edit/Delete/Reassign an approver in the approver’s manager.
Add:
   Not captured in ACH Audit Report:
 
Edit:
   Not captured in ACH Audit Report:
 
Delete:
 
Reassign:
   Not captured in ACH Audit Report:
 

12.	Add/Edit Customers
Add Customer:
 
Edit Customer:
The only field to edit for a regular customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report. 
Also when the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report.
 

13.	Add/Remove/Suspend/Activate/Sync agreements.
Add Agreement:
 
Remove Agreement:
Removing an agreement is not captured in the ACH Audit Report.
- Row for adding Agreement disappears when Agreement is removed.
Suspend Agreement:
 
Activate Agreement:
 
Sync Agreement:
 
 
14.	Editing fields, enabling check boxes, or updating drop downs within the agreements (user must submit the changes in the agreement and click save on the main agreement page for the changes to take affect).
Change Account Field:
 
Change Chargeback Account Field:
   Changing the Chargeback Account Field is not captured in the ACH Audit Report. 
Change SEC Field:
 
Change Tran Type Field:
 
Change Multi-Day Limit Field:
   Changing the Multi-Day Limit Field is not captured in the ACH Audit Report.
Change Days Field:
   Changing the Days Field is not captured in the ACH Audit Report.
Change Frequency Field:
 
Change Customer’s Email Field:
   Changing the Customer’s Email Field is not captured in the ACH Audit Report.
Change Prefunding Field:
 
Change Channel Field:
   Changing the Channel Field is not captured in the ACH Audit Report.
Check Same Day ACH Box:
 
Check Unbalanced Box:
   Checking the Unbalanced Box is not captured in the ACH Audit Report.
Check Enable Box (Prefunding):
 
Check ACH Emails Box:
 
Check NOC Emails Box:
 
Check Return Emails Box:
 

15.	Resubmit and Archiving Exceptions
Resubmit:
 
Archive:
 
 
16.	Add/Edit/Removal of bypass company IDs from the new front end (ITS 112767).
Add:
 
Edit:
The only field to edit for a Third Party Customer is the “Service Charge Account” Field and that is not captured in the ACH Audit Report.
Also when the “Service Charge Account” Field is edited, the Add Customer row disappears from the ACH Audit Report.
 
Remove:
It is not possible to remove a Third Party Customer via the user interface.
