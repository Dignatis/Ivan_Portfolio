# Ivan_Portfolio
Example of my work in Data Science

# [Project: Points to Profile](https://github.com/Dignatis/Points_to_Profile)
With this project task was to quantify change in the river bed over the years. 
Input data for this project was surveyed data from different  years (2004, 2014, 2016, 2018  and 2020). 
Surveyed data was in the form of points with X,Y,Z coordinates.  

<p>
    <img src="/images/ptp1.PNG" width="360" height="360" />
</p>

Task was thru different steps, here are quick summary of each (for more detailed explanation look in jupiter nootebook file): 

## Step 1

In this step all points data was projected on profile line.

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/PtP2.PNG" width="360" height="360" />
</p>


## Step 2

Was to change from global coordinate system (X,Y,Z) to local, profile coordinate system (Xprofile, Z)

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/PtP3.PNG" width="540" height="310" />
</p>

## Step 3

Was to determine referent plane and to find crossing points between  reference plane i profile (Xprofile, Z).

## Step 4

To find the area beneath the reference plane and profile for each year. 

## Step 5

To calculate and visualize changes.

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/PtP4.PNG" width="480" height="360" />
</p>




# [Project: Error analysis from log file HEC-RAS](https://github.com/Dignatis/Error_analysis_from_log_file_HECRAS)

Main idea for this project was to easily find cells in HEC-RAS 2D model that need corrections. Typical HEC-RAS 2D model contains between a couple thousand to a couple million cells. This tool needs to identify cells which make the biggest error.

<p>
    Log file from HEC-RAS looks like.
</p>

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/HecRas5.PNG" width="320" height="380" />
</p>

<p>
First step is to read only lines that contains data about cell and error and create DataFrame from it.
</p>

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/HecRas2.PNG" width="300" height="300" />
</p>

<p>
Next step is that for every cell get error statistic.
</p>

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/HecRas3.PNG" width="300" height="300" />
</p>

<p>
Last step is to choose parameter (SUM error, Average error, Count of error) 
and number top cells we want to see.
</p>

<p>
    <img src="https://github.com/Dignatis/Ivan_Portfolio/blob/main/images/HecRas4.PNG" width="300" height="300" />
</p>

<p>
  With this information we can go back to HEC-RAS and do changes to correct the model.
</p>
