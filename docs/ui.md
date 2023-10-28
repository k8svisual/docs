This software, an Excel spreadsheet, has several tabs that will be used to enter and maintain data along with viewing the results of the generated plan.  On the tabs are several icons that aid with navigation and usage.  The following provides information about the tabs and icons contained in this software.

When Retirement Planner is opened a __default__ set of tabs are shown in the spreadsheet. Clicking any of the tabs will navigate to the selected tab.

![DefaultTabs](images/allTabs.png){width=700}

Other __optional__ tabs are shown when a specifc function is selected. The optional tab will be closed when using the navigation return arrow icon (see Common Icons below).  If the navigation return arrow is not used the tab will remain open.  When the software is stopped and re-started all optional tabs will be closed.  

[Tab details](#tab-details) - (click this link to jump to this location)

??? note "Third category of tabs"

    A third category of,  __developer tabs__, is only available if the Developer menu option of Microsoft &reg; Excel is enabled.  Tabs can only be viewed if the Visual Basic feature has been selected.  These tabs are used internallly by the software and do not require any user entry of data. Details for how to enable the Developer menu option are out of scope for this document and not provided.  

<br>

View the icons that aid with navigation and usage.  Many of the optional tabs are only available by clicking one of these icons.  

[Common Icons](#common-ui-icons) - (click this link to jump to this location)


### Red triangles

![RedTag](images/allRedTagInformation.png){align="left" width="400"}

A brief description of a cell/field is available if a small red triangle in shown in the upper right-hand corner.  Place the mouse pointer on the red triangle to view the description.   

<br>

<hr style="border:1px solid green">

## Tab details

A description for each tab defined in this software is available in one of two categories: a) __Default tabs__ or, b) __Optional tabs__.  Select (click) the tab category then select (click) the tab name to scroll to the available information.  


