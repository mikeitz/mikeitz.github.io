---
layout: page
title: Resume
displaytitle: Michael C. Itz
permalink: /resume/
---
# OVERVIEW

- Technical leader and software engineering generalist with 20 years of tech industry experience  
- Experienced in founding and growing capable engineering teams through investment in people, expertise, infrastructure, and organizational relationships  
- Background in search, machine learning, data analysis, and distributed systems  
- Skilled in maintaining, extending, and debugging complex systems and large multi-language codebases  
- Values implementation simplicity, transparency, repeatability, and iterative data-driven processes

# EXPERIENCE

## **Google**

Cambridge, MA  
*Staff Software Engineer, 2019-2024*  
*Senior Software Engineer, 2015-2018*

### **Search Platforms Data Protection**

*Tech Lead for Privacy, 2023-2024*

- Designed engineering plan and lead technical execution to mitigate specific high priority risks in Incognito Search design  
  - Steered work for 15 engineers across six teams in coordinated changes to client, server, platform, storage, logging, and analytics (C++, Java, Python, SQL/mapreduce)  
  - Reworked core methodologies for log retention/processing, product health tooling, and metric/experiment evaluation in impacted traffic segments  
- Developed novel analysis technique to segment user data collection by product/feature across all transitive systems in the Google-wide production footprint by correlation of latency/reliability data with product quality logs (Python, gRPC, C++, Java, SQL/mapreduce)  
  - Covered \~million storage events per second across \~thousands of server binaries to identify sensitive data retention under various policies, across code/services operated by all product areas (Search, Ads, YouTube, Workspace, etc)  
- Designed technical architecture and migration plans to centralize/standardize application of policies for acceptable data use during model training and inference for generating interest based personal recommendations, addressing PR risks from policy misapplication  
  - Support live policy application in serving stack for Search, Discover, Google App, "What to Watch", and other personalized surfaces (C++, Java)  
  - Support per-event policy application within model training runs up to 1 year of click-level activity history for all active Search users  
  - Manage \~10k human annotations in categorizing \~millions of knowledge graph entities  
  - Obtained 5 permanent SWE staffing for build-out and ongoing governance

### **Search/Assistant Privacy Engineering**

*Tech Lead/Manager, 2020-2023*

- Owned user-facing technical privacy commitments for all personal data collection/use in Google Assistant, and managed team of 15 SWE in selection/scoping of projects to strengthen Google's privacy stance and user trust  
- Grew engineering team to respond to large regulatory and litigation-prompted technical challenges crossing product/organizational boundaries  
  - Including: UK Age Appropriate Design Code, EU Digital Markets Act, Apple Privacy Nutrition Label / App Tracking Transparency, "Misactivation" voice data handling  
  - Hired 12 engineers to the team, mentored 9 members to committee-approved promotion (2 SWE \[L4\], 6 Senior SWE \[L5\], 1 Staff SWE \[L6\]), and grew 4 as new team Tech Leads  
  - Conducted technical briefings for cross-org high priority regulatory workstreams for \~50 SWE/PM/PgM/Analysts across \~10 cost centers  
- Invested in adding collection/use monitoring and policy enforcement into the Google-wide tech stack at the core infrastructure level  
  - Lead Search partnership with Youtube to launch first use of the technology to coordinate cross-Product policy application, proving/standardizing the approach across Google (C++, Java, Android, Cast)  
  - Organized migration of all legacy Assistant collection policies forward to new framework  
