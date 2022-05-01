# Housing Rental Analysis for San Francisco
An application with interactive visualizations, and geospatial analysis, to find properties in the San Francisco market that are viable investment opportunities.

## Technologies

- Jupyter notebook
- hvPlot 
- GeoViews

---

## 1.Calculated and Plot the Housing Units per Year

- Used the groupby function to group the data by year. Aggregate the results by the mean of the groups.
- Used the hvplot function to plot the housing_units_by_year DataFrame as a bar chart. Make the x-axis represent the year and the y-axis represent the housing_units.

---

## 2. Calculated and Plot the Average Sale Prices per Square Foot

- Grouped the data by year, and then average the results.
- Created a new DataFrame named prices_square_foot_by_year by filtering out the “housing_units” column. 
- Used hvPlot to plot the prices_square_foot_by_year DataFrame as a line plot.

---

## 3. Compared the Average Sale Prices by Neighborhood

- Created a new DataFrame that groups the original DataFrame by year and neighborhood. Aggregate the results by the mean of the groups.
- Filter out the “housing_units” column to create a DataFrame that includes only the sale_price_sqr_foot and gross_rent averages per year.
- Created an interactive line plot with hvPlot that visualizes both sale_price_sqr_foot and gross_rent. Set the x-axis parameter to the year (x="year"). Use the groupby parameter to create an interactive widget for neighborhood.

---

## 4. Build an Interactive Neighborhood Map

- Using hvPlot with GeoViews enabled, create a points plot for the all_neighborhoods_df DataFrame. Be sure to do the following:
    Set the size parameter to “sale_price_sqr_foot”.
    Set the color parameter to “gross_rent”.
    Set the frame_width parameter to 700.
    Set the frame_height parameter to 500.
    Include a descriptive title.

---

##  Contributors
Brought to you by Carlos Polanco.

- Email: carlos.polanco0508@gmail.com
- GithubProfile: https://github.com/carlosmpr
- Linkedin: https://www.linkedin.com/in/carlosmpr/

---

## License

MIT

Copyright (c) 2012-2022

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.