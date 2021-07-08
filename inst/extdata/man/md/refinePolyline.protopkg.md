refinePolyline
==============

Example
-------

    # A simplistic example:
    # `source` select package contents to the user workspace / global environment
    DIR.PKG <- "~/PROTOPKGS/refinePolyline-WORM"
    COMPONENTS.PKG <- paste0(DIR.PKG,"/",as.character(read.csv(paste0(DIR.PKG,"/inst/extdata/collate/2.csv"))[[2]]))
    for(Component in COMPONENTS.PKG) source(Component)
    
