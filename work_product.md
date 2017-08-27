# Automating Performance Tests in Apache SystemML

# All my PRs below

## Getting Started
https://github.com/apache/systemml/pull/500
https://github.com/apache/systemml/pull/501
https://github.com/apache/systemml/pull/502
https://github.com/apache/systemml/pull/516
https://github.com/apache/systemml/pull/560

Before GSoC begin I made started working on easy issues. The getting started pull requests were a way for me to get famaliar with the review process and bond with the community.

## GSoC : Phase wise pull requests
https://github.com/apache/systemml/pull/537
https://github.com/apache/systemml/pull/575
https://github.com/apache/systemml/pull/604

As stated in the proposal at the end of every phase our work was merged with the master. For phase 1 finished the automation of performance test suit. Phase 2 required us to work on adding HDFS support and extra configuration parameters. Phase 3 was about consolidation and plotting results. We also got access to 3 node cluster from IBM to run our performance tests.

## Minor Fixes
https://github.com/apache/systemml/pull/615
https://github.com/apache/systemml/pull/616
https://github.com/apache/systemml/pull/624
https://github.com/apache/systemml/pull/563

These pull requests are minor changes and bug fixes in out performance tests. Along with the code we also created a performance test documentation. 

Work Done:
- Automation of performance test suit
- Integration of parameters
	- Test parameters
	- Backend parameters
	- SystemML parameters
- Google docs / offline support for consolidation and comparison of our results

Pending Items:
- All the tasks as mentioned in the proposal are complete. 

Highlights:
- During the community bonding period, I had worked on a pull request (systemml-spark-submit.py) which gave me the confidence and knoweldge to complete phase 1 tasks.
- I had an oppurtunity to present my work to all committers.

Challenges:
- At the begining it was difficult to come up with a good general architecture for the performance test suit. This was because I did not understand all the parameters completely. Hence I had to rewrite code couple of times.
- I needed to understand all the parmeter for all the algorithms to create an automated performance test suit. Some datagen scripts and algorithms did not have 1 to 1 mapping. This was difficult for me to understand initially. 
- For phase 2, I spent a lot of time on adding HDFS support. After my discussion with my mentor we came up with an easy solution which required me to add an extra parameter --config-dir.
- At the end of phase 2, we got access to 3 node cluster to run our performance test suit. The setup and configuration of the cluster had a learning curve.
