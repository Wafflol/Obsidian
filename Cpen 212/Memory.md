Top of memory: OS kernel, Stack
Bottom of memory: binaries loaded from disk, heap

#### Allocation Strategies
##### Manual: allocate + de-allocate pairs
malloc() + free(), new + delete
uncomplicated but hard and buggy to use


##### Automatic: Allocate and Forget
garbage collection
reference counting (limited)
implementation complex but easy to use
