---
title: Welcome
---

# Kitsuna Data


## About The Project

This is a concept for what a Rails-inspired small data platform for startups and SMEs could look like. After using a variety of end-to-end solutions like DOMO, Keboola, Mozart Data and others, I keep wishing there was something that would do the 80% of ELT + BI out-of-the-box, without the price surprises.

This project is an attempt to stitch together a set of solid and reliable open-source tools that combine into a lean platform where one data engineer can own the entire lifecycle. From ELT, to data modelling, to deploying and scaling in production.

!!! warning

    The project is very much in the pre-alpha stage. This is more of an experiment and is not meant for produciton workloads.

### Goals

- Local-first development for the entire stack.
- Support companies that can't afford heavy, expensive data tools or large teams.
- No "SSO tax" - all tools should be either fully free, or affordable once deployed in serious prod use case.
- No k8s, so a small data team can be self-sufficient .
- Cheap path to production and scaling.

### Tech Stack

- _Extract_ (planned): [dlt](https://dlthub.com/)
- Transform: [SQLMesh](https://sqlmesh.readthedocs.io/en/stable/)
- Data Storage: [DuckDB](https://duckdb.org/)
- BI / data viz: [Metabase](https://www.metabase.com/)
- Deployment: [Dokku](https://dokku.com/docs/getting-started/install/digitalocean.)

<p align="right">(<a href="#readme-top">back to top</a>)</p>
