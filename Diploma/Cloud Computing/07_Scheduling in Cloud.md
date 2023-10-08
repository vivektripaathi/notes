# Scheduling in Cloud Computing
- Technique to map set of jobs to set of VMs or allocating VMs to run on available resources.
- Aim to improve **throughput**, **load balance**, and maximize the **resource utilization**, save energy, reduce cost, and minimize the processing time. 
- Used to distribute valuable computing resources, usually processor time, bandwidth and memory, to the various processes, threads, data flows and applications that need them.
- To balance the load of the system, and to ensure the equal distribution of resources and give some prioritization according to set of rules.
- To ensure that computer can serve all requests and achieve some quality of service.
- Also known as process scheduling.

# Scheduling Problems
1. **Job Scheduling** :  This is the problem of finding the optimal schedule for a set of jobs, given a set of constraints such as the availability of resources and the deadlines for the jobs.
2. **Resource allocation:** This is the problem of assigning resources to a set of tasks, given a set of constraints such as the availability of resources and the priorities of the tasks.
3. **Load balancing:** This is the problem of distributing a workload evenly across a set of resources, in order to improve performance and avoid overloading any one resource.
4. **Fault tolerance:** This is the problem of ensuring that a system can continue to operate even in the event of failures, by gracefully migrating tasks to other resources.
There are a number of different approaches to solving scheduling problems in cloud computing. Some common approaches include:
- **Heuristics:** These are simple, rule-based algorithms that can be used to find good solutions to scheduling problems.
- **Metaheuristics:** These are more sophisticated algorithms that can be used to find better solutions to scheduling problems, but they may require more time to run.
- **Machine learning:** This can be used to develop models that can predict the behavior of scheduling problems, and to guide the search for better solutions.

# Types of Scheduling in cloud computing
1. **Task Scheduling** : It focuses on assigning tasks or jobs to available resources of the cloud, in order to minimize task execution time, maximize resource utilization, and achieve load balancing.
2. **Resource Scheduling** : Focuses on allocation of cloud resources such as storage, VMs, containers, and network bandwidth. Determines which resource should be assigned which task based on the requirements and availability.
3. **VM Scheduling** : Virtual Machine (VM) scheduling is specifically related to allocating and managing virtual machines in the cloud. It includes determining the placement of VMs on physical hosts or servers, considering factors such as resource utilization, load balancing, and fault tolerance.
4. **Data Scheduling** : Data scheduling involves managing the storage and movement of data within the cloud infrastructure. It includes techniques for efficient data replication, caching, and migration to ensure data availability, accessibility, and reliability.
5. **Workflow Scheduling** : Workflow scheduling focuses on orchestrating and optimizing the execution of complex workflows or business processes that involve multiple interdependent tasks or services. It aims to minimize the overall workflow execution time and improve resource utilization.
6. **Batch Scheduling** : Batch scheduling involves scheduling large-scale batch processing jobs or computations in the cloud. It aims to efficiently allocate resources to process a significant number of tasks or data sets simultaneously, typically with low interactivity requirements.

1. Centralized/Decentralized Scheduling :-Decision-making by central node/that of distributed system.
2. Primitive/Non-Primitive Scheduling:- interruption ,migration of task allowed during execution.
3. Immediate/Batch Mode:- Depends on time taken to start execution.
4. Heuristic/Meta Heuristic:- Problem dependent, higher problem dependent. Does not guarantee optimal Solution, but give good solution.
5. Static/Dynamic Scheduling:- Known timing information, unknown aadmi.


# Scheduling for Independent and Dependent Tasks
### Independent Task Scheduling
Independent tasks are those that can be executed in any order without any interdependencies. Scheduling independent tasks in cloud computing typically involves the following approaches:
   - **Load Balancing**: Independent tasks can be distributed across available resources in a load-balanced manner to optimize resource utilization and minimize task execution time. Load balancing algorithms consider factors like resource availability, load on each resource, and network conditions to evenly distribute the tasks.
   - **Task Duplication**: Replicating independent tasks and executing them simultaneously on multiple resources can enhance performance and fault tolerance. Task duplication techniques aim to leverage parallelism and redundancy to improve task execution time and increase the likelihood of successful task completion.
   - **Task Prioritization**: Assigning priorities to independent tasks allows the scheduler to allocate resources to high-priority tasks first, ensuring critical tasks are executed promptly. Priority-based scheduling ensures that important tasks are not delayed due to resource contention or other factors.
