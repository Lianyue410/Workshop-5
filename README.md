Task 1 
1.Appropriate classification: Restricted. The customer.json datastore contains direct identifiers (name, chino) and GDPR special category data (medication, ethnicity), which can uniquely identify an individual and pose a high risk if compromised
2.Access control: Apply the principle of least privilege. Only the operations team (who need it for deliveries) should have access to the raw customer.json data. Implement Role-Based Access Control (RBAC) and field-level authorization. All access must be logged and monitored.
3.Retention: Data should be stored for the minimum time necessary. Customer delivery data should be deleted once the order is completed and the refund period expires. Do not retain indefinitely.
Task 2 
2.Classification labels:
customer.json: Restricted. (Strict access control, short retention, encryption).
medicationbyvolume.json: Confidential. (Accessible to analysts, longer retention based on business needs).
3.Access design strategy: (c) Restrict access to the operational database to only the operations team, and give access to the analysis databases to only those who need it, this aligns with least privilege.
4.Improving retention: Set automated retention policies. For the analysis DB, keep data as long as needed for the specific analysis and storage budget allows. For the operational DB, delete delivery data immediately after order confirmation.
5.Retention policy: (b) Set the retention policy for data in analysis databases based on time required to complete analyses and allocated storage budget, and delete delivery data once order completion is confirmed.
6.Privacy protection: (c) Access should be highly controlled, limited, and monitored. Because it contains identifiable sensitive information, it should be "Restricted", not just "Confidential", and retention should be minimized, not extended.
