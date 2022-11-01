<!--Score ReadMe-->

<br />

<p align="center"><a href="https://www.overture.bio/" target="_blank"><img src="Overture_logo.png" width="66%"></a></p>

<br />

<!-- Replace slack with discourse once setup -->

[<img src="https://img.shields.io/badge/chat-on--slack-blue">](http://slack.overture.bio) 
[<img src="https://img.shields.io/badge/License-gpl--v3.0-blue">](https://github.com/overture-stack/score/blob/develop/LICENSE)

## Worry Less Science More

In this Overture repository, we (the [OICR Genome Informatics Team](https://softeng.oicr.on.ca/team/)) develop the [Score](https://www.overture.bio/products/score/) data transfer and storage microservice. 

[Overture](https://www.overture.bio/) is an ensemble of open-source, modular solutions made for big-data genomic science. Our core products work in concert to manage, explore and visualize molecular and clinical data. Visit our [website](https://www.overture.bio/) for more information on what Overture has to offer, and check out our other projects on [GitHub](https://github.com/overture-stack/).

## Score - Seamless Data Transfer & Storage



<!--State the problem-->



<br />

<img width="33%" alt="Data transfer and storage" src="score-padded.png">

Using the Score client data providers can upload files to their cloud storage system. Conversly, published data can be downloaded by data consumers. 

With the decreasing cost of sequencing, research groups are generating large [multi-omics](https://www.illumina.com/techniques/popular-applications/multiomics.html#:~:text=Multiomics%20approaches%20that%20combine%20methylation,complex%20pathways%20and%20disease%20mechanisms.) data sets for various cancer types. Along side this molecular data is an ever increasing amount of paired clinical data including but not limited to patient records, histological imagery and radiological imagery. Furthermore, much of this data is geographically distributed and inaccessible to the global research community. Therefore, the cancer research community requires new and innovative data management and data sharing tools.

<!--State our solution-->
<!--Do we have any statistics for this?-->

<!--Provide a brief outline of how/what we do to reach this solution-->

Score was developed to address these issues by:
- Securley managing fast data uploads/downloads to any cloud based storage system
- Facilitating file Bundling as well as multi-part, parallel and resumable uploads/downloads
- Providing built-in slicing of BAM/CRAM files with integrated command line tools
- Ensuring data integrety with MD5sum verification

Currently Score, along with Song ([see related products](#related-products)) manages over 1 petabyte of raw and interpreted data (121,000 files) on the Cancer Genome Collaboratory alongside Amazon S3. 


<!--This is one of many partnered projects, in perspective, it is approximated that 50 petabytes can hold the entire written works of mankind, through all of recorded history, in every language.-->





## Related Products 

<p align="left" ><img alt="Overture overview" src="https://www.overture.bio/static/124ca0fede460933c64fe4e50465b235/a6d66/system-diagram.png"></p>

As a data transfer management system, Score is focused on managing data upload and download, and does not handle the complexities of file metadata validation. To handle this, Score is built to interact with a required companion application, [Song](). Song is responsibe for validating file metadata, assigning unique global identifiers for data management, assigning permisssions for open (public) versus controlled (authentication required) file access. As Song manages metadata, it communicates with Score which manages the files on an object storage system. By defining new metadata shemas, all file types (sequencing read, variant calls, radiology imagies) can be supported through Song.

## Table of Contents

- [Quick Start](#quickstart)
- [Setup](#setup)
- [Usage](#usage)
- [Contribution](#how-to-contribute)
- [Feedback](#feedback)
- [Code of Conduct](#code-of-conduct)
- [License](#license)


## Quick Start

This is a step-by-step guide for setting up a dockerized version of Ego. See our [setup section](#setup) below for a comprehensive setup guide.

**1.** Set up a google oauth client app ([see here](https://www.overture.bio/documentation/ego/installation/prereq/#google)). 

## Setup

Please see the documentation linked below:

- [Setup Prerequisites](https://www.overture.bio/documentation/score/installation/installation/)
- [Installation](https://www.overture.bio/documentation/score/installation/installation/#installation)
- [Configuration](https://www.overture.bio/documentation/score/installation/configuration/)
- [Authentication](https://www.overture.bio/documentation/score/installation/authentication/)

## Usage

Please see the documentation linked below:

- [Setting up the score client](https://www.overture.bio/documentation/score/user-guide/client-setup/)
- [Uploading Data](https://www.overture.bio/documentation/score/user-guide/upload/)
- [Downloading Data](https://www.overture.bio/documentation/score/user-guide/download/)
- [Command Reference](https://www.overture.bio/documentation/score/user-guide/commands/)


## Contribute

* [Making a Contribution](CONTRIBUTING.md)
* [Filing an issue](https://github.com/overture-stack/score/issues)

## Feedback

* Connect with us on [Slack](http://slack.overture.bio)
* [Upvote](https://github.com/overture-stack/score/issues?q=is%3Aopen+is%3Aissue+label%3Anew-feature+sort%3Areactions-%2B1-desc) feature requests

## Code of Conduct

&emsp; [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)

## License

Licensed under the [GNU Lesser General Public License v3.0](LICENSE.txt) license.
