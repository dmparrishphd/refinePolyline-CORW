(Title)
=======

Example
-------

    DIR.PKG <- "~/PROTOPKGS/refinePolyline-WORM"
    COMPONENTS.PKG <- paste0(DIR.PKG,"/",as.character(read.csv(paste0(DIR.PKG,"/inst/extdata/collate/1.csv"))[[2]]))
    for(Component in COMPONENTS.PKG) source(Component)
    
    refine.xy(xy)


