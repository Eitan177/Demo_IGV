IGV (Integrative Genomics Viewer) Demo Sessions

This repositiory contains two XML files which are IGV session files:

1. copynumber.xml (a file that configures IGV to load and visualize multiple copy number data tracks from the specified SEG files, allowing the user to analyze copy number changes across different samples):
More Description about this File:
  A. Session element specifies Hg38 as the reference genome
  
  B. Multiple resource elements specifying paths to a SEG (segmentation) file.
  
  C. The Panel element defines a data panel with a specified height and width. Inside this panel, multiple Track elements are defined, each representing a different dataset (c1, c2, ..).
  
  D. Each Track element has attributes like attributeKey, autoScale, clazz, colorScale, fontSize, id, and name, which configure the appearance and behavior of the track.
  
  E. The DataRange element within each Track specifies the range of data values, with attributes like baseline, drawBaseline, flipAxis, maximum, minimum, and type.
  

2. egfr_vIII_demo.xml (a file that configures IGV to load alignment file from specified Bam file, allowing the user to analyze an EGFR vIII rearrangement):
  A. The Session element specifies the genome version (hg19) and the locus (chr7:55086528-55088221).
  
  B. The Resources element lists the data resources used in the session, in this case, a BAM file (proband.bam) from a specified URL.
  
  C. The Panel element defines a data panel with specified height and width. Inside this panel, multiple Track elements are defined:
    CoverageTrack for coverage data of proband.bam, with auto-scaling enabled and a data range from 0.0 to 445.0.
    SpliceJunctionTrack for splice junctions data of proband.bam, with a fixed height of 60.
    AlignmentTrack for alignment data of proband.bam, with a specified color and display mode set to EXPANDED, and duplicates filtered.
    
  D. Another Panel element defines a feature panel with specified height and width, including:
    SequenceTrack for reference sequence data.
    FeatureTrack for displaying Refseq genes with a continuous color scale.
