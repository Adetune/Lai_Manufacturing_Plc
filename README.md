# Lai_Manufacturing_Plc

![excel-to-powerbi-animated-diagram](assets/images/source.png)



# Table of contents 

- [Objective](#objective)
- [Data Source](#data-source)
- [Stages](#stages)
- [Design](#design)
  - [Mockup](#mockup)
  - [Tools](#tools)
- [Development](#development)
  - [Pseudocode](#pseudocode)
  - [Data Exploration](#data-exploration)
  - [Data Cleaning](#data-cleaning)
  - [Transform the Data](#transform-the-data)
  - [Create the SQL View](#create-the-sql-view)
- [Testing](#testing)
  - [Data Quality Tests](#data-quality-tests)
- [Visualization](#visualization)
  - [Results](#results)
  - [DAX Measures](#dax-measures)
- [Analysis](#analysis)
  - [Findings](#findings)
  - [Validation](#validation)
  - [Discovery](#discovery)
- [Recommendations](#recommendations)
  - [Potential ROI](#potential-roi)
  - [Potential Courses of Actions](#potential-courses-of-actions)
    

# Analysing and visualizing data in real time for operational efficiency in Lai Manufacturing Plc
This project involved gaining hands-on experience with Power BI to enhance operational efficiency in a manufacturing company. My role encompassed collecting, transforming, and analysing data to identify areas for improvement. Using Power BI, I created interactive, real-time dashboards and reports that provided actionable insights to decision-makers, demonstrating the tool's capacity to drive significant business enhancements through data-driven analysis.
Key learning points
Drill Through and Tooltips
Data Modelling
Refreshing your data using
Power Automate
Creating Date Table
Data Visualization
Writing Complex DAX Measures
Writing Complex DAX Measures

# Continue project
OverviewRationale for the ProjectAim of the ProjectData DescriptionTech StackProject Scope
Business Overview/Problem
The manufacturing landscape is not without its challenges, and Lai Manufacturing Plc understands the intricacies of optimizing processes, enhancing operational efficiency, proactively addressing issues, and mitigating risks. Their journey has not been without its hurdles, including the need for real-time reporting, ensuring top-notch data performance, and simplifying complex reports. Others include:
 
•	A. Production Downtime: The company experiences unexpected equipment breakdowns and maintenance delays, resulting in production downtime and increased costs.	 
•	B. Optimizing Processes: The company grapples with the task of streamlining its manufacturing processes, reducing inefficiencies, and eliminating bottlenecks to improve overall productivity.
•	C. Unmanageable, Unintuitive Reports: The company is burdened with unwieldy and unintuitive reports, hindering decision-making and data-driven initiatives. 
•	D. Inventory Management: Managing raw material inventory levels efficiently is challenging, leading to occasional shortages or overstocking. 
•	E. Supply Chain: Coordination with suppliers and distributors could be improved to reduce lead times and enhance overall supply chain efficiency.

# Rationale for the Project
Operation Analytics refers to the process of collecting, analyzing, and visualizing data from various operational sources within an organization to derive actionable insights and improve overall efficiency. For a complex and multifaceted entity like Lai Manufacturing Plc, where industrial machinery and home appliances are produced, the utilization of Operation Analytics is paramount.
 
Through Operation Analytics, Lai Manufacturing Plc can gain deep insights into its production processes, detect inefficiencies as they occur, and promptly take corrective measures. This proactive approach not only minimizes downtime but also optimizes resource utilization, resulting in substantial cost savings. Additionally, real-time and intuitive reporting allows for immediate identification of quality control issues, enabling rapid response to maintain the company's reputation for excellence.
 
Furthermore, the ability to visualize data in real time provides a holistic view of the entire manufacturing ecosystem. This empowers Lai Manufacturing Plc's leadership to make informed decisions, adapt to market trends swiftly, and respond to customer demands with agility. In an era where customer expectations evolve rapidly, the ability to customize production and product lines in real time is a game-changer.
Aim of the Project
 
# The primary goal of this project is to harness the power of real-time data analysis to overcome the business challenges and drive operational efficiency and improvements at Lai Manufacturing Plc. The project aims include:
 
•	A. Process Optimization: Implement data-driven process optimization strategies to identify and eliminate bottlenecks and inefficiencies in manufacturing operations. 
•	B. Intuitive Dashboards: Create intuitive and user-friendly data visualization dashboards that empower decision-makers at all levels with actionable insights. 
•	C. Answer crucial questions relating to business using data analysis, such as; Product Performance Analysis (Which products have consistently high production quantities and sales over time?), Quality Metrics Analysis (What is the overall trend in product quality, and has it improved or deteriorated over time?), Supplier Performance Analysis (Which suppliers have the shortest lead times and which ones may need closer monitoring or adjustments in our procurement processes?), Maintenance Analysis (What are the most common types of maintenance activities performed?) Employee Performance Analysis (Which employees consistently achieve the highest performance metrics?) Downtime Events Analysis (What are the most common reasons for downtime events, and can we prioritize efforts to address the most impactful issues?)
Data Description
 
# Dataset of 1000 rows will be extracted from Lai manufacturing Plc database. This dataset will be analyzed to understand the pain point of the business. The attributes include:
 
•	✓ Operations_ID:  A unique identifier for each operation or record in the dataset.
•	✓ Product_ID: A unique identifier for each product in the dataset. It associates each operation with a specific product.
•	✓ Product_Name: The name of the product associated with the operation.
•	✓ Product_Category: The category to which the product belongs (e.g., Home Appliances or Industrial Machinery).
•	✓ Production_Date: The date on which the operation or production occurred.
•	✓ Production_Quantity: The quantity of the product produced during the operation.
•	✓ Quality_Metrics: A measurement or assessment of the quality of the product produced during the operation. It may indicate whether the product "Passed," "Failed," or falls "In Between" quality standards.
•	✓ Quantity_in_Stock: The quantity of the product available in stock after the operation.
•	✓ Quantity_Sold: The quantity of the product that has been sold after the operation.
•	✓ Supplier_ID: A unique identifier for the supplier associated with the operation.
•	✓ Supplier_Name: The name of the supplier that provided materials or components for the production.
•	✓ Lead_Time: The time it takes for the supplier to deliver materials or components to support the operation.
•	✓ Employee_ID: A unique identifier for the employee involved in the operation.
•	✓ Employee_Name: The name of the employee responsible for the operation.
•	✓ Shift_Information: The shift during which the operation occurred. It can be "Morning Shift," "Afternoon Shift," "Evening Shift," or "Night Shift."
•	✓ Maintenance_Type: The type of maintenance carried out during or after the operation, which can be "Routine Maintenance" or "Repairs."
•	✓ Downtime_Duration: The duration of downtime experienced during the operation, indicating the time the operation was not productive.
•	✓ Energy_Consumption_Data: Data representing the energy consumed during the operation.
•	✓ Production_Time: The time it took to complete the operation or production.
•	✓ Downtime_Events: The number of downtime events that occurred during the operation.
•	✓ Employee_Rating: The rating or performance assessment of the employee involved in the operation, typically on a scale from 1 to 5.
•	✓ Downtime_Reason: The reason for any downtime experienced during the operation. Possible reasons may include "Material Shortage," "Technical Issues," or "Human Error."
Tech Stack
 
Power BI: A data visualization and business intelligence tool that aids in analysis by allowing users to transform raw data into meaningful insights and interactive reports. It helps extract data from sources, enable data exploration,  perform data modeling, and create visually engaging dashboards and reports.
 
# Project Scope
A. Data Importation: Lai Manufacturing Plc. data is imported into Power BI environment.

B. Data Modelling:  Data is modelled in power bi

C. Data Exploration &Analysis: The dataset is explored and analyzed to find trends, patterns, anomalies.
 
D. Data Visualization: The dataset is visualized in form of dashboard, reports and sent to the stakeholders for effective decision-making.

   
# Insights & Recommendation
 Sarah Llyod has produced and sold the highest quantity of products making her the most active employee. Victor Hernandez is the employee with the least produced and sold product
August experience an increase in lead time rate by suppliers and industrial mixer happens to be the product with the most lead time.
Industrial mixers has the highest rate of failed metrics by 23.7%  and also takes the most production time, followed by air conditioners while refrigerator was the lowest by 15.6%
The company produces a lot more than what gets sold, that is, quantity is stock is always more than sold quantity. May, July & September had more quantity sold than in stock, but there is still a huge difference between what was sold or in stock and what was produced. The company is advised to look into its Sales department/team to investigate what the underlining factors could be.
Diesel generator has the highest number of downtime events, followed by industrial mixer. This somewhat aligns with the earlier observation where industrial mixer also had the highest failure rate in quality checks.
Routine maintenance saw an increase in August and a decline in September. There has been a steady increase in repairs since June. 
Product turnover rate has varied throughout the months but industrial mixer was the most sold product.
A significant number of products have passed the quality check, However, a notable portion of products failed the quality check with industrial mixer leading the pack. Further analysis suggest that July had the month with the least pass and the most failed metrics.
Amber Powell is the highest performing employee with an average rating of 3.2 out of 5, but this rating is not consistent with employees output and performance.
A substantial portion of employees has an average rating, suggesting that most employees are performing less than expected with the huge presence of employees with lower ratings (1, 2 and 3). suggests that there might be performance or training issues that need addressing.
Based on the analysis of suppliers, it was evident that various products were associated with varying lead times from the suppliers.
Material inadequacy was the most reason for downtime. This means the company should make sure they optimize their supply chain by sticking with suppliers with short lead time for certain products they supply, instead of they supplying every product. 


# RECOMMENDATION
## On Employees 

Training and Development: Invest in training and development programs to enhance employees' skills and knowledge. Well-trained employees are more likely to perform efficiently.
Team Collaboration: Foster a collaborative work environment where team members support each other. Encourage knowledge sharing and cross-functional cooperation.
Incentive Programs: Introduce incentive programs that reward individuals and teams for meeting or exceeding production targets. Incentives can be financial or non-financial, such as recognition.
Process Improvement: Continuously assess and improve production processes. Involve employees in identifying bottlenecks and suggesting process enhancements.
Communication: Maintain open and transparent communication channels. Encourage employees to share their insights and concerns related to production.
 Working Shift: The management is advised to make the working shift more balanced.


## For product performance and to ward off any inconsistences, some strategies may be useful:

Diversify product Portfolio to reduce dependence on some products. It can help mitigate the impact of fluctuations in individual product performance. 
Seasonal Adjustments: If the decline in September is a recurring pattern, plan for seasonal adjustments in production and sales strategies. For example, increase marketing efforts before the decline period or offer promotions to boost sales during this time.
Inventory Management: Optimize inventory management to avoid overstocking products with declining sales. Implement just-in-time inventory practices to reduce carrying costs.


## To address the fluctuations in product quality metrics and work towards improving overall product quality over time, here are some recommendations:

Root Cause Analysis: Conduct a thorough root cause analysis to identify the specific reasons behind quality issues during the months when metrics were less favorable. This will help pinpoint the areas that need improvement.
Quality Control Measures: Implement robust quality control measures at various stages of the production process. This can include stricter quality checks, inspections, and adherence to quality standards.
Employee Training: Invest in training programs for employees involved in the production process. Ensure that they are well-equipped with the skills and knowledge needed to maintain high-quality standards.


On suppliers, assign the suppliers with the shortest lead times to manage specific products rather than distributing product orders among all suppliers.

## On maintenance, the company is advised to have:

Maintenance Schedule Optimization: Review and optimize the routine maintenance schedule to ensure that it is efficient and minimizes disruption to production. Identify opportunities to consolidate or streamline maintenance activities.
Predictive Maintenance: Implement predictive maintenance techniques, such as condition-based monitoring and sensor data analysis, to reduce the need for routine maintenance. Predictive maintenance can help identify issues before they lead to equipment failure.
Maintenance Automation: Explore automation solutions that can perform routine maintenance tasks more efficiently and with minimal human intervention. Automation can save time and reduce labor costs.
Maintenance Planning: Enhance maintenance planning by aligning it with production schedules. Ensure that routine maintenance is scheduled during periods of lower production demand to minimize disruption.


