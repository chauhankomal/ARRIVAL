# ARRIVAL

to run the code, run "run.sh" with two arguments, 1: folder name of the dataset being used, 2: queryfilename inside folder 1

The folder should contain edgefile (edges.txt) (each line of the form u v l, where there is an edge from u to v with a label l, if l is not present it is assumed to be 1), labelfile (labels.txt) (each line of the form u l, where node u has a label l, multiple labels on a node are allowed with newline) and the required queryfile (query has to be of the form u v noderegex edgeregex, if no edgeregex is found it will be assumed to be (1)\*).