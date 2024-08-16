# Apache Kafka Setup and Usage Guide

This document provides a detailed guide to setting up and using Apache Kafka on your system, including example commands and outputs.

## Table of Contents
- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Starting Kafka Services](#starting-kafka-services)
  - [Starting ZooKeeper](#starting-zookeeper)
  - [Starting Kafka Broker](#starting-kafka-broker)
- [Basic Kafka Commands](#basic-kafka-commands)
  - [Creating Topics](#creating-topics)
  - [Listing Topics](#listing-topics)
  - [Describing a Topic](#describing-a-topic)
  - [Producing Messages](#producing-messages)
  - [Consuming Messages](#consuming-messages)
- [Troubleshooting](#troubleshooting)
- [Outputs and Examples](#outputs-and-examples)

## Introduction

Apache Kafka is an open-source distributed event streaming platform used by thousands of companies for high-performance data pipelines, streaming analytics, data integration, and mission-critical applications.

## Prerequisites

- Java 8+ installed on your system.
- Kafka downloaded and extracted to your desired directory.
- Basic understanding of terminal commands.

## Setup

Download and extract Kafka from the [Apache Kafka download page](https://kafka.apache.org/downloads). Make sure you have the correct version that matches your system's architecture.

## Starting Kafka Services

### Starting ZooKeeper

Kafka uses ZooKeeper to manage its cluster state. Start ZooKeeper using the following command:

```bash
sahil@:/mnt/f/kafka_2.12-3.8.0/kafka_2.12-3.8.0$ bin/zookeeper-server-start.sh config/zookeeper.properties
