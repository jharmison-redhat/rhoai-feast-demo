# Real-time Credit Scoring with Feast on OpenShift AI

## Overview

This tutorial is built from the original **[feast-credit-scoring-tutorial](https://github.com/feast-dev/feast-credit-score-local-tutorial/tree/598a270353d8a83b37535f849a0fa000a07be8b5)**.

This tutorial demonstrates the use of Feast as part of a real-time credit scoring application inside OpenShift AI.

- The primary training dataset is a loan table. This table contains historic loan data with accompanying features. The dataset also contains a target variable, namely whether a user has defaulted on their loan.
- Feast is used during training to enrich the loan table with zipcode and credit history features from the **data** folder.
- Feast is also used to serve the latest zipcode and credit history features for online credit scoring using Redis.

## Requirements

- Python 3.12
- Registry: PostgreSQL
- Offline Storage: duckdb
- Online Storage: PostgreSQL
