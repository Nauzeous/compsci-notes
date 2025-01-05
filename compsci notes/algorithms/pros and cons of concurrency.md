### benefits

==reactive programming:==
the user can interact with applications while other tasks run.

==availability:==
prevents long-running tasks taking resources from short-running tasks

==parallelism:==
allows faster performance if multiple cores are used to deal with separate parts of a task

==Controllability:==
tasks may require preconditions to continue, so the process can be suspended until the preconditions are met

### disadvantages

==safety:==
concurrent tasks should not be allowed to disrupt memory and corrupt the state of a program

==liveness:==
running tasks concurrently can cause deadlock, where multiple tasks are waiting for each other to do something

==resource consumption:==
running multiple tasks at the same time can consume a lot of resources, due to scheduling, synchronisation, and context-switching.
this can cause parallel programs to run slower than their non-parallel implementation if designed poorly

