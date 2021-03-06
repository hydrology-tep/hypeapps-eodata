## Developer Cloud Sandbox hypeapps-historical application  

H-TEP Hydrological Modelling Thematic Application  - Pre-processing of EO data from TEP EO data applications to enable assimilation in the hydrological model Niger-HYPE.

## Quick link
 
* [Getting Started](#getting-started)
* [Installation](#installation)
* [Submitting the workflow](#submit)
* [Community and Documentation](#community)
* [Authors](#authors)
* [Questions, bugs, and suggestions](#questions)
* [License](#license)
* [Funding](#funding)

### <a name="getting-started"></a>Getting Started 

To run this application you will need a Developer Cloud Sandbox that can be requested at support (at) terradue.com

A Developer Cloud Sandbox provides Earth Sciences data access services, and helper tools for a user to implement, test and validate a scalable data processing application. It offers a dedicated virtual machine and a Cloud Computing environment.
The virtual machine runs in two different lifecycle modes: Sandbox mode and Cluster mode. 
Used in Sandbox mode (single virtual machine), it supports cluster simulation and user assistance functions in building the distributed application.
Used in Cluster mode (a set of master and slave nodes), it supports the deployment and execution of the application with the power of distributed computing for data processing over large datasets (leveraging the Hadoop Streaming MapReduce technology). 

### <a name="installation"></a>Installation

#### Pre-requisites

Requirements of the application in terms of software packages:

* miniconda
* cioppy
* R and following R packages:

To install these packages, run the simple steps below on the Developer Cloud Sandbox shell:

```bash
sudo yum install -y miniconda
sudo conda install -y cioppy
sudo conda install 
```

##### Using the releases

Log on the Developer Cloud Sandbox.

Install the package by running this command in a shell:

```bash
sudo yum -y install hypeapps-historical
```

> At this stage there are no releases yet

#### Using the development version

Install the pre-requisites as instructed above.

Log on the Developer Cloud Sandbox and run these commands in a shell:

```bash
git clone https://github.com/dgustafsson/hypeapps-historical
cd hypeapps-historical
mvn install
```

### <a name="submit"></a>Submitting the workflow

To submit the application with its default parameters, run the command below in the Developer Cloud Sandbox shell:

```bash
ciop-run
```
Or invoke the Web Processing Service via the Sandbox dashboard.

### <a name="community"></a>Community and Documentation

To learn more and find information go to 

* [Developer Cloud Sandbox](http://docs.terradue.com/developer-sandbox/)  

### <a name="authors"></a>Authors (alphabetically)

* David Gustafsson  ( david [dot] gustafsson [at] smhi [dot] se )
* Jafet Andersson   ( jafet [dot] andersson [at] smhi [dot] se )
* Frida Gyllensvärd ( frida [dot] gyllensvard [at] smhi [dot] se )

### <a name="questions"></a>Questions, bugs, and suggestions

Please file any bugs or questions as [issues](<app-url>) or send in a pull request if you corrected any.

### <a name="license"></a>License

Licensed under the GNU Lesser General Public License, Version 3.0: https://www.gnu.org/licenses/lgpl-3.0.en.html

### <a name="funding"></a>Funding

Put here any information about the funding.
