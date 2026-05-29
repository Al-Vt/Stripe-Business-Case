# Stripe Data Architecture Case Study

## Overview

This project designs a comprehensive data architecture for Stripe,
integrating OLTP, OLAP, and NoSQL systems to support transactional
integrity, advanced analytics, and flexible data management.

## Data Architecture

### OLTP — PostgreSQL

* Normalized schema with 13 tables
* Supports ACID properties
* Handles transactions, refunds, chargebacks and subscriptions

### OLAP — Snowflake

* Star schema with 3 fact tables and 5 dimensions
* 3 materialized views for performance optimization
* Supports revenue analysis, fraud detection and customer segmentation

### NoSQL — MongoDB

* 4 collections for unstructured data
* Handles logs, user interactions, ML features and customer feedback
* Embedding and referencing strategies

## Technologies

| Tool | Role |
|----|----|
| PostgreSQL | OLTP database |
| MongoDB | NoSQL database |
| Snowflake | OLAP data warehouse |
| Apache Kafka | Real-time streaming |
| Apache Airflow | Pipeline orchestration |
| Airbyte | Data extraction and loading |
| dbt | Data transformation |

## Regulatory Compliance

* GDPR — European customer data protection
* PCI-DSS Level 1 — Payment card security standard

## Machine Learning

Three ML models integrated within the NoSQL system:

* Real-time fraud detection
* Customer personalization
* Predictive analytics