### Dependent Task Scheduling
Dependent tasks are those that have interdependencies and need to be executed in a specific order. Scheduling dependent tasks in cloud computing involves considering their dependencies and ensuring proper coordination. Here are a few common techniques:
   - **Task Graph Scheduling**: Dependent tasks can be represented as a directed acyclic graph (DAG), where the nodes represent tasks, and the edges represent dependencies between tasks. Schedulers use graph-based algorithms to determine the optimal order of task execution, considering dependencies, resource availability, and other constraints.
   - **Critical Path Scheduling**: The critical path represents the longest sequence of dependent tasks that must be executed to complete the entire workload. Schedulers focus on scheduling tasks on the critical path first to ensure timely completion of the overall job. This approach optimizes the completion time of the entire workflow.
   - **Task Chaining**: Dependent tasks can be chained together, where the output of one task becomes the input for the next task. Schedulers ensure that tasks are scheduled in the correct order and their dependencies are satisfied. Task chaining allows for efficient data flow between tasks and minimizes data transfer overhead.
   - **Dependency-aware Scheduling**: Schedulers consider the dependencies between tasks when allocating resources. They ensure that dependent tasks are scheduled on the same resource or nearby resources to minimize data transfer delays and improve task coordination.

# Static Scheduling v/s Dynamic Scheduling
### Static Scheduling
Static scheduling refers to the process of allocating and assigning resources to tasks or jobs in advance, before their actual execution. It involves making scheduling decisions based on pre-defined policies or predetermined criteria.
### Dynamic Scheduling
Dynamic scheduling, on the other hand, involves making scheduling decisions dynamically during the execution of tasks based on the real-time conditions and workload characteristics. It enables adaptive resource allocation and optimization.

#### Differences b/w Static & Dynamic Scheduling

1. **Static scheduling is pre-determined, while dynamic scheduling is based on demand.** With static scheduling, the resources are allocated to tasks before they start running. This means that the resources are not always fully utilized, as some tasks may require more resources than others. With dynamic scheduling, the resources are allocated to tasks as they start running. This means that the resources are more likely to be fully utilized, as the amount of resources allocated to each task can be adjusted based on the demand.
2. **Static scheduling is simpler to manage, while dynamic scheduling is more complex.** With static scheduling, there is no need to monitor the resources or adjust the allocation as needed. This makes it easier to manage. With dynamic scheduling, the resources need to be monitored and the allocation adjusted as needed. This makes it more complex to manage.
3. **Static scheduling is less flexible, while dynamic scheduling is more flexible.** With static scheduling, the resources cannot be reallocated to other tasks if a task finishes early or takes longer than expected. This makes it less flexible. With dynamic scheduling, the resources can be reallocated to other tasks as needed. This makes it more flexible.
4. **Static scheduling is less responsive, while dynamic scheduling is more responsive.** With static scheduling, it can take some time to reallocate resources to a new task. This can lead to delays in the execution of the new task. With dynamic scheduling, resources can be reallocated to a new task immediately. This can help to improve the performance of the new task.
5. **Static scheduling is less scalable, while dynamic scheduling is more scalable.** With static scheduling, it can be difficult to scale up or down the number of resources allocated to a task. This can make it difficult to handle spikes in demand. With dynamic scheduling, the number of resources allocated to a task can be scaled up or down as needed. This makes it easier to handle spikes in demand.
6. **Static scheduling is less reliable, while dynamic scheduling is more reliable.** With static scheduling, if a resource fails, the task that is running on that resource will fail. This can lead to downtime for the application. With dynamic scheduling, if a resource fails, the task will be moved to another resource. This can help to improve the reliability of the application.
7. **Static scheduling is less secure, while dynamic scheduling is more secure.** With static scheduling, all tasks are running on the same resources. This makes it easier for an attacker to compromise all of the tasks. With dynamic scheduling, tasks can be run on different resources. This can help to improve the security of the application.
8. **Static scheduling is less cost-effective, while dynamic scheduling is more cost-effective.** With static scheduling, the resources are allocated to tasks even if they are not being used. This can lead to wasted resources. With dynamic scheduling, resources are only allocated to tasks when they are needed. This can help to improve the cost-effectiveness of the application.
9. **Static scheduling is more predictable, while dynamic scheduling is less predictable.** With static scheduling, the resources are allocated to tasks in a predictable way. This makes it easier to plan for future demand. With dynamic scheduling, the resources are allocated to tasks in an unpredictable way. This can make it more difficult to plan for future demand.
10. **Static scheduling is more suitable for batch processing, while dynamic scheduling is more suitable for real-time applications.** Batch processing is a type of processing where tasks are submitted to a system and then processed in batches. Dynamic scheduling is not suitable for batch processing, as it can lead to delays in the processing of the batches. Real-time applications are applications where the response time is critical. Dynamic scheduling is suitable for real-time applications, as it can help to improve the response time.