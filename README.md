DijkstraSpark Assignment (Python Version)

Prerequisites

Ensure Apache Spark 3.5.0 is installed on the VM.
Ensure Python 3 is installed:sudo apt update
sudo apt install python3 -y


PySpark should be available with Spark (typically located in /usr/local/spark/bin/).

Execution Instructions

Place dijkstra_spark.py in a directory (e.g., ~/dijkstra-spark).
Ensure weighted_graph.txt is in /home/azureuser/.
Navigate to the directory:cd ~/dijkstra-spark


Run the PySpark script:/usr/local/spark/bin/spark-submit dijkstra_spark.py


The output will be saved to /home/azureuser/dijkstra-spark/shortest_paths.txt, showing the shortest distances and paths from node 0 to all other nodes.

Notes

The program uses PySpark RDD transformations to implement Dijkstra’s algorithm.
The input file weighted_graph.txt should have the format specified in the assignment (e.g., first line: num_nodes num_edges, followed by edge list).
The output format is: Node <id>: Distance <dist>, Path <path> for each node.

