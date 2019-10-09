# Data Visualization Project Proposal
Work associated with WPI Data Viz class

## Data

The data I plan on using for my viz project include:
* The Massachusetts Department of Elementary and Secondary Education [(DESE) public data set on Advanced Placement](http://profiles.doe.mass.edu/statereport/ap.aspx) (AP) performance showing the number of students who received each possible score on the Advanced Placement exam for each subject.  This a transformed version of this dataset can be found [here](https://gist.github.com/erikerickson/c588471f631cd22b6745070eb0adabc0).

* The United States Census geographical data of [school districts in Massachusetts (TIGER)](https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2019&layergroup=School+Districts).  This has the shapefiles to create a map of all Massachusetts school districts.

* Update.  I found the [MassGIS Data: Public School Districts])https://docs.digital.mass.gov/dataset/massgis-data-public-school-districts) to have a better version of the data.  I used MapShaper to visualize the data and this updated datasource looks much better.

## Prototypes

I have created the first step of the visualization, which was creating a stacked bar chart of the AP data.  It shows a high-level view of general participation and performance across Massachusetts school districts through time.  My goal will be to create a choropleth map of Massachusetts by school district. 

To add interactivity, I would like to slice on different measures similar to what is shown in the [Scatter Plot with Menus](http://bl.ocks.org/curran/8c131a74b85d0bb0246233de2cff3f52/194c2fc143790b937c42bf086a5a44cb3c55340e) example. I would like to create a menu that will answer some of the previously identified questions that I found interesting, mainly those socio-economic and demographic attributes found in some DESE datasets.  Another interesting feature I would like to explore is the use of brushing or animation to help show changes through time.  This may not work with my choropleth map of Massachusetts.

### Map of MA
<img width="1440" alt="Screen Shot 2019-09-23 at 8 12 41 PM" src="https://user-images.githubusercontent.com/54564637/65472010-7c3a1d00-de3f-11e9-9491-cf2a8a86c667.png">

### Prototype Stacked Bar Chart
[<img width="960" alt="Screen Shot 2019-09-23 at 8 11 35 PM" src="https://user-images.githubusercontent.com/54564637/65472011-7c3a1d00-de3f-11e9-9dee-6533dcb1e96c.png">](https://beta.vizhub.com/erikerickson/994860e04695449fb499a3e36828e940)

## Questions & Tasks

The following tasks and questions will drive the visualization and interaction decisions for this project:
### Questions
 1. Are there longitudinal patterns of AP Test taking? e.g. Is there increased test-taking over time?  Are there higher rates of success (qualifying scores) over time?  
 2. Are there any notable socio-economic patterns?

 * Economically Disadvantaged
 * Free and Reduced Lunch

 3. Are there any notable demographic patterns?
 * First Language Not English
 * English Language Learner
 * Students With Disabilities
 * High Needs
 * Race
 * Gender
 
 4. e.g. Do high test taking schools have relatively high success rates (scores >=3)?
 5. Are there any notable geographical patterns associated with test taking or success?  Do certain geographical areas have higher levels of participation or success?

## Sketches

### Stacked Bar Chart
<img width="414" alt="Screen Shot 2019-09-23 at 9 11 29 PM" src="https://user-images.githubusercontent.com/54564637/65473695-d8ed0600-de46-11e9-826c-dcd9630089e5.png">

This is the baseline viz that I have created in Vega Lite.  I will need to take this viz and make it work in D3.  I will then need to visualize just one score, of success rate % on the map.  Once I have this working, adding in additional interactive functionality with filter(s) will be great.  Finding a robust tooltip will be helpful.

### Heat Map of Massachusetts School Districts
<img width="373" alt="Screen Shot 2019-09-23 at 9 11 37 PM" src="https://user-images.githubusercontent.com/54564637/65473694-d8ed0600-de46-11e9-97b7-2416f09d1d58.png">

## Open Questions
My experience in JS seems to be much thinner than others.  I am struggling with all the jargon that is being thrown around.  
I am not sure how to connect or implement the topoJSON into my viz or how to add the filtering, which in my mind is key to the success of the proposal.  It is the primary interaction and is critical to answer my proposed questions.

## Schedule of Deliverables

### Data
I will do all the processes necessary to acquire and transform the data to be visualized.
* Identify additional DESE datasets 10/5
* Download from DESE 10/6
* Tranform data if necessary 10/8
* Joing data if necessary 10/10
* Create new Gists 10/10
* Upload to datasets to GitHub 10/10
* Document Gists and link back to original datasets 10/10

### Viz
I will create the proposed visualization, adding interactive elements, and complete the project with a write up.
* Create Cloropleth with Tiger dataset 10/13
* Get one set of data to work with Cloropleth 10/16
* Create Menu interaction for additional data 10/20
* Create Animation (if times allows) 10/24
* Explore data to understand important outcomes 10/26
* Refine viz with colors 10/28
* Writeup (answer questions of proposal and describe the process) 11/1
