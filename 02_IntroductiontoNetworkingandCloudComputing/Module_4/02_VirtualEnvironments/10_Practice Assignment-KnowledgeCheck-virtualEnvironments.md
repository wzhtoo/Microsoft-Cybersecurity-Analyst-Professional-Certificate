# Knowledge check: Virtual environments

[Knowledge check: Virtual environments 🔗](https://www.coursera.org/learn/introduction-to-networking-and-Cloud-computing/assignment-submission/RijZU/knowledge-check-virtual-environments)

1.  Question 1
    True or False: Hypervisors are essential for creating virtual servers, which are also known as virtual machines.

- **True**
  - That's correct! Hypervisors are essential for creating virtual servers. Without a hypervisor, creating and managing virtual machines on a single physical server is impossible.
- False

2. Question 2
   Which of the following is true about type 1 hypervisors? Select all that apply.

- **They provide a high level of security by isolating virtual machine partitions**

  - That's correct! Type 1 hypervisors are known for their high level of security because they isolate virtual machine partitions, making it impossible for one virtual machine to affect other virtual machines on the same physical server.

- **They are more efficient in resource sharing than type 2 hypervisors**
  - That's correct! Type 1 hypervisors are more efficient in resource sharing than type 2 hypervisors, as they have direct access to the host machine's physical resources.
- They are installed on top of an existing operating system.
- They are designed for desktop virtualization and testing.

3. Question 3
   Which of the following statements about Azure Spot Instances are true? Select all that apply.

- They are great for mission-critical applications
- **They can be used to run workloads that are not time sensitive**
  - That's correct! Azure Spot Instances can run workloads that are not time-sensitive and can be interrupted without significant impacts, such as batch processing, rendering, and testing.
- They are good for production applications
- **They are significantly discounted compared to regular VMs**
  - That's correct! Azure Spot Instances offer a significant discount compared to regular virtual machines because they are allocated from unused Azure compute capacity.

4. Question 4
   Based on their resource allocation which of the following virtual machines can be purchased from the Cloud providers based on their resource allocations? Select all that apply.

- Operating system-optimized virtual machines
- **Memory-optimized virtual machines**
  - That's correct! Memory-optimized virtual machines are designed for workloads that require a high amount of memory and fast memory performance, such as in-memory databases and analytics.
- **Burstable virtual machines**
  - That's correct! Burstable virtual machines provide a baseline level of CPU performance with the ability to burst to a higher level of CPU performance when needed, making them ideal for workloads with variable or unpredictable computing needs.
- Network-optimized virtual machines

5. Question 5
   Which of the following statements about the remote app streaming feature of Microsoft Azure virtual desktop are true? Select all that apply.

- It requires a separate virtual desktop for each remote app
- Remote apps cannot be used to print on client machines
- **It allows users to run individual applications remotely without accessing the full desktop**

  - That's correct! Remote app streaming allows users to access specific applications hosted on a remote virtual machine without accessing the full desktop environment.

- **It supports USB device redirection**
  - That's correct! Remote app streaming in Azure Virtual Desktop supports USB device redirection, allowing users to access local devices connected to the USB.