- Sponsored work to understand drivers of user trust and launch user-facing trust positive features (Assistant's abilities to describe its privacy policies and features, instant Assistant-triggered history deletion, Assistant Guest Mode, and various cross-surface messaging experiments)  
- Partnered with legal counsel team to facilitate technical discussions between Assistant engineering and counsel  
- Delivered regular Search VP-level updates on cross-org workstreams

### **Google Assistant for Hospitality**

*Tech Lead/Manager, 2018-2022*

- Executed high-profile pilot of Assistant in public spaces (Disneyworld, JFK Terminal 4, Best Buy, Merrill Gardens, selected hotels), deploying 10k devices for 3 years  
- Built team of 4 engineers on Assistant software, in partnership with Nest hardware team  
- Designed legally critical partitioned data rights infrastructure to separate owner vs users of device; passed legal review in US/UK/EU/JP, including HIPAA audit for hospital room use (C++)  
- Shipped APIs for 3p vendors (Volara, SONIFI) to handle device deployment lifecycle and per-site customizations (ex., hotel amenities) (Javascript, Dart/Flutter)  
- Clean turndown at end of program, with zero privacy/security/press incidents reported over the lifetime of the program, despite risk of operation in public spaces

### **Google Assistant Help**

*Tech Lead/Manager, 2017-2023*

- Founded four-member team and built cross-discipline organization (UX design, UXR, content analysts, tech writers, linguists) to study and address areas in organic usage where users were not getting desired outcomes from the Assistant or its host device. Focused on segments missed by vertical feature teams' quality strategies  
- Built scalable vendor-staffable systems to identify gaps in live traffic and respond by routing to feature teams or by rapid launch of lightweight vendor-authored help content (C++, Java)  
- Defended the value of the segment to leadership to secure headcount, vendor support, and priority with other vertical feature teams through continuous measurement of interventions' impact against key metrics, including overall and per-feature daily active user counts  
- Initiated and led 4-month Assistant stack-wide sprint to fix critical cross-layer quality issues (Android client, client/server protocol spec, voice server, Assistant server, state management systems)

### **Google Assistant Query Classifiers**

*Software Engineer, 2015-2017*

- Owned quality of prediction of two key factors in Assistant response planning: information seeking intent and topic sensitivity  
- Key component to unblock first wave of Google Assistant launch surfaces (Allo, Google Home, Pixel 2\)  
- Designed and implemented framework for rapid prototyping of model structure and feature set via parallel to production deployment infrastructure (Python, C++, SWIG)  
- Selected and validated metrics for quantifying model changes, and developed tools for analysts to validate future model changes with strong focus on confidence intervals, still used 8 years later (Python)  
- Implemented test/train data collection and management methodology (Python)  
- Implemented fast incident response strategy for \<1hr updates in case of prominent model losses (C++, Python)

## **Nokia**

Cambridge, MA  
*Principal Software Engineer, 2012-2015*  
*Senior Software Engineer, 2010-2012*

### **HERE Map Search**

- Managed team of ten in research, development, and maintenance of map search backend used daily by two million unique users in forty languages and sixty countries   
- Architected rebuild of search ranking and indexing system in place to adopt flexible machine learned ranking in place of handcrafted rules, including:  
  - New metrics to track overall and specialized search concerns and used for experimental evaluation (R, Python)  
  - New data management strategy to apply train/test annotations on highly unstable underlying result data set (Python)  
  - Model-based ranking layer above existing heterogenous index/retrieval layers to decouple final ranking from index details and ensure response precision (Java, Python)  
  - New response rendering services to decouple rendering from indexing (Java)  
  - Per-source index rebuild to maximize recall, incorporating new retrieval strategies based on losses identified at model layer (Java)  
- Designed and led total rebuild of geographic data ingestion pipeline (intake, deduplication, indexing of multiple terabytes)  for statelessness, reproducibility, transparency, and use of elastic resources, including:  
  - New lightweight task sequencing tool to handle processing steps built with mismatched languages with minimum boilerplate and dependency-aware partial reruns to improve developer experience (Python, Java, C++, R)  
  - Redesign to run on per-job elastic resources instead of fixed prod/dev environments  
  - Parallel deduplication process to support stateless pairwise re-matching of full corpus on underlying changes to data, code, or models (instead of once-only stateful deduplication)  
  - Migrated backing store from key-value to indexed relational db for intermediate results and final outputs to allow easy ad hoc inspection, debugging, and measurement (Postgres)

## **Metacarta**

Cambridge, MA  
*Technical Lead, 2008-2010*  
*Software Engineer, 2006-2008*

### **Geographic Search/Referencing Platform**

- Contributed to development of Geographic Text Search appliance, using natural language processing to provide geography-aware document indexing and retrieval on third party document stores for GIS use (C++)  
- Curated geographic data store containing tens of millions of rows of place data and billions of rows of linguistic data used for constructing hybrid geographic/language models (Postgres)  
- Added support for extraction and indexing of partial/ambiguous street-level mentions, including evaluation and integration of third party geocoder components (C++)  
- Extended English-only product infrastructure to support indexing, searching, and rendering of French, Spanish, Russian, and Arabic documents (C++)  
- Added cross-compilation support to build chain (x86 Debian to amd64 Debian, RHEL, CentOS, and Windows targets)

## **eFitnessTools**

Grafton, MA  
*Developer Intern, 2005*

- Designed/implemented handwriting recognition module for in-gym scanner kiosks (C\#)

## **deNovis**

Lexington, MA  
*QA Engineer Intern, 2003-2004*

- Designed/implemented synthetic medical record and insurance billing generation for QA use

# EDUCATION

## **Worcester Polytechnic Institute**

Worcester, MA  
*Bachelor of Science, Computer Science, with High Distinction, 2002-2005*

### Natural Language Interface via First Order Logic (*Major Qualifying Project, 2005\)*

- Developed tools to translate Lojban language text to/from first-order logic

### Biodiversity Database Management (*Interdisciplinary Qualifying Project, 2004\)*

- Analyzed collection, storage, and availability of vegetation plot data onsite at Smithsonian Institution