# DISCRIMINATOR
DISCRIMINATOR is a command-line tool that assigns provisional pathogenicity classifications to CNVs based upon genomic location overlap with user-supplied presumed benign and pathogenic intervals.

# Requirements
DISCRIMNATOR requires Python (2.7.X) in a Linux operating system to run. Python3 is currently not supported. A list of the required Python modules is listed below. If you want to run the pre-processing script, bedtools is also required. 

Required Python Modules:
- progress
- networkx; version 1.8.1
- intervaltree

# Input
For processing, DISCRIMINATOR requires patient CNV datasets to be in tab-delimited with three columns with the header: 'Sample', 'Chromosome Region', 'Event'.
1.	The first column contains the patient or sample identifier.
2.	The second column contains the genomic coordinates for a single CNV in the following format (chr:start-end).
3.	The third column contains the direction of the CNV (accepted values: CN Gain or CN Loss)

To modify additional parameters for assigning provisional pathogenicity classifications, see the User Manual.

# Command to run DISCRIMINATOR:

    python CODE/INTERFACE_DISCRIMINATOR.py

# Citation
If you use the software, please cite: TBD

# Future Improvements
Support for Python3, Integration of bedtools pre-processing script with the rest of DISCRIMINATOR.
