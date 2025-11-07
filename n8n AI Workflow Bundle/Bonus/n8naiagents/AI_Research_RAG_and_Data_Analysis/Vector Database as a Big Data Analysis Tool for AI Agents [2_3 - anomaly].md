# Workflow Analysis for [2/3] Set up medoids (2 types) for anomaly detection (crops dataset)

## Description
This workflow is the second part of a three-part pipeline designed to set up anomaly detection for agricultural crop images. It focuses on identifying two types of cluster centers (medoids) and calculating their respective anomaly thresholds within a Qdrant vector database collection.

## Input Details
The workflow is manually triggered and utilizes predefined Qdrant connection variables, parameters for medoid threshold determination, and hardcoded textual descriptions of various crops.

## Process Summary
The workflow first initializes Qdrant connection details and anomaly detection parameters. It then retrieves total point counts and unique crop names from the Qdrant collection. For the "distance matrix" approach, it calculates a distance matrix for points within each crop cluster, identifies the most representative point (medoid) using SciPy, and updates its payload in Qdrant. Simultaneously, for the "text anchor" approach, it embeds predefined textual crop descriptions using Voyage AI and finds the closest image point in Qdrant to each description, marking it as a text anchor medoid. Finally, for both types of medoids, the workflow calculates an anomaly detection threshold by identifying the point furthest from the medoid within its cluster and stores this score in the medoid's payload in Qdrant.

## Output Details
The workflow updates existing points in the Qdrant collection by adding specific payloads: `is_medoid`, `is_text_anchor_medoid` to identify the designated medoids, and `is_medoid_cluster_threshold`, `is_text_anchor_medoid_cluster_threshold` to store their calculated anomaly thresholds.
