#
# sql_project2
Group NAME:
61608 Group 3
|
Database name: ha_group_crn61608
## Team Members
1. Cavanaugh, Rory
2. Chadha, Jasmine
3. McNally, Owen
4. Mulnix, Hayden
5. Nguyen, Timmy
## Dataset Description + What it contains
Our dataset shows all the registered electric vehicles within the state of Washington. The columns consist of a VIN code that acts as the primary key of the data set. This VIN number is given to each electric vehicle when registered with the state. Along with that the columns also consist of Consumer locational data (County, City, State, Postal Code), Make, Model, Model Year, Type (battery, hybrid, plug in), and Electric Range (Electric range is the distance an EV can travel on one full charge). 
## Two Questions and Importance
Our first question was "Compare the average electric range and the maximum electric range of the top five brands in each category." We wanted to propose this question and come to a conclusion to combat a scenario like this "Assume you are a perspective consumer of an EV vehicle. You work in Seattle, but you have a long commute through suburban areas. You need to find an EV that has an Electric Range (or gas milledge) that can support your needs." By asking this question, we were able to see if certain brands have different kinds of electrical vechicles for different needs. Moving onto our second question, "Which county in Washington utilizes the most electrical vehicles?" We proposed and researched this quesiton in the scenario of, "Assume you are apart of the environmental planning board for the state of Washington. The board wants to know which counties are utilizing electrical vehicles and why other counties are slower to adopt certain energy initiatives." While we thought this was a little more niche, we also realized that these car brands can use this map to advertise to the counties with the high adoption of electrical vechiles, and conduct research on why some other counties in the state are slow to adapt. 

## Manipulations Appiled to Dataset
For our question one visual, the dataset was filtered to include only the top five EV brands based on average and maximum electric range. Each brand was assigned a unique color for clarity, with Chevrolet highlighted as an example. The bars were sorted in descending order to emphasize the brands with the highest ranges. Additionally, the measure used was changed to show either the average or maximum electric range depending on the chart. Our question two manipulations was to generate the Washington state map visualization. The data was filtered to show only Washington counties and remove any unknown entries. The geographic role for "county" was set to generate a map, and then the map was resized and relabeled by county. A distinct count of VINs was used as the measure, and colors were applied using a reversed orange-blue diverging scale to highlight values. Location mismatches were resolved manually in the geographic role settings to correctly assign counties within the state of Washington.

## Analysis and Results
Our question one analysis consisted of the fact that Jaguar leads in average electric range, offering 193.2 miles across its models, making it the top choice for consumers prioritizing consistency in EV range. Tesla, while not ranked in average range, stands out for its highest maximum range of 337 miles, suggesting at least one of its models is highly optimized. This discrepancy highlights that Tesla offers more variety, possibly with performance or affordability trade-offs in some models. Overall, Jaguar appeals to those seeking reliable range across the board, while Tesla attracts those looking for high-end, feature-rich EVs with standout maximum performance.
<img width="679" alt="Screenshot 2025-04-30 at 9 18 16 PM" src="https://github.com/user-attachments/assets/e20aa68b-0fe7-410e-9e38-584d1ef63d42" />

Our question two analysis consisted of that King County leads Washington in electric vehicle (EV) adoption with 11,751 vehicles, while Garfield County has the fewest at just 3, highlighting stark regional differences in adoption. This data provides a strong foundation for EPB and energy providers to explore what drives adoption in high-density EV counties and how to support underserved areas. Areas with greater EV use could benefit from expanded charging infrastructure, and marketing teams can better target regions with concentrated EV presence. Overall, this analysis can guide strategic investment, resource allocation, and policy planning across the state.
<img width="637" alt="Screenshot 2025-04-30 at 9 20 33 PM" src="https://github.com/user-attachments/assets/f30df82d-7976-4c17-9f5f-7e3011a00160" />



















