---
title: Cloud Case Study Precis
keywords: summary, overview, case, study
last_updated: March 2, 2017
tags: [research_computing, data_science, case_studies, genomics]
summary: "Cloud Case Study Precis"
sidebar: mydoc_sidebar
permalink: ccs_precis.html
folder: ccs
---


## Introduction 


This page concisely describes public cloud use for research computing and data science at the University of Washington. 


We track close to 100 research projects using the public cloud for computing across issues of access, time, compute
power, storage, data management, cost and other issues.  The summary below is organized by domain. 
Our work in consulting and advocating for use of the public cloud is integrated with the mission and operation of
the UW eScience Institute.



## CC*IIE Remarks



### What are the impacts of the CC*IIE (NSF) sponsored projects? How has it contributed?


#### Preamble 


Much of the impact of this work is speculative. The general topic is public cloud computing applied
to research computing, broken down into smaller segments of work. These efforts were motivated as 
contributions to specific projects; and we comment on their impact on those projects. However the 
work was also carried out with the idea of solving broader recurring challenges.  For example we 
developed a push notification of cloud spending on AWS to catch unauthorized account use and runaway
resource allocation by student researchers; but this was in view of the fact that any research 
groupd taking advantage of the AWS cloud will benefit from the same mechanism. At-a-glance cost
summaries that arrive by email are easy to monitor in contrast with *every day* logging in to a 
cost tracking console and configuring a set of queries. The former process takes a matter of seconds, 
the latter requires 15 minutes.

A note on scale: The group responsible for the cloud adaptation work described here as supported by
NSF is tasked with supporting the entirety of University of Washington research including medicine. 
This large-scale proposition is currently manageable because cloud computing is a relatively new
technology that requires a certain investment of time to master. If we are on the verge of a phase
transition to large-scale cloud adoption then we are in the calm before the storm. We want to 
take advantage of the comparative lull to create as many pathways and patterns to successful 
cloud adoption in preparation for the increase in migration volume. This NSF-sponsored project
has been a windfall enabling us to bring in students and staff towards this end. 


#### Guiding concepts for this report 


- Discussion of data resources
- Acquisition of data skills
- Emergence of career paths (data scientists) 
- New disciplines


#### Cloud Computing Innovation and Cyber-Infrastructure Elements for Research Topics


- Data security
- Data sharing
- Computing at scale
- Institutional IT support for cloud adoption/migration
- Internet of Things in relation to the public cloud
- Student access to cloud platforms for research computing 
- Connectivity for high-speed data transfer from the lab to the cloud


### What is the impact on the development of the principal discipline(s) of the project?


To set the stage for our remarks on impact we describe a research transition to the cloud. 
Cloud computing represents a break with traditional research computing on 'owned resources'; 
and as such -- because of the perceived cost of change -- it requires considerable motivation 
to overcome social inertia. This motivation often originates from a desire to stop purchasing 
and maintaining computers. However the cloud has so many additional benefits that the 
inquisitive research team often finds there is more benefit from what the cloud *actually offers* 
than there is in *leaving behind* purchase orders and operating sytem patches. We call this
perceptual shift 'cloud socialization'.  Lastly it is important to note that a major impetus 
towards cloud socialization is the advent of cloud-hosted services. *GoogleDrive* is a typical
example but in the research the most impactful development has been the *Git* 
paradigm for open source code control, for example as embodied by *GitHub* repositories. 


We began discussion with a postdoc working within a well-funded molecular engineering laboratory.
This provided an opportunity to explore cloud computing scale as a means of solving two related
problems. First protein folding (the central research task) requires a huge number of computations to 
resolve peptide configuration in a search space of 10 trillion possible configurations. Second,
a research lab operating its own computers will experience intermittent resource demand with a
job queue. Our solution was to work with AWS representatives to harness a cluster technology
called **Batch** which enabled the postdoc to run a 2-week computation in 53 hours at a cost of
$3500. This cost is approximately 3x the corresponding cost on owned hardware. In strict terms
this means that the cloud is not cost competitive with owned hardware unless one or more of 
the following considerations comes into play:


- The researcher tasks owned compute resources at <= a 1/3 duty cycle
- The research scientist values their own time spent waiting for processing runs to start / complete
- There is more computation to be done than can be supported on owned resources
- The university hides or subsidizes cost of operations, for example power and HVAC
- The cost of cloud computing continues to drop, consistent with the current multi-year trend


Our engagement here had the impact of producing a library of ten million peptide structures in a
reference dataset that will be made publicly available. However the principle impact of this work
has been the documentation of the process within the *cloudmaven* resource corpus. By capturing
cloud adoption success stories such as this one we provide a means for addressing the scale of 
research computing cloud migration as the social phase transition accelerates over the next
decade. The methods described here will -- in the near term for this laboratory -- provide an 
alternative to standard computing practice that eliminates queue time and shortens the time
to complete processing runs. (The **AWS Batch** process secured 164 high-powered computers 
for the 53-hour duration of the compute task.)


