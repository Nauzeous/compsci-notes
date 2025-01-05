pipelining involves splitting a large task into individual chunks that are parallelised/overlapping in order to speed up the process

an example is a 3d video game; the physics engine runs on the CPU and sends a set of vertices to the shader that runs on the GPU to create the next frame

while the GPU is working on the next frame, the CPU does not have to wait to simulate the next frame's vertices, thus pipelining can be implemented

pipelining was also mentioned in [[Fetch, decode, execute]]