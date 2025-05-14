# IMPACT-OF-WORKFORCE-REDUCTION-ACROSS-DIFFERENT-SECTORS-OF-THE-TECH-INDUSTRY

![image_fx_ (1)](https://github.com/user-attachments/assets/1e5d470f-c62a-48f3-bbfe-bc1f0fcc544f)

## **PROJECT OVERVIEW**

**What If Data Could Help Us Understand Who’s Getting Laid Off and Why?**
Meet James, a mid-level developer laid off from a fast-growing startup. He’s not alone. Over the past year, thousands of tech workers like James, from engineers to product managers, have found themselves jobless overnight. But what’s really going on behind the scenes?

This project dives into the tech layoffs wave using real data. I wanted to know which companies are letting people go, what stage they’re in, and if certain roles or industries are being hit harder than others. With Power BI, I cleaned, explored, and visualized the patterns to find answers not just for James, but for anyone trying to make sense of the chaos and plan better for the future.

## **DATA STRUCTURE** 
The dataset was provided in an Excel format from 2020 to 2024. It consists of 1,673 rows and 16 columns

## **INDUSTRY TYPE OF DATA** 
This dataset falls under the Tech industry, focusing on analyzing tech layoff patterns across different countries

## **WHO IS THIS ANALYSIS FOR** 
This project is important to stakeholders like HR teams, Tech companies, tech-inclined workers, and industry observers.

## **OBJECTIVES**

The goal of this analysis is to explore key questions surrounding layoffs in the tech industry and provide insights that can help businesses, professionals, and policymakers understand emerging patterns and take proactive steps. Some of the questions addressed in this project include:

1. When are layoffs happening?
Analyze trends over time to identify whether layoffs are increasing, decreasing, or clustering during certain months or economic cycles.
2. Which sectors are most affected?
Explore the Industry Segment (e.g., software, hardware, fintech, AI) to determine which parts of the tech space are experiencing the highest layoff rates.
3. Which companies are cutting the most jobs?
Identify the top companies by number of layoffs and uncover patterns related to company size, total funding raised, or specific industry focus.
4. What strategies can reduce the impact of future layoffs?
Offer recommendations for smarter workforce planning, based on the trends and patterns uncovered in the data.

## **DATA CLEANING STEPS TAKEN**

I opened the dataset in Excel first to scan through it and identify any obvious issues before loading it into Power BI. Here’s what I did:

1.  I used the company ID column to check for duplicate rows. Thankfully, no duplicates were found in the dataset.
2.  Some columns, like Industry and Stage, had cut-off words (e.g., “construc…”, “infrastruc…”). I manually completed these words using Excel’s filter dropdown to ensure clarity and consistency.
3. The 'Money Raised' Column had mixed formatting and missing values. I used Excel’s Text to Columns tool to separate values properly and remove formatting issues that could cause errors in calculations later on.
4. Handled Missing Values:
   - For the Company Size Before Layoffs column, I filled in missing values using the average (3,654), since it had more filled values than blanks.
   - I used formulas to calculate missing values in the Laid Off, Percentage, and Company Size After Layoffs columns based on the available data.
   - For the remaining blanks, I used the average value of that column to fill them in and maintain consistency.
5. Instead of using a general average, I calculated the average money raised for each specific business stage (e.g., Post-IPO = $2,144M) and filled missing values accordingly.
6. After doing the heavy cleaning in Excel, I loaded the data into Power BI's Power Query Editor for further steps.
7. I renamed several columns for clarity and changed data types to ensure accurate calculations (e.g., converting text to numbers where needed).
8.  I used the Trim and Clean functions to remove spaces and unprintable characters from text fields like industry and company stage.
9. Created New Groupings for Better Analysis
10. Once all cleaning steps were completed, I clicked Close & Apply to load the cleaned dataset into my Power BI model for visual exploration.

## **METHODOLOGIES**

To gain better insights from the tech layoff data and make the dashboard more interactive and user-friendly, I used the following Power BI features:

1. Power Query for Cleaning: Most of the data cleaning was done using Power Query for faster processing and better handling of column transformations and calculated fields.
2. Calculated Columns and Custom Columns: I created new fields like Layoff Severity, Company Size Category, and Funding Category using conditional logic. These helped group raw numbers into more useful categories.
3. Charts and Visualizations: I used various charts (bar, column, pie, line) to show:
   - Layoff trends over time 
   - Industry segments most affected
   - Companies with the highest layoffs
   - Distribution of layoffs by business stage and funding size
4. Slicers: I added a Year dropdown slicer that allowed users to quickly switch between different years (or time-based views) using buttons, improving the user experience and visual flow of the report.
5. Drillthrough Page: I created a drillthrough page so users could right-click on a specific company or stage and explore detailed information, like layoff numbers, impact severity, and funding, filtered for that item only.
6. Page Navigator: I used a page navigator to help users easily switch between key views, such as Layoff Overview and Funding Overview, making the report more intuitive to explore

These methods helped ensure the analysis was not only clean and organized but also dynamic, engaging, and easy for stakeholders to interact with.

## **NOTABLE TRENDS AND KEY METRICS**

### **LAYOFFS INSIGHTS**

![Screenshot (450)](https://github.com/user-attachments/assets/f93e8073-943b-40ae-9465-da3d67005e8b)

- Retail companies recorded the highest number of tech layoffs, showing the impact of changing shopping habits and reduced consumer spending.
- Consumer and transportation sectors followed closely behind, as many companies cut jobs to manage costs and stay profitable.
- Amazon, Meta, and Google were among the top companies with large-scale layoffs. These tech giants made workforce cuts to reduce expenses and shift focus to high-growth areas like AI and cloud computing.
- The highest number of layoffs happened in 2023, with January recording the most job cuts. This indicates that companies often restructure or downsize at the beginning of the year.
- A second spike occurred in November, likely due to year-end budget decisions.
- The lowest layoffs occurred in 2021, as companies were still recovering from the pandemic and hiring to rebuild.
- Public companies had the largest share of layoffs, driven by pressure from investors and the need to maintain profitability.
- Private companies recorded fewer layoffs, with many still in growth mode and less exposed to market pressures.
- Large companies led in total layoffs, mainly because of their bigger workforce and higher operational costs.
- Small businesses reported the fewest layoffs, as their teams are already lean and more sensitive to staffing changes.
- The United States had the most layoffs, driven by its large number of tech firms and startups.
- Other top-affected countries included India, Germany, and the United Kingdom, while Sweden had the lowest layoffs among the top five.

### **FUNDING INSIGHTS**

![Screenshot (462)](https://github.com/user-attachments/assets/76688f03-e089-415e-ae8c-628490ff205f)

- Netflix received the highest funding, signaling strong investor confidence in the streaming industry.
- Uber and Meta also secured large investments, driven by their focus on expansion and innovation.
- Cruise and Xerox received significant funding but rely less on external capital, likely due to their established market positions.
- Large companies received the most investor funding, reflecting their strong reputation and stability.
- Enterprise-level companies followed, while medium-sized businesses attracted moderate investment.
- Small companies received the least funding, which limits their growth potential.
- Companies in the exit stage (public or acquired) received the highest funding, indicating investor trust in proven business models.
- Growth-stage businesses also attracted substantial funding, showing investor interest in scaling opportunities.
- Startups and early-stage companies struggled to raise large investments due to higher perceived risks.
- Mature companies received the least new funding, as they are already stable and require less capital for growth.
- Overall funding fluctuated over the years. Initial excitement around digital businesses led to high investments, but caution grew over time, causing a decline in funding activity.
- The United States attracted the most investor funding, reinforcing its position as the global tech hub.
- India ranked second, showing rapid growth and increasing investor interest.
- Germany, Singapore, and the UK also attracted decent funding but remained behind the U.S. and India.

## **DATA-DRIVEN RECOMMENDATIONS ALIGNED TO STAKEHOLDERS, TECH FOUNDERS, WORKERS, AND INVESTORS FROM THIS ANALYSIS**

1. Big tech companies like Amazon, Meta, and Google laid off thousands of workers, even though they were still making billions. It’s time for the tech industry to stop treating people like numbers.
2. They should focus more on reskilling and moving people into new roles instead of laying them off.
   They should keep investing in high-growth areas like AI and cloud computing, but do it with balance.
4. Companies should stop hiring aggressively only to fire later. Many startups do this too, raising money, hiring fast, and then laying off over 70% of their team. It’s not sustainable.
5. Startups should only hire when it makes sense, and founders need to build lean teams from day one.
   Investors should fund companies that treat workers fairly and have a clear, long-term plan.
6. Freelancing, investing, or having a side hustle can help tech workers stay secure, especially with layoffs happening often.
   Big companies still offer more job stability than most startups, so employees need to be smart about where they work.
7. Startups looking for funding should focus on the U.S. and India. They attract the most investor attention.
   For investors, the U.S. is the safest choice, while India offers fast growth and big opportunities.
   Germany, Singapore, and the U.K. are also good for niche markets and solid bets.
8. Since most layoffs happen in January and November, employees should be ready for changes around those months, whether it’s learning new skills or saving more.
   Companies should plan ahead and try other ways to save money before cutting jobs.
9. When funding is good, companies need to save and plan for slow periods.
   When funding drops, they should focus on efficiency and real revenue, not just surviving on investor money.
10. Many big companies laid off workers not because they were failing, but to boost profits.
    Instead of job cuts, they should improve financial planning, automate smarter, and cut unnecessary spending.
11. If you're a worker, upskill regularly and stay updated on what’s trending in your field.
    If you’re a founder, build a solid, lean business that doesn’t depend on constant fundraising.
    If you're an investor, back companies that are smart with money, not just chasing the latest hype.
12. Startups that raise big funds should use them wisely. Focus on long-term growth and innovation, not burning through cash.
    Startups outside the U.S. and India should learn from their models by building stronger ecosystems, solid business models, and earning investor trust.
13. Big companies should find smarter ways to save money without just firing employees.
    Small companies should avoid over-hiring in good times so they don’t struggle when things slow down.

In conclusion, Companies should focus on keeping their employees instead of cutting jobs whenever things get tough. Workers should always keep learning new skills to stay valuable. Founders should build businesses that grow steadily rather than depending too much on investors.
If everyone plays their part, we’ll have fewer layoffs, better job security, and stronger businesses in the long run for everyone in tech. 
If everyone plays their part, we’ll see fewer layoffs, stronger companies, and better job security for everyone in tech.
