# Pandas File Format Comparision
## Table Of Content
* [Overview](#overview)
* [Numerical Data](#num_data)
* [Numerical + Categorical Data (Object)](#num_data_cat_obj)
* [Numerical + Categorical Data (pandas.Category)](#num_data_cat)


## Overview<a name="overview"/>
This repository is about comparing how different file formats behaves in Pandas DataFrame. In this study we are considering the following file formats:
* csv - common text file that is comma separated.
* hdf5 - an open-source file format that supports large, complex, heterogeneous data.
* parquet - an open source, column-oriented data file format designed for efficient data storage and retrieval.
* feather - a portable file format for storing Arrow tables or data frames (from languages like Python or R) that utilizes the Arrow IPC format internally.

Parameters we are comparing for:
* Time to write.
* File Size on Disk.
* Time to read.
* Memory Usage.

## Numerical Data<a name="num_data"/>
Data Count: 1L || RT Environment: Google Colab || Ram: 12.68GB || Disk: 107.72GB
Parameters     | CSV           | HDF5          | Parquet       | Feather       |
-------------  | ------------- | ------------- | ------------- | ------------- |
Write Time  | 1.74 sec | 0.267 sec | 0.51 sec | 0.072 sec |
Read Time   | 0.254 sec | 0.0274 sec | 0.0994 sec | 0.018 sec |
File Size On Disk  | 19 MB | 8.5 MB | 9.7 MB | 7.7 MB |
Memory Usage  | 7.6 MB | 8.4 MB | 7.6 MB |  7.6 MB |

Check the notebook for more details.

## Numerical + Categorical Data (Object)<a name="num_data_cat_obj"/>


## Numerical + Categorical Data (pandas.Category)<a name="num_data_cat"/>
