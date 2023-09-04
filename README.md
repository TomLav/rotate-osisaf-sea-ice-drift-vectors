# Transformation and Rotation of OSI SAF Sea Ice Drift vectors
This repo demonstrates common transformations of sea-ice drift vector components. It was originally prepared as a companion to the manuscript documenting the first version of the OSI SAF sea-ice drift Climate Data Record (OSI-455):

_Lavergne, T. and Down, E.: A Climate Data Record of Year-Round Global Sea Ice Drift from the EUMETSAT OSI SAF, Earth Syst. Sci. Data Discuss. [preprint], https://doi.org/10.5194/essd-2023-40, in review, 2023._

The notebook contains python software to:
1. express displacement vectors (unit km over a time period, e.g. 24 hours) as mean velocity vectors (unit km/d, m/s, etc...);
2. rotate vector components from the original grid (EASE2 of PolStere) to any other grid (including the lat/lon projection to yield eastward/northward components);
3. average vector fields from daily to weekly and monthly periods.

We strongly encourage to read the discussion about the choice of vectorial representation for satellite-based sea-ice drift vectors in Lavergne and Down, 2023 (Sect. 4.2) before using the software. While it is technically possible to express the OSI SAF sea-ice drift vectors as velocities or onto other grids, the results must be interpreted with caution.

Although the software was developed for the OSI-455 CDR, we made it compatible with the OSI SAF near-real-time (NRT) sea-ice drift product as well (OSI-405). The two products and their documentation can be accessed from:
* OSI-455 (Climate Data Record) : https://osi-saf.eumetsat.int/products/osi-455
* OSI-405 (Near Real Time product) : https://osi-saf.eumetsat.int/products/osi-405-c

The software is provided AS-IS in hope that it is useful to the user of the OSI SAF sea-ice drift products. You are free to copy and modify the software for your needs. Please cite the notebook on Zenodo if you use it, and the data if you use it in your research.

We welcome feedback and bug reports either through the github issue page, or by email to Thomas Lavergne.
