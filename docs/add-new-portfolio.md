New Portfolio Page Checklist
Preparation

☐ Duplicate an existing working portfolio page
☐ Rename the file using your naming convention
☐ Example: momentum-june01.html

Google Sheets Setup
Create Main Portfolio Sheet

☐ Create new sheet
☐ Example: Momentum June 01

Required columns:
☐ Ticker
☐ Shares
☐ Price
☐ TOTAL $

Create History Sheet

☐ Create history sheet
☐ Example: Momentum June 01 History

Required:
☐ “Total” column
☐ Historical totals added over time

Portfolio HTML Page
Update Portfolio Title

☐ Change page heading

Example:

<h2>MOMENTUM</h2>
Update Main Sheet Loader

☐ Replace old sheet name

Example:

loadSheet("Momentum June 01", "handlePortfolio");
Update History Loader

☐ Replace old history sheet

Example:

loadSheet("Momentum June 01 History", "handleHistory");
Homepage Card Setup
Duplicate Existing Card

☐ Copy an existing homepage card block

Update Link

☐ Change href

Example:

href="momentum-june01.html"
Update Share Link

☐ Change data-link

Example:

data-link="momentum-june01.html"
Update Card Title

☐ Change strategy name

Example:

<h4>MOMENTUM</h4>
Update IDs

☐ Update total id

Example:

id="momentum-total"

☐ Update chart canvas id

Example:

id="momentum-mini"
Update Active Date

☐ Set correct start date

Example:

data-start="2026-06-01"
JavaScript Setup
Add Callback Functions

☐ Add total callback

Example:

function handleMomentum(d) {
  renderTotal(d, "momentum");
}

☐ Add history callback

Example:

function handleMomentumHistory(d) {
  renderCard(d, "Total", "momentum");
}
Add Loaders

☐ Add main loader

Example:

loadSheet("Momentum June 01", "handleMomentum");

☐ Add history loader

Example:

loadSheet(
  "Momentum June 01 History",
  "handleMomentumHistory"
);
Prefix Matching Check

These MUST match exactly:

☐ momentum-total
☐ momentum-mini
☐ "momentum"
☐ handleMomentum
☐ handleMomentumHistory

Final Testing
Homepage

☐ Card appears
☐ Total loads
☐ Chart loads
☐ Daily % works
☐ Portfolio % works
☐ Share button works
☐ Active days works

Portfolio Page

☐ Table loads
☐ Charts load
☐ Totals correct
☐ TradingView widgets work
☐ Mobile layout works

Common Problems
Card shows $--

☐ Check sheet name spelling
☐ Check callback names
☐ Check matching prefixes

Chart missing

☐ Check canvas id
☐ Check history sheet exists
☐ Check “Total” column exists

Share button broken

☐ Check:

data-link="momentum-june01.html"
GitHub Deployment

☐ Save files
☐ Commit changes
☐ Push to GitHub
☐ Wait 1–2 minutes for Pages refresh

Recommended Naming Convention
Item	Example
HTML file	breakout-june15.html
Sheet	Breakout June 15
History Sheet	Breakout June 15 History
Prefix	breakout
