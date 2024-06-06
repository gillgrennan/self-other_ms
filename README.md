

Functional parcellation of DMN activity taken from this paper: 
https://www.nature.com/articles/s41598-020-72317-8

Methods of DMN mask creation: 
DMN mask
First, to find regions that are functionally related but restricted to the four anatomical regions within the DMN that we are interested in, we created a DMN mask that constrained wider functional activation within an anatomical atlas95 (Fig. 1A). Specifically, we performed a meta-analytical association test by searching the term “DMN" in Neurosynth to create a functional mask that specifically mapped the term “DMN” to brain regions. We chose an association test (formerly named a “reverse inference”) because it can help estimate the relative specificity between brain activity and the DMN94,96. The resulting mask included 9,650 activations from 366 studies, and thus identified voxels in studies where the term “DMN” was mentioned in their abstract given brain activation. All of the images are thresholded with a false discovery rate of 0.01. Next, we constrained the mask to the four DMN regions of interest by using the Harvard–Oxford probabilistic atlas97 at P > 0.25, which included the medial prefrontal cortex (MPFC), the posterior cingulate cortex (PCC), and the left and right temporal parietal junction (left- and right-TPJ). This constraint was applied in the interest of specifying the output of our functional mapping and subsequent parcellation to a precise set of standardized coordinates within the four regions of interest.

Notes for later: 

Run typical ROI-analysis: 
  pre-define ROIs beforehand (DMN regions) -- take average activity in the mPFC, PCC, lTPJ, and rTPJ (based on Neurosynth dmn network map) --> run 4 roi values (1 value per ROI) through first / second-level w usual motion confounds, subject-wise intercepts etc. 

Third-level ROI analysis: 
  whole-brain first / second-level analysis 
  perform corrections on JUST DMN mask -- ignore the rest 
  (small voxel corrections?) 

example for third-level ROI analysis: 
https://nilearn.github.io/dev/auto_examples/06_manipulating_images/plot_roi_extraction.html#sphx-glr-auto-examples-06-manipulating-images-plot-roi-extraction-py
^ for overlapping voxels that survive threshold (bonferroni corrected across tested voxels) AND lie in the DMN mask 


