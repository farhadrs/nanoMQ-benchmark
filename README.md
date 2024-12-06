# nanoMQ-benchmark
This is a simulation of benchmarking the performance of nanoMQ in a multi-region, multi-broker scenario.

NanoMQ Multi-Region Multi-Broker Performance Benchmark Simulation
This repository contains the setup and configuration for benchmarking the performance of NanoMQ in a multi-region, multi-broker scenario. The purpose of this simulation is to evaluate NanoMQ’s performance in a distributed MQTT broker environment across multiple regions (subnets) to simulate real-world deployment scenarios, focusing on aspects such as connectivity, performance, and reliability.

# Overview
NanoMQ is a high-performance MQTT broker designed for IoT and edge applications. In this setup, multiple instances of NanoMQ are deployed in different regions (subnets), and communication between the brokers is simulated. Each broker in a region will be set up as a container, and the system will be benchmarked based on metrics such as latency, message throughput, and resilience.

# Objectives
Simulate a multi-region setup with multiple brokers (NanoMQ) deployed across separate subnets.
Test the performance of NanoMQ in a distributed environment across regions.
Benchmark key metrics such as message latency, throughput, and broker-to-broker communication.
Test MQTT bridge connections between brokers across regions.
Evaluate the scalability and resilience of NanoMQ in a distributed setup.
Architecture
The architecture consists of three brokers (broker-a, broker-b, and broker-c), each deployed in separate regions (subnets). These regions are:

Region A: 10.0.0.0/16
Region B: 10.1.0.0/16
Region C: 10.2.0.0/16
Each broker is assigned a unique IP within its region:

Broker A: 10.0.0.2
Broker B: 10.1.0.2
Broker C: 10.2.0.2

These brokers are connected via bridge connections, allowing them to communicate across different regions, replicating a real-world IoT application environment where different services and devices are distributed across multiple locations.
