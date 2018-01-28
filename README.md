# Stream Data into Hadoop using Flume

## Problem

We all know that [Sqoop](https://a-djebali.github.io/hadoop-sqoop-data-aggregation/) is a component used to transfer structured data from RDBMS like databases (e.g. MySQL, SQL Server, ect.) to Hadoop HDFS and vice versa (from HDFS to RDBMS). Now, what if we want to load semi-structured and unstructured data into Hadoop HDFS, or live streaming data that is generated from sources like twitter, facebook, weblogs and more into Hadoop HDFS.

## Solution (Proposition)

The [solution](https://a-djebali.github.io/hadoop-flume-stream-data/) to the challenge in the Hadoop ecosystem is [Flume](https://flume.apache.org/), which is a component used to collect, aggregate and moves large amount of log data from different sources to a centralized data store. It is an open source component which is designed to locate and store the data in a distributed environment and collects the data as per the specified input key(s).

## Prerequisites 

* Hadoop
* Flume
* Streaming data source 

## Solution Architecture 

Before moving forward and deploy the data pipeline using Flume, It is mandatory to know its architecture. In this project, we used Flume to collect data from the Twitter Streaming API and forward it to HDFS. Looking closer at the Flume pipeline from that example, we come away with a system like this:

![Data Pipeline Architecture using Flume](https://raw.githubusercontent.com/a-djebali/a-djebali.github.io/master/images/flume-architecture.png)

## Deployment (step by step)

In this [blog](https://a-djebali.github.io/hadoop-flume-stream-data/) you find a very easy and detailed walk through. And if you already have an idea on how to implement this, you can find the configuration that has been used for this project [here](twitter.conf)