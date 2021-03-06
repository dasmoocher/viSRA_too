# viSRAtoo
Viewing RNA expression on the gene and genome level using sequencing reads in the SRA database
## Please cite our work -- here is the ICMJE Standard Citation:

### ...and a link to the DOI:

## Awesome Logo

### You can make a free DOI with zenodo <link>

## Website (if applicable)

## Intro statement
*The future of biomedical research depends on the ability to rapidly access and analyze Next-Generation Sequencing (NGS) data stored at the NCBI’s Sequence Read Archive (SRA). NGS provides an unprecedented level of resolution, allowing researchers to ask previously unanswerable questions such as how cancer pathogenesis might be mediated by very small changes in gene expression.*

*With ~3 million records currently stored in the SRA database, and submissions growing exponentially, the SRA collection represents a treasure-trove of data to be mined by academia and industry. The information contained in a single SRA dataset is equivalent to hundreds of in vitro experiments worth of work, potentially saving thousands of dollars and research hours.*

*Here we present viSRA, a tool for visualizing RNA-seq data from SRA datasets on the fly. There are a variety of tools to analyize and visualize microarray data, and these can be leveraged to accelerate development of feature rich RNA-Seq tools. viSRA facilitates the interrogation of SRA datasets for differential gene expression via dockerized pipeline. viSRA makes it easy for biologists to perform pathway enrichment analyses and to interrogate which genes are differentially expressed between experiments. viSRA benefits greatly from previous work on deSRA and the MicroArrayPipeline*

## What's the problem?
*The NCBI Sequence Read Archive (SRA) provides NGS data along with sample and project metadata (NCBI Resource Coordinators 2017). As part of the International Nucleotide Sequence Database Collaboration, the SRA supports access to data from a wide variety of experimental types and sequencing instruments. Unfortunaltely, it can be time-consuming and difficult to access and analyze the data, especially if you want to quickly develop meaningful hypotheses. viSRA bridges this gap between advanced bioinformatic data and users.*

## Why should we solve it?
*The amount of NGS data stored in the Sequence Read Archive (SRA) data-base is growing rapidly. However, many researchers who are interested in this data do not have experience with the tools necessary to analyze it effectively. viSRA increases the utility and return on investment of NGS projects by making the data more accessible to a wider range of individuals.*

# What is <this software>?

![Overview Diagram](https://github.com/dasmoocher/viSRAtoo/blob/master/images/viSRA_workflow.png)

# How to use <this software>

## Installation options:

We provide two options for installing <this software>: Docker or directly from Github.

### Docker

The Docker image contains <this software> as well as a webserver and FTP server in case you want to deploy the FTP server. It does also contain a web server for testing the <this software> main website (but should only be used for debug purposes).

1. `docker pull ncbihackathons/<this software>` command to pull the image from the DockerHub
2. `docker run ncbihackathons/<this software>` Run the docker image from the master shell script
3. Edit the configuration files as below

### Installing <this software> from Github

1. `git clone https://github.com/NCBI-Hackathons/<this software>.git`
2. Edit the configuration files as below
3. `sh server/<this software>.sh` to test
4. Add cron job as required (to execute <this software>.sh script)

### Configuration

```Examples here```

# Testing

We tested four different tools with <this software>. They can be found in [server/tools/](server/tools/) . 

# Additional Functionality

### DockerFile

<this software> comes with a Dockerfile which can be used to build the Docker image.

  1. `git clone https://github.com/NCBI-Hackathons/<this software>.git`
  2. `cd server`
  3. `docker build --rm -t <this software>/<this software> .`
  4. `docker run -t -i <this software>/<this software>`
  
### Website

There is also a Docker image for hosting the main website. This should only be used for debug purposes.

  1. `git clone https://github.com/NCBI-Hackathons/<this software>.git`
  2. `cd Website`
  3. `docker build --rm -t <this software>/website .`
  4. `docker run -t -i <this software>/website`
  
