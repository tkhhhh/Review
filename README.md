# Review
information about computer science

## OS

### file system
 - File Attributes
 - File Access Methods (index sequential access)
 - Space Allocation (index allocation)
 - soft link / hard link
 
### CPU and Task
 - System calls
 - blocking call / non-blocking call
 - scheduling
   + context switch
   + progress / thread
      * sleep / wake
   + example Go routines
      * go routine -> OS thread with go scheduler and go run time
      * hood
      ```
         func ServeHTTP(w http.ResponseWriter, r *http.Request) {

            // the underlying network call here is non-blocking
            rows, err := db.Query("SELECT ...")
            
            for _, row := range rows {
               // do something with the rows,
         // each request in its own goroutine
            }

            w.Write(...) // write the response, also non-blocking

         }
      ```
 - different caches


## Datastructure and algorithm
 - math description
    - absolute value
    - arccosine / arcsine / arctangent (how to achieve)
    - retangular coordinate / polar coordinate
    - cube root / square root (how to achieve)
    - exp() (how and description)
    - hypot(x, y) (avoid overflow and underflow)
    - natural logarithm base (E)x (log) (how)
    - positive / negative infinity
    - random number
    - rounded to (how) round()
    - sign of x signum()
    - hyperbolic sine / tangent
    - in radians / in degrees
    - unit of least precision / distance between this and next larger value in magnitude
    - built-in
    - 