To be very specific about how this effort drives a new approach in science: From molecular engineering
to genomics to the hydrology of high mountain Asia (all real projects we are involved in): 
Scientists tend to compute in bursts and the cloud is at cost parity with on-premise computers; 
the cloud is much much powerful than owned machines; the cloud is public and hence dissociated from 
any particular funding source or agency; and so the public cloud allows scientists to ask deeper and
more computationally intensive questions without purchasing a single extension cord; at the cost of 
the time investment to learn the procedures and services; and at the cost of just the resources
(computers) used. Cloud computing is a new solution for moving research forward, for coping
with the data deluge problem, for *not being constrained* by available compute resources. To this 
end we are documenting solutions and building a trans-disciplinary community of practice that is 
leading the way into this new solution. 



### What is the impact on other disciplines? 


This work included as one of its focus topics the security of data that are moved, managed and analyzed
on the public cloud. The cloud solution involves (particular to AWS) a virtual private cloud construct that
guarantees isolation of the data (i.e. unauthorized data access via internet is virtually impossible). 
Furthermore data encryption can be required and guaranteed (at rest and in motion) and access logging is 
facilitated to track parties that come into contact with the secured data. Together with best practices 
this ensemble of technologies essentially guarantees data security for a given project where the largest 
threat is (as one might expect) human error. 


A signal impact of our data security work can be cited from hydrological science: Proprietary data 
(for example river stage) received from countries can be sequestered on private subnetworks and used
to force or validate hydrological models with no risk of public dissemination of those data. 


Extending beyond hydrology and the proprietary 'national asset' nature of water resource data: Our 
group has been in contact with research teams from other disciplines looking for a cloud-based data
security template. These include researchers from clinical trial research, disease and epidemiology, 
laboratory medicine (for example annotation of genomic markers), genomics, demography, business, 
and data centers that have some degree of contact with sensitive data. Our progress in this area
is helping to build the cyberinfrastructure of data security on the public cloud. 


### What is the impact on the development of human resources? 


University IT staff are faced with a constantly shifting landscape of technology; which they are
obliged to filter through, understand, and pass along to a somewhat indifferent (or intransigent)
user community in the form of stable, reliable services. As a perceived edifice the public cloud
can present an intimidating prospect to IT staff: Rather than one or two new ideas, a given cloud 
provider can surface 100 or more new technologies. To hazard a normative statement in response
to this observation: It is incumbent on early cloud adopters -- be they researchers, IT staff, 
graduate students, undergraduates, or administrators -- to leave a well-documented path in the 
wake of their learning and solution-building projects. This path should emphasize 'how it was
done' but as importantly 'how a new person can learn the background -- in depth -- to do 
likewise.'


From this there follows a corollary: University administration must keep pace by providing for 
the training and hiring of IT staff in support of cloud computing. Research is a natural avenue 
for this growth because it is by its nature unbounded. The work carried out in this project 
produced a set of case studies with documentation; where the attempt has been to imply such 
a path, from cloud newcomer to cloud adept. The shift of training on the cloud will take 
diligence but we feel we have contributed some impetus to the process. Cloud working groups
and workshops for community of practice will be the follow-on sign posts as the effort 
continues. 


One further aspect of this sociological and technical shift deserves mention. 
The most flexible and adaptable demographic within the university community is (arguably) 
the student population.  It was therefore a natural choice to hire several students in the 
course of this work to take on tractable problems and build solutions; for example push
notifications of daily cloud expenditure. This approach proved to be extremely effective.
Further: Through a student computing organization these students have the opportunity to 
transfer their enthusiasm and technical skills for cloud computing to others; and thence 
into research groups and through the community in general. 


### What is the impact on physical resources that form infrastructure? 


Research teams are rapidly improving their table tennis skills, having emptied their server rooms and 
installed high-quality ping pong tables. 


### What is the impact on informational resources that form infrastructure? 


