refine.xy
=========

Usage
-----

    refine.xy(xy, tolerance, quiet = TRUE, draw = FALSE )
    
|  Argument | Description |
| --------: | :---------- |
|        xy | a `numeric` `matrix` |
| tolerance | a `numeric` specifies the maximum segment-quadrance in the result. |
|     quiet | tells whether to write diagnostic information to standard out. |
|      draw | tells whether to draw the resultant polyline as it is created. |

Value
-----

A modified copy of `xy`, containing additional vertices that are uniformly spaced along the edges of `xy`.
The shortest edge of the result should be less than or equal to the `tolerance`.

Details
-------

Each row of `xy` is interpreted as a vertex having the number of dimensions indicated by `ncol(xy)`.

The `tolerance` value is interpreted as a quadrance.
Quadrance can be thought of as the _square_ of length.

Examples
--------

    m <- matrix(1:4, 2)
    m
    #      [,1] [,2]
    # [1,]    1    3
    # [2,]    2    4
    refine.xy(m, tolerance = 5^2)
