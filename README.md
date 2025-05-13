# cc
---

Cloudlet Scheduling Simulator using SimPy (Shortest Job First)

This project is a simulation of Cloudlet Scheduling in Cloud Computing using Shortest Job First (SJF) algorithm, built with the simpy discrete event simulation framework.

It demonstrates how cloudlets (tasks) are scheduled on virtual machines (VMs) using an SJF policy, where shorter jobs are prioritized first.

Features

Simulates task execution using the SimPy framework.

Supports multiple virtual machines (VMs).

Custom Shortest Job First (SJF) scheduler.

Simple console output to show task execution order and time.


Requirements

Python 3.x

SimPy


Install SimPy using pip:

pip install simpy

How It Works

1. Cloudlet: A unit of work with a specific instruction length.


2. VM: A Virtual Machine with a defined MIPS (Million Instructions Per Second) capacity.


3. SJF Scheduler: Sorts cloudlets by their length (shortest first) and schedules them in a round-robin manner across available VMs.



Project Structure

Cloudlet:    Represents a task with an instruction length.
VM:          Executes cloudlets using SimPy’s Resource.
SJFScheduler: Sorts and schedules cloudlets based on the SJF policy.
simulate():  Sets up the environment and runs the simulation.

Example Output

[0] VM-1 started Cloudlet-3(len=1000)
[1.0] VM-1 finished Cloudlet-3(len=1000)
[1.0] VM-2 started Cloudlet-2(len=2000)
[3.0] VM-2 finished Cloudlet-2(len=2000)
...

How to Run

Save the Python code to a file (e.g., sjf_simulation.py) and run it using:

python sjf_simulation.py

Customize

You can modify:

Number of VMs

MIPS values

Cloudlet lengths

Scheduling logic (e.g., switch to FCFS or Round Robin)


License

This project is open-source and available under the MIT License.
