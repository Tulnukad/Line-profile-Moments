To calculate moments you have to upload your .dat files, which contain spectral line profile. It should be normalized, isolated spectral line.
Each file must contain two columns: Velocity in km/s and normalized Flux. No headers in the files, numbers only! File-names have to be in such format (example): object_yyyymmdd_xx.dat In such way the script
can sort files by date.
Within the files also have to be JD-file, which contains Julian Date for each spectrum as a list in one column.
First, the script fit Voight profile into the spectral line profile and calculates centroid of the line. Then it calculates Moments for the velocity range from -150 km/s to +150 km/s 
relative to the center of the line.
Finally, we have "output_file", which contains 5 columns: JD, Mo, M1, M2, M3.
