# Lead to Account Match
This is a simple way to reference the domain in the email address of a lead record with the account website domain. If the email domain matches the account domain, a Best Matched Account field is updated on the Lead record. 

This project was inspired by <a href="https://www.amazon.com/Lightning-Sales-Ops-Salesforce-Development-ebook/dp/B06XMR93HC">Lightning Sales Ops</a> by Matt Bertuzzi.

<h2>Use Case</h2>
<hr>
<p>When a sales team is using both the Leads and Contact & Account objects, in particular when BDR teams are working both inbound and outbound leads, conflict can emerge if a clear connection doesn't exist between a lead that came inbound and an account that the sales team has been prospecting outbound.</p> 

<p>To help mitigate conflict and ensure continuity in account ownership a team needs to know if a lead comes inbound from an account they've been working outbound. This allows the company to easily provide key account information to the BDR or proactively route leads to the team member who is already actively working an account.</p>  

<h2>Solution</h2>
<hr>
<p>A no-code solution is to use the Process Builder and a Flow to populate a custom Best Matched Account field on the lead record. A flow is used to reference the email address of a lead record and reference the website domain of all existing accounts and if a match exists to populate that information on the lead.</p> 

<p>Once an account match has been made, additional information about the account can then be displayed ont the lead record, such as Account Status, Last Activity Date, Account Owner and BDR Signal.</p> 