=== "Default tabs"

    * [Assets](#assets)
    * [Budget](#budget)  
    * [Home](#home)  
    * [Income](#income)
    * [Individuals](#individuals)  
    * [Overview](#overview)  
    * [Retire](#retire) 
    * [Useful Info](#useful-info)
    * [Welcome](#home)  


=== "Optional tabs"
    
    * [COLACPI](#colacpi) 
    * [Calculators](#calculators)
    * [EData](#edata)
    * [Export](#export)
    * [Housing](#housing)
    * [IRMAA](#irmaa)
    * [ImportMsg](#importmsg)
    * [Investments](#investments)
    * [LifeTables](#lifetables)
    * [Med-Insur](#med-insur)
    * [Notes](#notes)
    * [RMD](#rmd)
    * [RMD Table](#rmd-table)
    * [Rental](#rental)
    * [Settings](#settings)
    * [SS Estimator](#ss-estimator)
    * [TaxRates](#taxrates)
    * [TaxTables](#taxtables)
    * [Vehicle](#vehicle)

<hr style="border:1px solid green">

## Default tabs

---

### Assets  

Provides the ability to define multiple types of assets. The asset categories available are cash, housing, vehicles, investments, and rental.  The combined total dollar amounts for these categories is shown in the upper portion of this tab.  Cash assets are included to assist in providing a comprehensive picture of all assets.  The dollar amount in the cash category is not utilized when creating the retirement plan.  

The other four categories provide financial data for the retirement plan along with links to optional tabs.  Use the pencil or eyeball icons associated with each category to navigate to the associated optional tab.

![Home](images/assetsBreakout.png){width=500}

<br>

The value entered in the Payment column for Vehicles and Housing assets is used to populate information for the associated tabs and sections.  

The Housing category provides for the entry of the payment frequency while the Vehicle category assumes payments are monthly.  

If a house is owned enter the appropriate information. If the house has no mortgage, ensure the 'Payment' and 'Payment Frequency' fields are zero.  The 'Current Value' field will be used as the basis to calculate future value of your home.  This future value is calculated using the value provided in the 'Annual Appreciation Rate' field.  

To enter additional data for each category, e.g., budget, sale date, etc. click the pencil for the section to open the associated tab.

Investments e.g., IRA, 401K, stocks, etc. information should be entered in this section.  The Monthly Contribution column is used to indicate the amount of additional monies that will be added to the investment each month.  The columns Before or After tax and Investment Owner are required and used in calculating any IRS Required Minimum Distribution (RMD) as needed. Any investment that does not have the Before-tax or After-tax value set will be considered after tax investments.

All investments with a value in the column Category Item ID will be included in the beginning balance of investments.  A blank Category Item ID will cause the line item to __NOT__ be included in the current value of all assets and will __NOT__ be included when creating the retirement plan.

Two rental properties can be defined.  If provided on the Assets tab the pencil icon for this section will need to be clicked to open the Rental tab and define the necessary data for each the property if needed.


The following are messages that can occur on the Assets tab.

![AssetsMsg01](/images/assetsMessageBeforeAfter.png?raw=true){width="400" align="right"}
The Before or After tax value for one or more investments is not properly defined. Select a new value from the drop-down for the field.

![AssetsMsg02](/images/assetsMessageOwnerCannotBeJoint.png?raw=true){width="400" align="right"}
A Before tax investment cannot have an owner of Joint.  Select a new value from the drop-down for the field.

![AssetsMsg03](/images/assetsMessageOwnerNotSet.png?raw=true){width="400" align="right"}
An investment owner is not set for one or more investments.  Select a new value from the drop-down for the field.

![AssetsMsg04](/images/assetsMessageZeroDollars.png?raw=true){width="400" align="right"}
One or more investments have a zero dollar amount and a Category Item ID defined. Provide a dollar amount to include the investment. Or to exclude the investment remove the value for the Category Item ID.  Blank Category Item ID investments my have a dollar amount.

![AssetsMsg05](/images/assetsMessageFirstRentalZero.png?raw=true){width="400" align="right"}
The first rental property has reported income but the value for the property is zero.  Either provide a property value and/or edit the property on the Rental tab to remove the income.

![AssetsMsg05](/images/assetsMessageSecondRentalZero.png?raw=true){width="400" align="right"}
The second rental property has reported income but the value for the property is zero.  Either provide a property value and/or edit the property on the Rental tab to remove the income.

<br>



<hr style="border-top: 1px solid green">


### Budget  

Enter budget data for multiple categories with detailed itemized entries.  Each detailed budget item can indicate frequency, dollar amount, whether impacted by inflation, and whether the budget item is required or optional (discretionary).  

| Column | Valid value(s) | Description |
| :--- | :--- | :--- |
| Description | Any value | Enter a description for the line item of this category. |
| Expense Amount | $0 to $100,000 | The positive dollar amount of the expense for the defined frequency. |
| Annual Freq. | 0 - 366 | The number of times per year this expense occurs. |
| Inflation Applies | Y / N | If Y then this expense will be increased by the defined annual inflation rate. N indicates this line item is not impacted by inflation. |
| Optional or Required | Optional / Required | Values are used to calculate the defined category for chart on Home tab. |
| (+/-) Monthly Adjust at Retirement | -$100,000 to $100,000 | A negative or positive dollar amount that will be used to adjust the beginning budget at retirement start year. |

For Housing, Medical Insurance, and Transportation categories the pencil icon enables entry of budget information for the category.  Click the pencil icon to the left of the associated section title to enter the budget information.

The eyeball icon in the upper portion is used to toggle the viewing of three columns of information.  These columns are:

* (+/-) Monthly Adjust at Retirement - A positive or negative dollar amount to adjust the line item at retirement start year.
* Projected Retirement Monthly $ - The monthly amount for this line item at retirement.
* Projected Retirement Annual $ - The annual amount for this line item at retirement. 

A red text message in the upper portion of the screen will be displayed if any line item has a value in the column labeled (+/-) Monthly Adjust at Retirement.  The following is the message that is shown.  The message is informational only and no action is necessary.

<p align="center">
  <img src="/images/adjustmentMessage.png?raw=true" width="500">
</p>

The annual inflation rate that is entered on the Home or Retire tabs is used to calculate the budget for the retirement start year.  This inflation adjusted budget amount will be used as the starting budget when the retirement plan is generated.

<hr style="border-top: 1px solid green">

### Home

A collection of graphs and a single report can be viewed on this tab to aid in understanding the generated retirement plan.  The graphs and report are: 

| Icon | Chart/Report | Description |
| --- | :--- | :--- |
| ![Lifetime](images/graphLifetime.png){width=40} | Lifetime Investments & Assets | A stacked bar chart for each associated item from the current year to age 100 of the youngest of the individuals defined on the Individuals tab.  If needed this chart includes a line for Before Tax, After Tax, Home, Rental 1, and Rental 2. |
| ![30YearFin](images/graph30Financial.png){width=40} | 30 Year Financial | From the first year of retirement chart 30 years of financials via a line chart.  Each category of financials is shown as a separate line on the chart. |
| ![30YearIncome](images/graph30Income.png){width=40} | 30 Year Income | Starting with the current year chart income for the next 30 years as a stacked bar chart. Each source from the Income tab is shown in this chart. |
| ![BudgetCurrFuture](images/graphBudgetCurrentFuture.png){width=40} | Budget Current & Future | One or two pie charts providing the breakout of budget categories for the current & future budgets. If retirement has already started the second pie chart, future budget, will not be shown. Another pie chart provides the breakout of Required, Optional, and First Year Additional budget needs. |
| ![30BudgetTrend](images/graph30Budget.png){width=40} | 30 Year Budget Trend | The line chart is from the first year of retirement charting 30 years of budget needs. The second chart is any additional withdrawal amounts as defined on the Retire tab in the columns 1) Single Year Monthly Budget Adj. (+/-) and 2) Multi-year Monthly Budget Adj. (+/-) for 30 years. |
| ![30YearHomeRental](images/graph30HomeRental.png){width=40} | 30 Year Home & Rentals | From the current year chart the appreciation of the home and rental properties if defined. |
| ![ChecklistReport](images/graphChecklistReport.png){width=40} | Checklist Report | Create the checklist report to review and identify any possible concerns or issues with the entered information.  |




![UpDown](/images/iconChevronUpAndDown.png?raw=true){width="100" align="right"}

Modifying the control points 1) Average Rate of Return, 2) Annual Inflation Rate, and 3) Retirement Year by using the appropriate green or red chevron icons.  Once these icons are pressed it will trigger the need to re-calculate the retirement plan.  Start the re-calculation of the retirement plan by pressing the green calculator icon.   

<br>

![PressCalculator](/images/greenCalculator.png?raw=true){width="40" align="right"}

Pressing the calculator icon will start the process to create the updated plan.  During the creation of the plan there will be a message indicating with row of the plan is being processed.  The following table of messages provides examples of the expected messages.

<br>


![HomeNav](/images/homeGreenNavButtons.png?raw=true){width=100 align=right}

Navigation to the other default tabs can be performed by using the left-hand navigation buttons. Clicking a button will navigate to the target tab a shown on the associated button. Returning to this tab can be accomplished by using the green return arrow in the upper left-hand corner of the target tab. 


<br><br><br>


The following informational and warning messages are shown in the upper region of the screen or as a popup message on this tab.  

| Action  | Message and Description |
| :-- | :-- | 
| Press green calculator icon | ![PressCalculator](/images/homePressCalculator.png?raw=true){width="300"} <br> Once changes are made to any of the three control points the user will be informed the green calculator icon needs to be pressed to create an updated retirement plan. |
| No action, information only | ![UpdatingRow](/images/homeRowMessage.png?raw=true){width="125"} <br> Which row of the retirement plan that is being processed.  If all rows are successfully processed the message will be cleared from the screen. |
| Click associated chart or report icon | ![UpdatingRow](/images/homeUpdateChart.png?raw=true){width="500"} <br> This message will be shown at the top of the screen is the current chart on this Home tab is possibly out of sync with other financial data.  The current chart name is shown in the upper right-hand portion of the tab.  Press the associated icon for the current chart or report to update the data and remove the warning message. |
| Press OK button | ![UpdatingRow](/images/homeCalculationsStopped.png?raw=true){width="175"} <br> This message will be shown if there are insufficient funds in the investments to span the forty year retirement plan.  This message will be displayed to indicate the calculations have been stopped.  |
| Press OK button | ![YearNotSupported](/images/homeYearNotSupported.png?raw=true){width="175"} <br> An attempt to decrease the retirement year earlier than the current year has occurred. The retirement year cannot be earlier than the current year.  The retirement year value will not be changed and will be set to the current year. |

<br>


<hr style="border-top: 1px solid green">

### Income  

Define estimated or actual incomes that are currently being received or expected to be received during retirement. Incomes can include Social Security, Railroad Retirement, Government, Teacher pension, qualified pensions, annuities, rental, employment, and one-time annual supplementals.  The entry fields for each source are:

| Field name | Valid value | Description |
| :--- | :--- | :--- |
| Source name | Any value | A value that helps identify the source of income. |
| Monthly Amt | $0 - $100,000 |The monthly dollar amount of income that will be received.  Entered as a whole dollar amount without cents. |
| Year to start | 1900 - 2300 | The year the income will start being received. |
| Year to stop | 1900 - 2300 | The year the income will stop being received. |
| COLA / Pay raise | 0% - 100% | An estimated annual percentage of COLA (Cost of Living Adjustment) or pay increase. |
| % Taxable | 0% - 100% | What percent of the income is subject to income tax.  Example: Social Security benefits are not taxed at 100%.  The benefit is taxed at zero, 50%, or 85% based on total income. |

Two additional incomes can be defined.  These are Supplemental and Rental.  Supplemental income provides the ability to add a one-time annual income such as the sale of a car, and inheritance, etc.  Rental income a calculated amount and only shown if Rental property is defined on the Asset and Rental tabs.    


!!! Info 

    Consider using the Social Security Estimator to help determine what amounts may be appropriate to enter for Social Security.

<hr style="border-top: 1px solid green">


### Individuals  

Retirement planner supports defining or or two individuals.  When defining two individuals the age of the youngest is used to calculate the maximum year, age 100, for the Lifetime Investments & Assets chart on the Home tab.  

Enter data for one or two individuals.  The data consists of name, date of birth, hopeful retirement date, a target retirement year, and tax filing status and state.  

The name field is only used to help identify and is not required to be the actual name of the individual. 

The year entered in the Date of birth will be used to calculate the individuals age in a specific year.  

The hopeful retirement date is only used to calculate the values shown on this tab for the fields: months and days till retirement. 

The Retirement Planning Year will be used as the start year for calculations regarding data for retirement.  

![TaxTables](/images/updateTaxesButton.png?raw=true){width="200" align="right"}

The tax filing status and state drop down fields are used to define the proper income tax tables.  Once selected be sure to click the Update tax tables button.  This will create the formulas based on the selected tax tables.  Clicking this button will also remove the following warning message.

![TaxTables](/images/taxTableMessage.png?raw=true){width="400" align="right"}

This warning message will be shown if the selected tax status and state do not match the tables loaded for calculations. 

<br>
![IndividualMsg01](/images/individualsMessage01.png?raw=true){width="400" align="right"}

Individual two has been defined and no individual one is defined. Use the individual one entry fields if there is only one person defined in the plan.

<br>

![IndividualMsg02](/images/individualsMessage02.png?raw=true){width="400" align="right"}

No date of birth has been entered for individual one.  The field is required.

<br>

![IndividualMsg03](/images/individualsMessage03.png?raw=true){width="400" align="right"}

Provide a name for individual one.  This name will be shown on other tabs.

<br>

![IndividualMsg04](/images/individualsMessage04.png?raw=true){width="400" align="right"}

Provide a name for individual one.  This name will be shown on other tabs.

<br>

![IndividualMsg05](/images/individualsMessage05.png?raw=true){width="400" align="right"}

No date of birth has been entered for individual two.  The field is required if a second person is to be defined for the plan.

<br>
<hr style="border-top: 1px solid green">



### Overview

Provides general information about Retirement Planner, access to scenarios, how to upgrade to a new version of the software, and supports export and import of user entered data.  

<hr style="border-top: 1px solid green">



### Retire  

View the created the retirement plan spanning forty years.  All views provide individual(s) information and the Investment Balance in the left portion of the tab. Varying amounts of data are shown with the other views. Toggle the two eyeball icons on the left-hand side to view or hide data detail information.  Scroll up and down and left and right is necessary to view the additional detail information.  

The column Annual withdrawal from Investments is a calculated withdrawal amount is either the amount needed to meet budget requirements or that amount plus any additional amount to meet the IRS Required Minimum Deduction (RMD). 

The column titled RMD Event is used to indicate if RMD supplemental withdrawal has occurred.  Click the eyeball icon in the column title to view detail information for the event.

Pressing the lower eyeball on the left-hand side of the screen will toggle the viewing of significant amounts of data. Scroll right to view the data.  The data is grouped by colored headings.  These groupings are a) Budget Related, Housing Related, Combined After/Before, After Tax, Before Tax, and Validation Checking.  The After Tax grouping is where any amounts reinvested from RMD calculations is shown.  Column titles in each section identify the column values.



Three entry fields for each year of the plan may be utilized.  These fields are:

| Field | Valid value | Description / Use |
| :--- | :--- | :--- |
| Single Year Monthly Budget Adj. (+/-) | +$10,000 to -$10,000 | A positive or negative dollar amount that will be used to adjust the monthly budget for the year in which the value is entered. |
| Multi-year Monthly Budget Adj. (+/-) | +$10,000 to -$10,000 | A positive or negative dollar amount that will be used to adjust the monthly budget for the year in which the value is entered and all subsequent years. |
| Comments | Any value | Enter any comment value. | 

The fields a) Annual inflation rate %, b) Avg. rate of return %, and c) Retirement year may be modified with the use of the associated green up and red down chevrons.  If these fields are modified the message informing the user to press the 
calculator will be displayed.


The following messages and popup messages can occur on the Retire tab:


![ExceedsFunding](/images/retireExceedsNeedsMessage.png?raw=true){width="150" align=left}

Income monies for one or more years exceed the budget needs resulting in a negative withdrawal amount. 


<br><br><br>

![PressCalculator](/images/retirePressCalculator.png?raw=true){width="175" align=left}

The green calculator icon/button needs to be pressed to update all financials and invoke the create plan process.  This message will be cleared once processing is completed.


<br>

![UpdatingRow](/images/retireRowMessage.png?raw=true){width="175" align=left}

Current row of the plan that is being processed.  If all rows are successfully processed the message will be cleared from the screen.

<br>

![StoppedCalculations](/images/retireCalculationsStopped.png?raw=true){width="175" align=left}

If there are insufficient funds in the investments to span the forty years a message will be displayed to indicate the calculations have been stopped.  

<br><br><br>

![YearNotSupported](/images/retireYearNotSupported.png?raw=true){width="175" align=left}

Pressing the red down chevron for the Retirement year field is attempting to decrease the retirement year earlier than the current year. The retirement year cannot be earlier than the current year.  The retirement year value will not be changed and will be set to the current year.

<br><br>

<hr style="border-top: 1px solid green">


    
### Useful Info

Reports and Calculators are provided to aid in understanding factors related to creating a robust retirement plan.

<hr style="border-top: 1px solid green">



### Welcome

General information regarding the Retirement Planning software.

<hr style="border-top: 1px solid green">



## Optional tabs

<hr style="border-top: 1px solid green">



### COLACPI

Provides Social Security Cost of Living Adjustment (COLA) and Consumer Price Index (CPI) information. 

The data in the CPI table is also used to calculate the average inflation rate for the last ten years.  The calculated value is then used to determine if the defined inflation rate for the retirement is more than one percent more or less.  If the defined inflation rate is more or less than one percent difference this difference is reported when creating the Checklist Report from the Home tab.  

These tables can be updated by the user.  Use of the lock in the upper portion of the screen to allow editing.

This tab is accessed from Useful Info tab.

<hr style="border-top: 1px solid green">



### Calculators

Multiple calculators for use in understanding the following:

    1) Present value  
    2) Future value  
    3) Mortgage Payment  
    4) Vehicle Payment  
    5) Investment Fee Impact  
    6) Rate of Return (Overall & Annual)  

This tab is accessed from Useful Info tab.

<hr style="border-top: 1px solid green">
   
    
### EData

A tab used to aid with importing or exporting data for this software.  The data in this tab has been obtained from user entered data in this spread sheet, "Retirement Planner".  The data can be imported to a newer version of "Retirement Planner".  Copy the data in rows 5 to the last row containing data.  Open the newest version of "Retirement Planner", select "Welcome", scroll to the bottom of the tab and press the button "Open EData".  Remove the existing data if any exists and paste the copied data into the spreadsheet.  Close the EData tab in the latest version of "Retirement Planner" by pressing the return arrow.  Once closed you should be in the "Welcome" tab again, press the "Import Data" button.  It will take several seconds to multiple minutes import the data.  

This tab is accessed from the Overview tab.

<hr style="border-top: 1px solid green">
    

### Housing

Enter your housing related information in this tab.  Expenses for housing are entered in the top portion of this tab.  The expense data is copied to the HOUSING section of the Budget tab as read only data.

If you own a home be sure enter the related information.  If you plan to sell your home in the future also enter that related information.

Access this tab from the following locations: 

1) The HOUSING section of the Budget tab.
2) The HOUSING section of the Assets tab.  

<hr style="border-top: 1px solid green">
   

### IRMAA

Information for Medicare Income Related Monthly Adjustment Amount (IRMAA).  The income related monthly adjustment amount (IRMAA) sliding scale is a set of statutory percentage-based tables used to adjust Medicare Part B and Part D prescription drug coverage premiums. The higher the beneficiary's range of modified adjusted gross income (MAGI), the higher the IRMAA. 

This tables can be updated by the user.  Use of the lock in the upper portion of the screen to allow editing.

This tab is accessed from Useful Info tab.

<hr style="border-top: 1px solid green">


### ImportMsg

Provides status information once the 'Import Data' button from the Overview tab has been pressed.  All status lines will not be shown when the import process is started.  Status data will be shown as each tab of import data is processed.  The following image is like what will be show.

![ImportMsg](images/importMsg.png)

<hr style="border-top: 1px solid green">


### Investments

This tab provides the estimated annual changes in each investment that is defined in the INVESTMENTS section of the Assets tab.  The defined target retirement year is indicated by the value '==>' shown in the column titled __Retire target year__.   

![ImportMsg](images/investments.png)

<hr style="border-top: 1px solid green">


### LifeTables

Life expectancy information tables that are available from the Nation Vital Statistics reports.  URL links to the data sources are provided.

This tables can be updated by the user.  Use of the lock in the upper portion of the screen to allow editing.

This tab is accessed from Useful Info.

<hr style="border-top: 1px solid green">


### Med-Insur

Detailed medical expense information for one or two individuals.  The upper portion of the tab is the combined costs from the individual sections in the lower portion of the tab.  The combined expense data is included in the Budget tab.  The medical expenses can only be edited from this tab.  

This tab is accessed by pressing the Pencil icon in the left-hand column of the MED-INSUR section of the Budget tab. 

<hr style="border-top: 1px solid green">


### Notes

User entered notes or comments.  The entered data can be used as needed by the user.  

This tab is accessed from Useful Info.

!!! danger "CAUTION"  
    
    The data entered on the __Notes__ tab will NOT be migrated using the Export data feature from the Overview tab.

<hr style="border-top: 1px solid green">


### RMD

This tab provides the calculated IRS required distribution that must be taken from "BEFORE TAX" investments based on an individual's age.  Calculated amounts to withdrawal are for each individual.

This tab is accessed from the Retire tab by pressing the Eyeball icon in the column titled __RMD Event__.

!!! Info "RMD should be taken seriously" 

    If monies are not taken there is a significant penalty.  There may be a 50 percent excise tax on the amount not distributed as required﻿, according to the IRS.

<hr style="border-top: 1px solid green">


### RMD Table

An RMD is the annual Required Minimum Distribution that you must start taking out of your retirement account after you reach age 70 or 72. Refer to the trigger date for when the age moves from 70 to 72.  The amount is determined by the fair market value of your IRAs at the end of the previous year, factored by your age and life expectancy.  The IRS penalty for not taking an RMD, or for taking less than the required amount, is steep: 50% of the amount not taken on time. The deadline to take your first RMD is normally April 1 of the year after you turn 72, and December 31 each following year.

This table can be updated by the user.  Use of the lock in the upper portion of the screen to allow editing.

This tab is accessed from Useful Info.

<hr style="border-top: 1px solid green">


### Rental

If you own rental property this tab is used to enter related information.  The information is used to calculate rental income and appreciation of rental property.  The 'Combined yearly Total' amount is transferred to the Rental section of the Income tab. Rental property is included in the calculation of total assets.

This tab is accessed by pressing the Pencil icon in the upper left portion of the Income tab or the Rental section of the Assets tab.  


<hr style="border-top: 1px solid green">

### Settings

This tab provides the ability for the user to configure options and upgrade the software. Feature are: 

* Modify the default first screen shown when starting the software. Options are the Welcome or Home tabs.

* Modify the displaying of the informational message regarding the green calculator.

* Modify the screen zoom percentage for all tabs.  This will reset the zoom percentage for all tabs, default, optional, and developer.

* Upgrade the software using an approach that will 1.) save data, 2.) copy data, and 3.) import data.  

This tab is accessed by pressing the green gears in the upper right-hand corner of the Home tab.


<hr style="border-top: 1px solid green">


### SS Estimator

This tab is used to determine an estimated amount of Social Security benefit that will be received.  This estimate requires the user to obtain their Full Retirement Amount (FRA) from the Social Security Administration.  

The calculated amount will use the FRA as the base to determine if the benefit amount should be less or more than the FRA based on the target date to retire.  If a user has not reached the FRA year and month the benefit will be less than the FRA.  If the retirement date is later than the FRA year and month the benefit will be larger.

This amount can then be used as an estimate on the Income tab.

This tab is accessed from the RENTAL section of the Assets tab or from the Income tab by pressing the Pencil icon labeled __Detail 

<hr style="border-top: 1px solid green">


### TaxRates

Income tax rates for Federal, State, County, and City can be defined and then calculated as applicable to your location.  This tab displays the values to be used for the tax calculations.  

From the Income Tax section of the Individuals tab the proper filing status and state can be defined.  Pressing the 'Update tax tables' button is required.  A warning message will be displayed if the tax tables are not updated to match the selected values.

County and City tax table information must be manually entered on this tab.  Entry of either County or City tax rates also requires updating of the tax rates.  No warning message to update the tax tables will be displayed if either the County or City taxes are entered or updated. 

Access this tab from the following locations: 

1) Pressing the Pencil icon in the left column of the Income Tax section of the Individuals tab.  
2) Pressing the Pencil icon in the upper middle portion of the Income tab.

<hr style="border-top: 1px solid green">


### TaxTables

Individual and joint tax rate tables for Federal, state and Washington D.C.  The data from these tables is used to populate the TaxRates tab when the Update tax tables button from the Individuals tab is pressed.

This table can be updated by the user.  Use of the lock in the upper portion of the screen to allow editing.

This tab is accessed from Useful Info tab.

<hr style="border-top: 1px solid green">


### Vehicle

Detailed vehicle expense information for one to four vehicles can be entered in the lower portion of this tab.  The entered amount is the combined amount for all vehicles.  The upper portion of this tab is the individual vehicle information from the VEHICLES section of the Assets tab.  

The combined expense data is included in the Budget tab.  The vehicle expenses can only be edited from this tab.  

Access this tab from the following locations: 

1) Pressing the Pencil icon in the left-hand column of the VEHICLES section of the Assets tab.  
2) Pressing the Pencil icon in the left-hand column of the VEHICLE section of the Budget tab. 

<hr style="border-top: 1px solid green">


## Common UI Icons

The icons below are used on the tabs of this software.  The icons are intended to assist in navigation and use of the software.  

| Icon | Name | Description |
| --- | :--- | :--- |
| ![Decrease](images/iconChevronDown.png){width=30} | Down chevron | Decrease the associated value. |
| ![Increase](images/iconChevronUp.png){width=30} | Down chevron | Increase the associated value.|
| ![Eyeball](images/iconEyeball.png){width=30} | Eyeball | Toggle view or hide associated data. |
| ![Green Gears](images/iconGears.png){width=30} | Green gears | Open the Settings tab.|
| ![Green Calculator](images/iconGreenCalculator.png){width=30} | Green calculator | Invoke the create retirement plan process. |
| ![Home](images/iconHome.png){width=30} | Home | Navigate to the Home tab. |
| ![Lock](images/iconLock.png){width=30} | Lock | Toggle the lock or unlock of the tab to enable editing of the tab.|
| ![Calculators](images/iconMathSigns.png){width=30} | Calculators | Navigate to the calculators tab. |
| ![Notes](images/iconNotes.png){width=30} | Notes | Navigate to the Notes tab. |
| ![Pencil](images/iconPencil.png){width=30} | Pencil | Navigate to the associated tab to view, enter, or update data. |
| ![Report](images/iconReport.png){width=30} | Report | Navigate to the associated report tab. |
| ![Return](images/iconReturn.png){width=30} | Home | Return to the previous tab. |
| ![Home](images/iconHome.png){width=30} | Home | Navigate to the Home tab. |

<hr style="border-top: 1px solid green">

