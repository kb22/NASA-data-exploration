# NASA-data-exploration
The repository includes detailed steps to get NASA data from GES DISC, convert HDF5 files to CSV and plotting geographic data. In this repository, we extract Global Precipitation Measurement (GPM) data, which keeps measures precipitation all across the globe. We'll capture the data for January, 2020. While this repository steps get specific, the exact same steps apply to any HDF5 data downloaded from GES DISC.

## Step 1: Get data
The first step is to get data from the [GES DISC](https://disc.gsfc.nasa.gov/) website. The detailed steps are described by me in the article [Getting NASA data for your next geo-project](https://towardsdatascience.com/getting-nasa-data-for-your-next-geo-project-9d621243b8f3?source=friends_link&sk=b5b1e2415be5738e578dbf28386e3b9d). Here, we'll be working with HDF5 files.

## Step 2: From HDF5 to CSV
The second step is to take the HDF5 files we downloaded, understand their content and generate CSV files which can be easily used. We use the package `h5py` to read in the HDF5 files, and based on the column data we need, we create a CSV file which can be easily distributed or analyzed.
