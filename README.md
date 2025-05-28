This project runs in Excel and RStudio. A rough workflow of the project is, but not entirely, as follows:

1) The all_car_adverts_modified.csv is derived from a much larger data set, 'lightly' modified to remove inconsistent data and unnecessary columns, dated from October 2022, that claims to have about a million entries of car sales from a major UK auto retailer (uknown). This data set can be downloaded here: https://www.kaggle.com/datasets/guanhaopeng/uk-used-car-market/data
2) A postcode lookup table postcodes.csv was taken from https://github.com/academe/UK-Postcodes/blob/master/postcodes.csv, to calculate distances from car seller locations based on average postcode distance, also with the aid of the PostcodesioR R package (https://cran.r-project.org/web/packages/PostcodesioR/PostcodesioR.pdf)
3) CAAS.Rmd is where most calculations, analysis, charts and figures are produced. This .Rmd file was built based on several online sources and some of my own previous work. This .Rmd depends on the two .csv files mentioned, so they need to be in the same work directory. CAAS.Rmd will also need three .csv files which are not directly produced in R, but were partly edited by  hand: vauxhall_parameters_combined.csv, volkswagen_parameters_combined.csv, and audi_parameters_combined.csv. They should also be in the same work directory.
4) finance_solver_data.csv is set up to be run through Excel Solver, to find optimal values for the given MIP problem. Most data in the table was obtained from major bank and credit broker websites, transport and insurance providers, as well as manually calculated. This .csv relies on data outputs from the CAAS.Rmd file, so it should be run during the last stage.

References:

 ▶ Guy Abel.
 Bank of England Fan Charts in R.
 https://guyabel.github.io/fanplot/articles/02_boe.html, 2021.
 ▶ academe.
 UK Postcodes.
 https://github.com/academe/UK-Postcodes/blob/master/postcodes.csv, 2012.
 ▶ Airtasker.
 How much does car transport cost in the UK?
 https://www.airtasker.com/uk/costs/car-transport/cost-to-transport-car/, 2025.
 ▶ APM–ACostE.
 Estimating Guide.
 https://www.apm.org.uk/media/rqgnraf5/estimating-guide-sample-chapter.pdf, 2019.
 ▶ Kausthub Balaji.
 Triangular Distribution.
 https://rpubs.com/pac25/la1, 2023.
 ▶ Bank Underground.
 Car finance: what’s new?
 https://bankunderground.co.uk/2017/08/15/car-finance-whats-new/, 2017.
 ▶ Barclays.
 Car Loans.
 https://www.barclays.co.uk/loans/car-loans/, 2025.
 ▶ Betty.
 Amortization Methods.
 https://rpubs.com/Betty_XG/1153314, 2024.
 ▶ Car Carry.
 UK Vehicle Transportation Cost Map.
 https://www.carcarry.co.uk/auto/how-much-to-transport.php?mode=delivery, 2025.
 ▶ CarFinance 247.
 AFFORD FOCUS: A Definitive Report on the UK’s Used Car Finance Market in 2020.
 https://www.carfinance247.co.uk/downloads/used-car-finance-market-report-2020.pdf, 2020.
 ▶ CarFinance 247.
 Car Finance Calculator.
 https://www.carfinance247.co.uk/car-finance-calculator, 2025.
 ▶ Sayan Chakraborti.
 Used Car Depreciation Analytics.
 https://rpubs.com/SayanChakraborti/usedcaranalytics, 2025.
 ▶ Coding Finance.
 Calculating car loan payments in R.
 https://www.codingfinance.com/post/2018-03-23-car-payment/, 2018.
 ▶ Delivery Quote Compare.
 Delivery Quote Compare.
 https://www.deliveryquotecompare.com/vehicle-delivery/car-transporters, 2025.
 ▶ Eryk Walczak.
 PostcodesioR: API Wrapper Around ’Postcodes.io’.
 https://cran.r-project.org/web/packages/PostcodesioR/PostcodesioR.pdf, 2025.
 ▶ Evolve Relocation.
 What is the cost to move a car.
 https://evolverelocation.co.uk/office-moves/cost-to-move-car/, 2025.
 ▶ GitLab.
 4 ways to use GitLab Issue Boards.
 https://about.gitlab.com/blog/4-ways-to-use-gitlab-issue-boards/, 2018.
 ▶ Grid Reference Finder.
 UK Grid Reference Finder.
 https://gridreferencefinder.com/#, 2025.
 ▶ Guanhao Peng.
 UK Used Car Listing Data.
 https://www.kaggle.com/datasets/guanhaopeng/uk-used-car-market/data, 2022.
 ▶ HSBCUK.
 Car Loans.
 https://www.hsbc.co.uk/loans/products/car-loan/, 2025.
 ▶ Hyndman and Athanasopoulos.
 Forecasting: Principles and Practice (2nd ed.).
 https://otexts.com/fpp2/, 2018.
 ▶ MoneySuperMarket.
 Car Finance Calculator.
 https://www.moneysupermarket.com/loans/car-finance/calculator/, 2025.
 ▶ Jeffrey T. Monroe.
 Business Analytics with R- Chapter 9.
 https://bookdown.org/jeffreytmonroe/business_analytics_with_r7/finance.html, 2024.
 ▶ NimbleFins.
 Average Cost of Cars UK 2025.
 https://www.nimblefins.co.uk/cheap-car-insurance/average-cost-cars-uk#nogo, 2025.
 ▶ Peter Prevos.
 Monte Carlo Cost Estimates: Engineers Throwing Dice.
 https://lucidmanager.org/data-science/monte-carlo-cost-estimates/, 2021.
 ▶ Project-Management.info.
 Three-Point Estimating and PERT Distribution (Cost Time Estimation).
 https://project-management.info/three-point-estimating-pert/, 2025.
 ▶ RAC.
 Temporary Car Insurance.
 https://www.rac.co.uk/insurance/temporary-car-insurance, 2025.
 ▶ Santander UK.
 Car Loans.
 https://www.santander.co.uk/personal/loans/car-loans, 2025.
 ▶ TheAA.
 Vehicle Delivery.
 https://www.theaa.com/cars/vehicle-delivery, 2025.
 ▶ Jakob Theis.
 Used Car Data Analysis.
 https://rpubs.com/JakobTheis/1170433, 2024.
