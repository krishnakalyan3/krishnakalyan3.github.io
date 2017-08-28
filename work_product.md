# Automating Performance Tests in Apache SystemML

# All my PRs below

## Getting Started

- https://github.com/apache/systemml/pull/500
- https://github.com/apache/systemml/pull/501
- https://github.com/apache/systemml/pull/502
- https://github.com/apache/systemml/pull/516
- https://github.com/apache/systemml/pull/560

Before GSoC begain I started by working on easy issues. These pull requests were a way for me to get familiar with the review process and bond with the community effectively.

## GSoC : Major Pull Requests

- https://github.com/apache/systemml/pull/537
- https://github.com/apache/systemml/pull/575
- https://github.com/apache/systemml/pull/604

As stated in the proposal at the end of every phase our work had to be merged with the master. For phase 1 we finished the automation of performance test suit. Phase 2 required us to work on adding HDFS support and extra configuration parameters. Phase 3 was about consolidation and plotting results. We also got access to 3 node cluster from IBM to run our performance tests.

## Minor Fixes

- https://github.com/apache/systemml/pull/615
- https://github.com/apache/systemml/pull/616
- https://github.com/apache/systemml/pull/624
- https://github.com/apache/systemml/pull/563

These pull requests are minor changes and bug fixes in out performance tests. Along with code we also created a performance test documentation.

Birds Eye View of the Work Done:

#### Phase 1:

- [x] Generate Data
- [x] Test all algorithms with `singlenode` 
- [x] Test all algorithms `spark-hybrid` execution mode  
- [x] Capture Time Taken
- [x] Generate a full set of plain text reports
- [x] Test automatic benchmark end to end

following algorithms included in the performance test suit

- [x] Clustering 
- [x] Binomial
- [x] Multinomial
- [x] Regression1
- [x] Regression2
- [x] Stats1
- [x] Stats2

#### Phase 2:

- [x] Decouple systemml-spark-submit.py
- [x] Decouple systemml-standalone.py
- [x] Refractor perf test suit to accept args like debug, stats, config etc...
- [x] Add HDFS support
- [x] Google Docs support for consolidation and comparison of our results
- [x] Compare SystemML with previous versions
- [x] Pylint, Comment
- [x] Extra arguments configuration Test
 -- Test parameters
 -- Backend parameters
 -- SystemML parameters
- [x] Windows Test
- [x] Documentation Update
- [x] systemml standalone comments
- [x] systemml spark submit comments

#### Phase 3:
- [x] Offline CSV support
- [x] Plots comparing algorithm performance across different releases
- [x] End to End Performance Test
-- Local System
-- `3` node Hadoop Cluster


Highlights:
- During the community bonding period, I had worked on a pull request (systemml-spark-submit.py) which gave me the confidence and knowledge to complete phase 1 tasks.
- I had an oppurtunity to present my work to all committers.

Challenges:
- Initially beginning it was quite difficult to come up with a good general architecture for the performance test suit. This was because I did not understand all the parameters completely and some data generation scripts / algorithms did not have 1 to 1 mapping. This required me to rewrite code couple of times.
- For phase 2, I spent a lot of time on adding HDFS support. After my discussion with my mentor we came up with an easy solution which required me to add an extra parameter --config-dir.
- At the end of phase 2, we got access to 3 node cluster to run our performance test suit. The setup and configuration of the cluster had a learning curve.
