# Software-Design-Quality-Assurance
Scenario
Endothon Finance is a loan servicing company specializing in loans for small businesses
wishing to expand or improve their operations. Recent changes to Endothon Finance’s loan
application process necessitated the launch of a new applicant-facing web app. Businesses
applying for a loan through Endothon Finance interact with the web app, experiencing a
streamlined process with customized loan application requirements based on core details
(e.g., business age, industry, number of employees). The information collected during this
process is used by Endothon Finance to construct a loan profile of each business, which is
shared with a list of partnered lending vendors. The automation of both the web app’s logicbased requirements and the dissemination of the loan profile to potential lenders allows
quicker processing of loan applications.
Endothon Finance requires business applicants to provide their previous five years of
financial data to determine qualification status. The web app was intended to request
financial data for the five most recently completed fiscal years of a business, disregarding
the current year. If a business was created less than five years ago, the web app logic
should adjust and instead request the most current years in business and a forecast for the
remaining future years. For example, if a business was established in 2000 and the current
year was 2023, then the web app should request historical financial data from 2018, 2019,
2020, 2021, and 2022. Alternatively, if a business was established in 2020 and the current
year was 2023, then the web app should request historical financial data from 2020, 2021,
and 2022, as well as projected financial data from 2023 and 2024.
An internal ticket has been prioritized due to unexpected results in the new web app. Loan
profiles created by the web app are being returned with the first five fiscal years of financial
data as opposed to the five most recent years. For example, if a business was established in
2000 and the current year was 2023, then the web app is incorrectly requesting historical
financial data from 2000, 2001, 2002, 2003, and 2004. As the software developer, you have
been tasked with providing a software design and quality assurance plan to address the
ticket and ensure expected behavior.
