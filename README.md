IGV (Integrative Genomics Viewer) Demo Sessions

This repositiory contains two XML files which are IGV session files:
copynumber.xml (a file that configures IGV to load and visualize multiple copy number data tracks from the specified SEG files, allowing the user to analyze copy number changes across different samples):
More Description about this File:
A. Specify Hg38 reference genome
A. The Resources element contains multiple Resource elements, each specifying a path to a SEG (segmentation) file.
B. The Panel element defines a data panel with a specified height and width. Inside this panel, multiple Track elements are defined, each representing a different dataset (c1, c2, ..).
C. Each Track element has attributes like attributeKey, autoScale, clazz, colorScale, fontSize, id, and name, which configure the appearance and behavior of the track.
D. The DataRange element within each Track specifies the range of data values, with attributes like baseline, drawBaseline, flipAxis, maximum, minimum, and type.

