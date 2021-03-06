# Moberg Analytics HDF5 Functions

This package provides user-friendly functions organized into Classes for reading [HDF5](https://www.hdfgroup.org/solutions/hdf5/) file content and components into Python. It is built on top of the [h5py package](https://www.h5py.org/) which interfaces directly with the HDF5 file. 

## Installation

Install the Moberg-Analytics-HDF5 package from [PyPI](https://pypi.org/project/Moberg-Analytics-HDF5/):

    pip install Moberg-Analytics-HDF5
    
This package was created using Python version 3.9.0.

## How to use

1 - Import the hdf5_tools module from moberg_analytics_hdf5 package into Python:
	
	from moberg_analytics_hdf5 import hdf5_tools
	
2 - Select the path to the HDF5 file:

	hdf5_filepath = r"path to the hdf5 file"
	
3 - Instantiate the HDF5Content, HDF5Components, and/or the HDF5Helper class:

-The HDF5Content class contains functions that organize the content of the HDF5 file into lists and dictionaries.

-The HDF5Components class contains functions that return various components of the HDF5 file such as
groups, datasets, dataset values, NumPy/Pandas matrices of dataset values, metadata attributes, and structured dictionaries.

-The HDF5Helper class contains functions for argument, group, dataset, and duplicate checks and adds additional functionality to the HDF5Content and HDF5Components classes.

	hdf5_content = hdf5_tools.HDF5Content(hdf5_filepath=hdf5_filepath)
	
	hdf5_comps = hdf5_tools.HDF5Components(hdf5_filepath=hdf5_filepath)
	
	hdf5_helper = hdf5_tools.HDF5Helper()
	
4 - Use the functions as detailed in the documentation below.

## Documentation 

The Moberg-Analytics-HDF5 documentation is located [here](https://moberg-analytics-inc.github.io/Moberg-Analytics-HDF5-Documentation/).
