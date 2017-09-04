[![Build Status](https://travis-ci.org/IBM/REPO.svg?branch=master)](https://travis-ci.org/IBM/REPO)
<!--![Bluemix Deployments](https://deployment-tracker.mybluemix.net/stats/CODE/badge.svg)-->

# Building a Recommender with Apache Spark & Elasticsearch
In this developer journey, we will create a scalable recommender system using Apache Spark and Elasticsearch.

[Explain briefly how things work].

When the reader has completed this journey, they will understand how to:

* Ingest and index user event data into Elasticsearch
* Load event data into Spark DataFrames and use Spark's machine learning library (MLlib) to train a
collaborative filtering recommender model
* Export the trained model into Elasticsearch
* Using a custom Elasticsearch plugin, compute user and _similar item_ recommendations and combine
recommendations with search and content filtering

![TODO - Architecture](doc/source/images/architecture.png)

## Flow
<!--Add new flow steps based on the architecture diagram-->
1. Step 1.
2. Step 2.
3. Step 3.
4. Step 4.
5. Step 5.

## Included components
* [Apache Spark](http://spark.apache.org/): An open-source, fast and general-purpose cluster computing system
* [Elasticsearch](http://elasticsearch.org): Open-source search and analytics engine 
* [Jupyter Notebooks](http://jupyter.org/): An open-source web application that allows you to
create and share documents that contain live code, equations, visualizations and explanatory text.

## Featured technologies
* [Data Science](https://medium.com/ibm-data-science-experience/): Systems and scientific methods to analyze
structured and unstructured data in order to extract knowledge and insights.
* [Artificial Intelligence](https://medium.com/ibm-data-science-experience): Artificial intelligence can be
applied to disparate solution spaces to deliver disruptive technologies.
* [Python](https://www.python.org/): Python is a programming language that lets you work more quickly
and integrate your systems more effectively.

<!--Update this section when the video is created-->
# Watch the Video
[![TODO - Video](http://img.youtube.com/vi/VIDEO/0.jpg)](https://www.youtube.com/watch?v=VIDEO)

# Steps
Use the ``Deploy to Bluemix`` button **OR** create the services and run locally.

## Deploy to Bluemix
<!--Update the repo and tracking id-->
[![Deploy to Bluemix](https://deployment-tracker.mybluemix.net/stats/CODE/button.svg)](https://bluemix.net/deploy?repository=https://github.com/IBM/REPO.git)

1. Press the above ``Deploy to Bluemix`` button and then click on ``Deploy``.

<!--optional step-->
2. In Toolchains, click on Delivery Pipeline to watch while the app is deployed. Once deployed, the app can be viewed by clicking 'View app'.
![](doc/source/images/toolchain-pipeline.png)

<!--update with service names from manifest.yml-->
3. To see the app and services created and configured for this journey, use the Bluemix dashboard. The app is named `APP` with a unique suffix. The following services are created and easily identified by the `APP-` prefix:
    * TODO

## Run locally
> NOTE: These steps are only needed when running locally instead of using the ``Deploy to Bluemix`` button.

1. [Clone the repo](#1-clone-the-repo)
2. [Set up Elasticsearch](#2-set-up-elasticsearch)
3. [Download the Elasticsearch Spark connector](#3-download-the-elasticsearch-spark-connector)
4. [Download Apache Spark](#4-download-apache-spark)
5. [Run the Notebook](#5-run-the-notebook)

### 1. Clone the repo

Clone the `REPO` locally. In a terminal, run:

```
$ git clone https://github.com/IBM/REPO
```

We’ll be using the file [`data/conversation/workspaces/banking.json`](data/conversation/workspaces/banking.json) and the folder
[`data/conversation/workspaces/`](data/conversation/workspaces/)

### 2. Set up Elasticsearch

TODO

### 3. Download the Elasticsearch Spark connector

TODO

### 4. Download Apache Spark

Launch the **Watson Discovery** tool. Create a **new data collection**
and give the data collection a unique name.

> Save the **environment_id** and **collection_id** for your `.env` file in the next step.

Under `Add data to this collection` use `Drag and drop your documents here or browse from computer` to seed the content with the five documents in `data/discovery/docs`.

### 5. Run the Notebook

TODO
> Note: TODO

# Sample output

![TODO - output](doc/source/images/sample_output.png)

# Links
* [Demo on Youtube](https://www.youtube.com/watch?v=VIDEO)

# Troubleshooting

* Error: XYZ

  > Solution

* Error: ABC

  > Solution

<!--keep this-->

# License
[Apache 2.0](LICENSE)

<!--This can stay as-is if using Deploy to Bluemix-->

# Privacy Notice
If using the `Deploy to Bluemix` button some metrics are tracked, the following
information is sent to a [Deployment Tracker](https://github.com/IBM-Bluemix/cf-deployment-tracker-service) service
on each deployment:

* TODO

## Disabling Deployment Tracking

To disable tracking, TODO
