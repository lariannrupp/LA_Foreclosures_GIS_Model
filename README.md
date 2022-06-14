# LA_Foreclosures_GIS_Model

---

The purpose of this exercise is to chart a set of interactive GIS maps for Los Angelos real estate foreclosure data.

---

## Technologies

**A Python 3.9.7 (ipykernal) in JupyterLab** was used to write this notebook.


Additional Python libraries are imported into the start of the app: 

![Screenshot 2022-06-14 150853](https://user-images.githubusercontent.com/95719899/173689316-7a060037-5139-4878-98d6-383395d963da.jpg)





---

## Installation Guide

To use the app, from the Github repository, download:
- **plotting_foreclosures.ipynb** Jupyter file 
- **Resources** folder that contains a csv file which the program uses

Use either Terminal or GitBash to run the app in a conda dev environment. 
To enter a conda dev environment, type
'conda activate dev'

You may need to install the PyViz Ecosystem in Terminal or GitBash.
Install the PyViz packages by using the conda install command as follows:
> conda install -c pyviz hvplot geoviews

Confirm the installation of all the PyViz packages by running the following commands:
> conda list hvplot
> conda list geoviews

To run the app, navigate to the root directory, which contains **plotting_foreclosures.ipynb** and the **Resources** folder adjacent to one another, and then type
'jupyter lab'



---

## Usage

As you run through the exercise, observe how I analyzed San Francisco Real Estate Investment Opportunities through the following steps:

1. Using the read_csv function and the Path module, read 2018_Registered_Foreclosure_Properties.csv from the Resources folder, and create the la_foreclosures_2018 DataFrame.

![Screenshot 2022-06-14 151410](https://user-images.githubusercontent.com/95719899/173690145-849547a6-6ac5-49d6-a95c-fe3edc92a2ad.jpg)


2. Use the points function to plot the data from the most_foreclosures_df DataFrame. 

Include parameters as follows:

- Use the “Longitude” and “Latitude” columns in the DataFrame as your geospatial data.

- Set geo equal to True to enable the GeoViews integration

- Set color based on the “Lender” column.

- Set tiles to "OSM".

- Set frame_width to 700.

- Set frame_height to 500.

- Create a title for the plot.

![Screenshot 2022-06-14 150245](https://user-images.githubusercontent.com/95719899/173690191-cd6178ed-623e-488d-8f44-704150137071.jpg)




3. Use the points function to create a second plot from the most_foreclosures_df DataFrame. 

Keep all the parameters unchanged except as follows:

- Set the color parameter to “Property Type”.

- Change the title parameter to correspond to the new information that you’re plotting.


![Screenshot 2022-06-14 150331](https://user-images.githubusercontent.com/95719899/173690290-c890f68d-3c02-4467-909f-589370761eaf.jpg)



4. Use the points function to create a third plot from the most_foreclosures_df DataFrame. 

Keep all the parameters unchanged except as follows:

- Set the color parameter to “Council District”.

- Change the title parameter to correspond to the new information that you’re plotting.


![Screenshot 2022-06-14 150406](https://user-images.githubusercontent.com/95719899/173690317-b4cfcff7-39dc-479c-a10c-f1940ac9b8c7.jpg)


---

## Contributors

This exercise was based on a challenge problem from UC Berekely Fintech Bootcamp Module 6, accessed on 2022.06.14. 

For any questions, please reach out to me on [LinkedIn](https://www.linkedin.com/in/lari-rupp-5baa49153/)

---

## License

Creative Commons Zero
