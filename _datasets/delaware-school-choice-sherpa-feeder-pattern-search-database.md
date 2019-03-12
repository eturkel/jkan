---
schema: default
title: 'Delaware School Choice Sherpa: Feeder Pattern Search database'
organization: 'Open Data Delaware, Newark Codes'
notes: "Tables: districts, feeder_patterns, raw_feeder_patterns_by_grades, schools\r\n\r\nRequirements: PostgreSQL >=10.5, PostGIS\r\n\r\nInstall: psql sherpa_development < sherpa.dump\r\n\r\n`districts` contains the merged information from the datasets on district information and geometry of the districts\r\n`feeder_patterns` contains the grade levels and geometries of the mapped regions that feed into each school\r\n`raw_feeder_patterns_by_grades` this is an intermediate table containing unmerged geometries for each school\r\n`schools` contains the discrete information about each school"
resources:
  - name: Post-Transformation PostgreSQL 10.5 data dump
    url: 'https://s3-us-west-2.amazonaws.com/privateerconsulting/sherpa.dump'
    format: api
license: 'http://www.opendefinition.org/licenses/odc-pddl'
category:
  - Education
maintainer: >-
  Source Data: Delaware Department of Education; Transformation Dump: Eric L.
  Truitte
maintainer_email: etruitte@privateerconsulting.com
---