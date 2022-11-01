<!--Score ReadMe-->

<br />

<p align="center"><a href="https://www.overture.bio/" target="_blank"><img src="Overture_logo.png" width="66%"></a></p>

<br />

<!-- Replace slack with discourse once setup -->

[<img src="https://img.shields.io/badge/chat-on--slack-blue">](http://slack.overture.bio) 
[<img src="https://img.shields.io/badge/License-gpl--v3.0-blue">](https://github.com/overture-stack/score/blob/develop/LICENSE)

## Worry Less Science More

In this Overture repository, we (the [OICR Genome Informatics Team](https://softeng.oicr.on.ca/team/)) develop the [Score](https://www.overture.bio/products/score/) data transfer and storage microservice. 

[Overture](https://www.overture.bio/) is an ensemble of open-source, modular solutions for big-data genomic science. Our core products work in concert to manage, explore and visualize molecular and clinical data. Visit our [website](https://www.overture.bio/) for more information on what Overture offers, and check out our other projects on [GitHub](https://github.com/overture-stack/).

## Score - Seamless Data Transfer & Storage

<!--State the problem-->

<br />

<img width="22%" align="left" alt="Data transfer and storage" src="score-padded.png">

Using the Score client, data providers upload files to their cloud storage system. Conversely, published data gets downloaded by data consumers.

With the falling cost of sequencing, research organizations are producing enormous multi-omics data sets for many cancer types. Along with this molecular data comes a growing amount of matched clinical data, such as patient records, histology images, and radiographic imagery. Furthermore, the global research community cannot access a large portion of this data due to its geographic distribution. Therefore, cancer researchers require new and innovative data management and data-sharing tools.

<!--State our solution-->
<!--Do we have any statistics for this?-->

<!--Provide a brief outline of how/what we do to reach this solution-->

**We created Score to solve these concerns by:**
- Managing secure and fast data uploads/downloads to any cloud-based storage system
- Facilitating file bundling and resumable uploading and downloading
- Providing built-in slicing of BAM and CRAM files with integrated command line tools
- Using MD5sum verification to ensure data integrity

<!--Where has it been used-->

Score is used in various initiatives, including the Cancer Genome Collaboratory, which employs Score and Song ([see related products](#related-products)) to manage nearly 1 petabyte of raw and analyzed data (121,000 files).

## Related Products 

<p align="left" ><img alt="Overture overview" src="https://www.overture.bio/static/124ca0fede460933c64fe4e50465b235/a6d66/system-diagram.png"></p>

Score is a data transfer management system that focuses on data uploads and downloads rather than the intricacies of file metadata validation. Score works with a companion program, Song, to address this. Song is responsible for evaluating file information, assigning unique global identifiers, and determining open versus controlled file access permissions. As Song manages metadata, it communicates with Score, which handles the files on an object storage system. 

## Table of Contents

- [Setup](#setup)
- [Usage](#usage)
- [Contribution](#how-to-contribute)
- [Feedback](#feedback)
- [Code of Conduct](#code-of-conduct)
- [License](#license)

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
