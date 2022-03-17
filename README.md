# Analytics 2: Introduction to the command-line for Bioinformatics

## Course Content



This course offers an introduction to working with Linux. We will describe the Linux environment so that participants can start to utilize command-line tools and feel comfortable using a text-based way of interacting with a computer. We give example of processing data arising from Next-Generation Sequencing experiments, in particular an RNA-seq experiment.

## Pre-requisites

No prior programming experience is required. Computers will be provided. You can bring your own laptop to the workshop if you wish but it will need a working wi-fi connection and you will have to let the tutor know in advance so a temporary York password can be created for you.

## Learning Outcomes

After this course you should be able to:

- Connect to a Unix / Linux system
- Navigate around a file system by issuing commands; rather than using a Desktop environment
- Move and copy files and directories within the Linux system
- Work with text files
- Run programs from the command-line
- Run quality assessment tools on data derived from High-throughput sequencing experiments
- Write short scripts to document an analysis

## Schedule (Provisional)

- 10:00 - 10:30 Course Setup
- 10:30 - 12:45 Introduction to the command line
- 13:30 - 14:30 Obtaining sequencing data and assessing quality
- 14:30 - 16:00 Aligning sequencing data and quantification

## Amazon

- ami-0f9124f7452cdb2a6
- User data
```
#!/bin/bash

sudo apt-get update
sudo apt-get install -y docker.io
sudo service docker start
sudo usermod -aG docker $username
sudo docker pull markdunning/rnaseq-toolbox
docker run -p 6080:80 markdunning/rnaseq-toolbox
```