The GitHub repository-based [coudmaven.org](http://cloudmaven.org) website is the principle informational
resource proceeding from this work. The website captures basics of cloud computing, provides links to 
instructional resources online, and follows cloud case studies at the level of tutorials. These enable
subsequent research teams to accelerate the pace at which they can build cloud-based research computing
tools, workflows, websites, data repositories and other data-arc solutions. 



## Links


- [eScience Institute](http://escience.washington.edu)
- [genome sciences at UW](http://www.gs.washington.edu)
- [medical science at UW](http://www.uwmedicine.org)


## Admonitions	


- ***Contact us regarding updates to this material***
- ***Focus here is topics; we try to preserve a degree of anonymity***


## Yun Zhao Guan: A cloud library -- digital curation -- in cooperation with Suzallo Library


- LIDARY: A pilot study providing geospatial LIDAR data as an open, curated digital resource
  - [A simple map](http://map.cloudmaven.org) 
  - [A GeoServer implementation](http://lidargeoserver.cloudmaven.org) 
- Proof-of-concept curation of an epigenome imputation engine (see Student Research) 
- Migration to the cloud of [BrainInfo.org](http://braininfo.org/) including [NeuroNames](https://en.wikipedia.org/wiki/NeuroNames)


## General Systems and Tools


- [SQL Share](https://sqlshare.uw.edu): A system for managing, sharing and manipulating research data.
- [Myria](http://myria.cs.washington.edu/): A distributed, shared-nothing Big Data management system and Cloud service from the University of Washington
- IOT based on Arduino Yun leaf technology and cloud IOT endpoint services
- Geohackweek and Neurohackweek: Hosting intensive workshops for learning and developing cloud-based tools and methods at UW


## Student-driven research


The UW Student High Performance Computing Club has begun making cloud computing available to its members. This includes 
training and consulting on implementation as well as careful cost management and tracking. The following is a partial list
of projects undertaken by students during the pilot phase of this program, spring 2017.


- Epigenome imputation across a nucleotide-protein-cell tensor (Status: Successful completion)
- Design of a high-reliability micropump for cooling high-heat semiconductors (In progress)
- Novel peptide characterization of marine organic matter: insights into carbon cycling (In progress)
- Characterizing the progression of three pathologies in ER electronic medical records (In progress)
- Quora question pair intent comparison (In progress)
- Novel peptide characterization of marine organic matter: insights into carbon cycling (In progress)
- Schedular development and benchmarking for containerized bioinformatics workflows (UW Tacoma; in progress)
- Empirical Studies of Docker Orchestration Tools for The Analyses of Big Biomedical Data (UW Tacoma; in progress)
- Predictive models to optimize cloud computing using genomics data (UW Tacoma; in progress)
- A Dynamic Scaling Engine in the Cloud (CSE; in progress)
- LaraDB Experiments for the DARPA Graph Challenge (CSE; in progress)
- Learning multiple outcomes with predictive coding (CSE; in progress)


## Medical 


- Laboratory Medicine: Genome analysis and annotation (clinical oncology & co)
- Clinical data availability for research 
- Data access and tool access for MRI- and EEG-based research
- Gut biome metagenomics (Children's Hospital)
- Patterns in unexpected in-hospital mortality
- Studies on Post-hospital-admission sepsis (blood infection)
- Deep learning for patient behavior prediction: EEG data in relation to A/V transcripts of patient behavior
  - See above under *Student research*
- Canine longitudinal aging studies
- Biostatistics
- Light-sheet microscopy for fast-turnaround biopsy analysis 
- Neuroimaging: Functional MRI
- Neuroimaging: Visual cortex studies


## Genomics and Biochemistry (not included in *Medical* above)


- Epigenome imputation: See above under *Student Research* 
- Genetic architecture of autism
- Metagenomics of methane-consuming microbial communities
- Enzyme inhibition molecular structure
- Peptide scaffolding enumeration and design: Large-scale computing using the Rosetta protein folding toolkit





## Hydrology and Geochemistry


- GDS: Geometabolomics Data System, a community library and reproducible workflow environment for molecular spectral 
analysis applied to naturally occurring Dissolved Organic Matter (DOM).
- HiMAT (NASA): Atmosphere-land coupled analysis of the hydrological state and future of high mountain Asia
  - Hydrological studies and human impacts drawing from *in situ*, remote sensing, model, re-analysis and assimilation data and methods.
- Dynamic Infomation Framework (DIF) (World Bank): Scientific hydrological expertise transferred into public information
   - In resource management and public safety domains the incorporation of scientific modeling is not well developed.
   - This program provides localized information building from a reproducible model of free and open access



## Ocean science


- LiveOcean: Ocean modeling forecast
- Marine microbial ecology
- Mesoscale eddie structure and correlation to marine life

## Computer Science


- Analysis of code fault detection: Student project
- IOT: A design pattern and tutorial for using cloud-based support of **Internet of Things** implementations 
(NSF: Campus Cyberinfrastructure)
- Data security on the cloud: A generic data system with automated and human protocols for working on sensitive
data including elements of compliance with oversight regulations 
(NSF: Campus Cyberinfrastructure)
- Scale on the cloud: See under Molecular Engineering and Science the protein folding case study
(NSF: Campus Cyberinfrastructure)
- Collaboration on the cloud: See case studies herein on GeoServer/THREDDS, on LIDAR, on Dynamic Information 
Frameworks and on HiMAT; thematically lightweight geospatial data system with the underlying theme of 'access 
to data through pre-built frameworks, data APIs and minimal (non-redundant) software engineering.
(NSF: Campus Cyberinfrastructure)


## Mechanical and Civil Engineering


- Computational fluid dynamics of hydrogen and methane combustion


## Astronomy


- Identifying stellar composition through spectral model superposition in nearby galaxies
- Large Scale Synoptic Telescope (LSST) toolchain development


## Geospatial 


- Implementation of GeoServer and a THREDDS server on the public cloud
- Various data archival projects: Using the cloud for many 9s of reliability


## Stubs and pending


- IOT
- Power consumption



{% include links.html %}
