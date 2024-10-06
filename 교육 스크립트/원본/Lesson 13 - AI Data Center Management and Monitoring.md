# Lesson 13 - AI Data Center Management and Monitoring

0:07
Welcome to unit 13. In this unit, we'll be covering tools for management and monitoring AI clusters.
Play video starting at ::15 and follow transcript0:15
In this unit, we'll begin with an overview of cluster management and monitoring. We'll discuss infrastructure provisioning and management and monitoring for resources and workloads. Finally, we'll give an overview of NVIDIAs base command manager software.
Play video starting at ::32 and follow transcript0:32
By the end of this unit you'll be able to, identify the general concepts about provisioning, managing, and monitoring AI infrastructure. Describe the value of cluster management tools. Describe the concepts for ongoing monitoring and maintenance. And identify tools that are used for provisioning, management, and monitoring.
Play video starting at ::52 and follow transcript0:52
There are three main concepts to consider when considering managing AI infrastructure. First is infrastructure provisioning. Provisioning is the process of setting up and configuring hardware. This includes the servers, switches, storage, and any other components of the AI cluster.
Play video starting at :1:9 and follow transcript1:09
The next concept is resource management and monitoring. This includes getting metrics and data from the resources in the cluster to determine how the cluster is performing and to make any updates or changes. The final concept is workload management and monitoring. This is how we ensure the data scientists and AI practitioners have the tools they need and understand the usage of the cluster. In the rest of this unit, well discuss these concepts in more detail and discuss some tools that can be used to accomplish the related tasks.
Play video starting at :1:42 and follow transcript1:42
In this section, we'll talk about infrastructure provisioning.
Play video starting at :1:47 and follow transcript1:47
Once the infrastructure is installed in the data center or procured in the cloud, the hardware needs to be provisioned before it can be used.
Play video starting at :1:56 and follow transcript1:56
The installed hardware may not have the latest or correct versions of software or firmware installed by default. The versions necessary will be dependent on the collective components in the data center and the workload needs.
Play video starting at :2:9 and follow transcript2:09
In preparation for provisioning, the correct versions of software and firmware must be determined and downloaded.
Play video starting at :2:16 and follow transcript2:16
Once the firmware and software are retrieved, the systems can be updated.
Play video starting at :2:21 and follow transcript2:21
This can include the operating system, GPU drivers, networking drivers, management tools, and any applications that need to be run on the servers, switches, and storage. The process can also include updating firmware for the hardware. When provisioning is complete, the compute nodes, GPU's storage, and networking should be ready for workloads to be run on the system.
Play video starting at :2:46 and follow transcript2:46
There are several tools available for provisioning servers and systems. Ansible is an open source command line IT automation software application that can configure systems and deploy software.
Play video starting at :2:59 and follow transcript2:59
Terraform is an infrastructure as code tool that lets you define both cloud and on-prem resources.
Play video starting at :3:6 and follow transcript3:06
Foreman is an open source project that helps system administrators manage servers throughout their lifecycle, from provisioning and configuration to orchestration and monitoring. In addition to the tools mentioned here, there are many other tools for on prem and cloud based provisioning and configuration.
Play video starting at :3:26 and follow transcript3:26
Next we'll talk about resource management and monitoring.
Play video starting at :3:31 and follow transcript3:31
Managing and monitoring resources in a data center go hand in hand. There are standard maintenance tasks that must be done for the data center systems. Monitoring these systems can give insights into which systems might need attention beyond regular maintenance. Managing resources like compute nodes, network fabric, and other cluster components is critical to keeping a high performance cluster operating at its best. Let's discuss some of the monitoring and management tasks for an AI cluster.
Play video starting at :3:59 and follow transcript3:59
For the compute nodes, the overall system health of the nodes should be monitored as well as metrics on any special hardware like GPUs. Management tasks include installing patches and updates for security flaws, keeping the firmware up to date, installing and maintaining drivers, and replacing failing components.
Play video starting at :4:18 and follow transcript4:18
Network congestion, connection quality and connectivity across the network should be monitored. This provides information on possible network issues like cable degradation or lost connections that could require changing out faulty cables. In addition, as workloads change or the cluster grows, the networking topology, bandwidth, or other factors may need to be upgraded.
Play video starting at :4:41 and follow transcript4:41
In addition to the compute nodes and the networks, other cluster components such as storage and maintenance nodes need to be monitored and managed. This includes monitoring disk space usage and the health of management nodes. Management also includes ensuring that management node software stays updated, that cloud and on-prem tools work together, and that the correct users are authorized and able to access and use the cluster.
Play video starting at :5:9 and follow transcript5:09
Depending on the configuration and servers in an AI cluster, there are a variety of tools that can be used for management and monitoring.
Play video starting at :5:17 and follow transcript5:17
Redfish, by the distributed management task force, is a standard designed to deliver simple and secure management of servers, networks, storage devices, and other infrastructure. It can be used for many of the management tasks in an AI data center.
Play video starting at :5:32 and follow transcript5:32
For data centers with NVIDIA GPUs, the data center GPU management, or DCGM exporter tool, is a tool based on the Go APIs to NVIDIA DCGM that that allows users to gather GPU metrics and understand workload behavior or monitor GPUs in clusters.
Play video starting at :5:51 and follow transcript5:51
Prometheus is an open source monitoring system that collects and stores metrics. It works in connection with Grafana, a tool used to visualize time series data. As with provisioning, there are a multitude of management and monitoring tools available for AI clusters. We only shared a small subset of the tools here.
Play video starting at :6:11 and follow transcript6:11
Next, we'll talk about workload management and monitoring.
Play video starting at :6:16 and follow transcript6:16
Workload management and monitoring are critical tasks in an AI cluster. Workload management includes tasks like making sure workloads get the resources they need to run. Having access to the necessary number of GPU's or CPU cores is critical. Once the needs are determined, the jobs must be scheduled to run on the compute nodes. If a job has an issue, it may need to be stopped and failed jobs may need to be restarted. Monitoring of workloads includes checking the efficiency of their resource usage. This can include if the GPUs and CPUs are being properly utilized, and if there are memory or storage concerns with certain workloads. Workload monitoring also includes monitoring the status of jobs to provide results or release resources back to the cluster.
Play video starting at :7:4 and follow transcript7:04
There are a variety of tools used for workload management. Many of these tools also include some monitoring capabilities or share job metrics with other tools. Some of the more common workload management tools are Kubernetes, Jupyter Lab, and Slurm.
Play video starting at :7:20 and follow transcript7:20
Kubernetes is an open source tool that manages and orchestrates containerized workloads. It has operators that allow it to work with NVIDIA GPUs, share metrics with Prometheus, and integrate with advanced schedulers like Run AI.
Play video starting at :7:35 and follow transcript7:35
Jupyter is an open source web application used by data scientists and machine learning professionals to create and share computational documents like code and data visualizations. It's an interactive web application that can be launched and run from within containers.
Play video starting at :7:51 and follow transcript7:51
Slurm is a tool created by SchedMD that's used to simplify resource sharing on large AI and HPC clusters. It's an advanced scheduling tool that can run interactive and batch jobs, prioritize jobs, and allows for resource reservations and per job quality of service settings.
Play video starting at :8:11 and follow transcript8:11
In the final section of this course, we'll give an overview of NVIDIA-based command manager, NVIDIAs set of tools to deploy and manage an AI data center.
Play video starting at :8:22 and follow transcript8:22
In the prior sections, we have discussed the importance provisioning, monitoring, and management needs for AI clusters and workloads. We've also discussed a variety of tools to handle these tasks. NVIDIA-base command manager, or BCM, is a comprehensive software system that can handle the tasks of provisioning, managing, and monitoring an AI data center. It handles infrastructure provisioning, user access and workload management, and resource monitoring, sets up networking, security, and DNS, and ensures cluster integrity. It also automates server management and updates, preventing server drift. BCM can deploy Kubernetes and Slurm, and other workload managers. It also allows for streamlined setup of Jupyter Lab. Finally, BCM has built-in job monitoring and metrics for GPUs and other cluster resources.
Play video starting at :9:16 and follow transcript9:16
Base command manager has a lot of capabilities that translate to three key value propositions. It one, accelerates time to value by simplifying infrastructure, bring up and workload provisioning so that data scientists can get resources they need quickly. Two, reduces complexity and effort by automating the management and operations of accelerated infrastructure. Three enables agility by streamlining the ability for the infrastructure to support many different types of workloads with dynamic resource allocation based on business needs. All of these benefit the whole AI team, from it to data scientists to line of business owners.
Play video starting at :9:55 and follow transcript9:55
Let's summarize what we've learned.
Play video starting at :9:59 and follow transcript9:59
Now that you've completed this unit, you should be able to identify the general concepts about provisioning, managing, and monitoring AI infrastructure. Describe the value of cluster management tools. Describe the concepts for ongoing monitoring and maintenance. And identify tools that are used for provisioning, management, and monitoring.
Play video starting at :10:20 and follow transcript10:20
Don't stop here, continue the learning journey with Unit 14, orchestration and scheduling. See you in the next unit.