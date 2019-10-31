# Data Visualization of Massachusetts School District Retention Rates
WPI Data Viz class finali project

## Data

The data I used for this visualization include:

* A Massaschusetts Department of Elementary and Secondary Education [(DESE) public data set on student retention](http://profiles.doe.mass.edu/statereport/retention.aspx).  This report presents data on grade retention rates in Massachusetts public schools. The Massachusetts Department of Elementary and Secondary Education defines a student retention as: a student who was reported to have repeated the grade in which he or she was enrolled during the previous school year.

I processed the data by combining all available years into one dataset (2009-2018), removed non-targeted columns of data.  Additionally, I did a lookup between school district and city.  All those schools with unassociated towns (e.g. virtual schools) were removed.  Lastly, I calculated the dataset's quartiles and assigned each row to a quartile.


* The Massachusetts GeoJSON data can be found [here.](https://docs.digital.mass.gov/dataset/massgis-data-community-boundaries-towns-survey-points)

[Click to download](https://docs.digital.mass.gov/dataset/massgis-data-community-boundaries-towns-survey-points)

The [Mapshaper utility](https://mapshaper.org/) was used to convert the data.  GeoJson was imported, simplified, repaired, and exported to TopoJSON for use in [my VizHub account.](https://beta.vizhub.com/erikerickson)

The [gist with all data can be found here.](https://gist.github.com/erikerickson/4878febf8be358351aac34a29a63372a)

## Current Visualization

Here is the preview of the Massachusetts School District Retention visualization.

Click on the picture to go to the interactive visualization.
<img width="1440" alt="Visualization Preview" src="https://user-images.githubusercontent.com/54564637/67971170-a7542100-fbe2-11e9-9ab8-4f6290a085c2.png">

This visuaization shows a geographical representation of school district retention rates.  The interactive element includes two menus that allows users to filter to see one or all years.  The second menu allows a user to filter based upon quartile performance of the district, options include: all quartiles or one of the four.

### Map of MA
Here was in initial rendering of the Massachusetts School District json file using the MapShaper utility.
<img width="1440" alt="Screen Shot 2019-09-23 at 8 12 41 PM" src="https://user-images.githubusercontent.com/54564637/65472010-7c3a1d00-de3f-11e9-9491-cf2a8a86c667.png">

### Prototype Scatter Plot
Here was an initial scatter plot visualization that used the same public DESE dataset on school district retention rates.  This does not use the GeoJSON to visualize the data in a geographical way.

[<img width="960" alt="Visualization Prototype" src="https://user-images.githubusercontent.com/54564637/67972855-d8822080-fbe5-11e9-92e6-80fc72aed21c.png">](https://beta.vizhub.com/erikerickson/a62de7dcc3fb4677ac47330d95254e08?mode=full)

## Questions & Tasks

The following tasks and questions drove the visualization and interaction decisions for this project:
### Questions
 1. Are there longitudinal patterns of MA DESE Retentions? e.g. With school policies and political pressure promoting advancement, are there decreases of retentions over time? 
 
 2. Are there any notable geographical patterns?

 * Are retentions centralized in urban and economically disadvantaged areas in Massachusetts?
 * Are rural areas similar to those or urban or suburban areas?

## Preliminary Sketches

### Stacked Bar Chart
This is a sketch of what an initial bar chart visualization may look like.

<img width="414" alt="Screen Shot 2019-09-23 at 9 11 29 PM" src="https://user-images.githubusercontent.com/54564637/65473695-d8ed0600-de46-11e9-826c-dcd9630089e5.png">

### Bubble Map of Massachusetts School Districts
This is a sketch of an initial Geo Bubble Map may look like.

<img width="373" alt="Screen Shot 2019-09-23 at 9 11 37 PM" src="https://user-images.githubusercontent.com/54564637/65473694-d8ed0600-de46-11e9-97b7-2416f09d1d58.png">

## Open Questions
My experience in JS seems to be much thinner than others.  I am struggling with all the jargon that is being thrown around.  
I am not sure how to connect or implement the topoJSON into my viz or how to add the filtering, which in my mind is key to the success of the proposal.  It is the primary interaction and is critical to answer my proposed questions.

## Deliverables

### Data
I did the following activities near the dates indicated:
* Identified additional DESE datasets 10/5
* Downloaded from DESE 10/6
* Tranformed data 10/8
* Joined data 10/10
* Created new Gists 10/10
* Uploaded datasets to GitHub 10/10
* Documented Gists and linked back to original datasets 10/10

### Viz
I created the proposed visualization, adding interactive elements, and complete the project with a write up.
* Created Bubble map with MA GIS dataset 10/13
* Operationalize one set of data to work with Bubble Map 10/16
* Created Menu interaction for additional data 10/20
* Writeup (answer questions of proposal and describe the process) 11/1

## Future Work
This is not the visualization I was wanting.  There are continued opportunities to improve this visualization including the following:
* My goal will be to create a choropleth map of Massachusetts by school district. 
* Another interesting feature I would like to explore is the use of brushing or animation to help show changes through time.
* I would like to consider adding animation to the marks similar to this [example](http://bl.ocks.org/curran/8c131a74b85d0bb0246233de2cff3f52/194c2fc143790b937c42bf086a5a44cb3c55340e)
* Refine viz with colors
