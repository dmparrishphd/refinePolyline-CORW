(Title)
=======

Example
-------

    DIR.PKG <- "~/PROTOPKGS/refinePolyline-WORM"
    COMPONENTS.PKG <- paste0(DIR.PKG,"/",as.character(read.csv(paste0(DIR.PKG,"/inst/extdata/collate/2.csv"))[[2]]))
    for(Component in COMPONENTS.PKG) source(Component)
    
    #REMINDER: tolerance is a *quadrance*, not a distance
    refine.xy(matrix(1:4, 2), tolerance = 5^2)
    
    #      [,1] [,2]
    # [1,] 1.00 3.00
    # [2,] 1.25 3.25
    # [3,] 1.50 3.50
    # [4,] 1.75 3.75
    # [5,] 2.00 4.00
