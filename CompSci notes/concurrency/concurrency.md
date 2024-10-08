concurrency means that an application is doing multiple things at the same time

==thinking concurrently== involves working out the parts of a program that are independent, and can be processed separately from other tasks

**exam questions on concurrency ask which parts of a program can be processed concurrently, and which parts cannot be processed concurrently**

non-concurrent code can be traced through line by line with your finger, whereas concurrent code will be running multiple sets of lines of codes at a time

concurrency in python is limited by the **Global Interpreter Lock** (GIL), which limits running python code to 1 core

concurrency in only one core is achieved using [[scheduling techniques]], giving each thread a time slice

concurrency is called concurrency whether or not the code is running on multiple cores, or multiple threads on a single core
### distinguishing parallelism and concurrency

it is easy to conflate the two terms as they have overlapping definitions

parallelism is a subsection of concurrent processing that involves **simultaneous execution** of processes, using multiple processor cores

parallelism does not require multiple processes in order to be classed as parallelism, as a single task can be subdivided and managed by multiple cores



