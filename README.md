# Parallel-Volume-Rendering-Using-MPI (Course Project, CS677)

In this project, we are provided with a 3D dataset of a cyclone (in vti format). The task is to visualize this dataset by utilizing the ray-casting algorithm. However, implementing ray-casting algorithm over this dataset (sufficiently large) is computationally expensive and time-consuming. And so, there is a need to perform this ray-casting algorithm in parallel.

Hence, the data was first splitted among n processes. Then each of these n process performs the ray-casting algorithm in a parallel manner. This step reduces the processing time to a large extent (Please refer to the report for details) and thus makes the ray-casting implementation efficient. Finally, the output (a 2D image) from each of these n processes was collected and merged into a single, complete image.
