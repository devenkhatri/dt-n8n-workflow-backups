# Workflow Analysis for CalcsLive Demo Workflow Template

## Description
This workflow demonstrates how to use the CalcsLive custom node in n8n to perform unit-aware physical calculations—such as calculating the area and volume of a cylinder, and then using that volume to compute mass from a given density. It also includes a speed calculation example and sends the final results via email.

## Input Details
The workflow is triggered manually and receives hardcoded physical quantities (like diameter, height, distance, time, and density) as inputs within the workflow nodes.

## Process Summary
First, the workflow is manually triggered. It then uses the CalcsLive node to calculate the area (A) and volume (V) of a cylinder from diameter (D) and height (h). Separately, it calculates speed (v) from distance (d) and time (t). Next, it computes mass (m) using the previously calculated volume (V) and a given density (ρ). Finally, it sends an email with the mass result and other calculation details.

## Output Details
The workflow sends an email via Gmail containing the results of the physical calculations, including the computed mass and metadata about the calculations.

## Tags
CalcsLive, physical calculations, unit-aware, n8n, automation, email notification, cylinder volume, mass calculation, speed calculation, production-ready
