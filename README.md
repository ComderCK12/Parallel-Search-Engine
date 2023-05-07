# Parallel-Search-Engine

This is a parallel search engine that uses MPI to search for a target word in a given text file. The program is designed to run on multiple processors, allowing it to perform the search in parallel, which can significantly reduce the search time.

Installation <br/>
To use this program, you'll need to have MPI installed on your system. You can download MPI from the MPI website.

Once you have MPI installed, you can download the program files from this repository and run them on your system. <br/>


Performance Analysis <br/>
We compared the performance of this parallel search engine with a linear search engine using the same target word and text file. We ran the searches multiple times and measured the average search time for each engine.


Here are the results:

| Engine | Search TIme |
| ---------------|----------------|
| Linear  | 0.004189491271972656  |
| Parallel  | 0.002236582298337453  |

Performance ratio = T(linear)/T(Parallel) = 0.004189491271972656/0.002236582298337453 = 1.8731666056227325 =~ 2 <br/>
<br/> As you can see, the parallel search engine was able to perform the search almost 2x faster than the linear search engine. This is because the parallel engine is able to split the search across multiple processes, allowing it to search for the target word simultaneously on different parts of the text file.
