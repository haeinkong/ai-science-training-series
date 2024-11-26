Theory Homework

1.What are the key architectural features that make these systems suitable for AI workloads?

Specialized Hardware Design to accelerate matrix multiplications and tensor operations.
High Memory Bandwidth and larger amount of on-chip memory help to accelerate memory intensive AI worklaods.
Scalability and Parallelism: Parallel processing of data across many cores or processing units, which significantly speeds up training and inference tasks
Identify the primary differences between these AI accelerator systems in terms of their architecture and programming models.

2.Identify the primary differences between these AI accelerator systems in terms of their architecture and programming models.

Sambanovas Reconfigurable Dataflow Unit (RDU) allows for flexible dataflow processing that features a multi-tiered memory architecture with terabytes of addressable memory for efficinet handling of large data.
Cerebras Wafer-Scale Engine (WSE) consists of processing elements (PEs) with its own memory and operates independently. Fine-grained dataflow control mechanism within its PEs make the system highly parallel and scalable.
Graphcore’s Intelligence Processing Unit (IPU) consists of many interconnected processing tiles, each with its own core and local memory. The IPU operates in two phases—computation and communication—using Bulk Synchronous Parallelism (BSP).
Groq’s Tensor Streaming Processor (TSP) architecture focuses on deterministic execution which s particularly advantageous for inference tasks where low latency is critical.
Based on hands-on sessions, describe a typical workflow for refactoring an AI model to run on one of ALCF's AI testbeds (e.g., SambaNova or Cerebras). What tools or software stacks are typically used in this process?

3.Based on hands-on sessions, describe a typical workflow for refactoring an AI model to run on one of ALCF's AI testbeds (e.g., SambaNova or Cerebras). What tools or software stacks are typically used in this process?

For example, Samba compilation flow consists of 4 steps: Saaba PyTorch compilation, Graph compiler, Kernel compiler, and Kernel library.
Typical worksflow involves using vendor specific implementation of ML framework like PyTorch to port model. 

4.Give an example of a project that would benefit from AI accelerators and why?

This can be used to compare the performance of Large Language Models across diverse AI accelerators. This project can help to understand the strength and weaknees of models and hardward platforms. 
