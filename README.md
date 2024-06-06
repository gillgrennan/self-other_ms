

Functional parcellation of DMN activity taken from this paper: 
https://www.nature.com/articles/s41598-020-72317-8

Methods of DMN mask creation: 
DMN mask
First, to find regions that are functionally related but restricted to the four anatomical regions within the DMN that we are interested in, we created a DMN mask that constrained wider functional activation within an anatomical atlas95 (Fig. 1A). Specifically, we performed a meta-analytical association test by searching the term “DMN" in Neurosynth to create a functional mask that specifically mapped the term “DMN” to brain regions. We chose an association test (formerly named a “reverse inference”) because it can help estimate the relative specificity between brain activity and the DMN94,96. The resulting mask included 9,650 activations from 366 studies, and thus identified voxels in studies where the term “DMN” was mentioned in their abstract given brain activation. All of the images are thresholded with a false discovery rate of 0.01. Next, we constrained the mask to the four DMN regions of interest by using the Harvard–Oxford probabilistic atlas97 at P > 0.25, which included the medial prefrontal cortex (MPFC), the posterior cingulate cortex (PCC), and the left and right temporal parietal junction (left- and right-TPJ). This constraint was applied in the interest of specifying the output of our functional mapping and subsequent parcellation to a precise set of standardized coordinates within the four regions of interest.

