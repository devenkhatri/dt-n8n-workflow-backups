# Workflow Analysis for Raw Materials Inventory Management with Google Sheets and Supabase

## Description
This workflow automates raw materials inventory management by handling incoming material receipts, processing material issue requests with approval workflows, updating stock levels in real-time, and sending email alerts when stock falls below minimum levels.

## Input Details
The workflow is triggered by two webhook endpoints: one for receiving raw material delivery data via POST requests and another for handling material issue requests, plus a third webhook for approval responses.

## Process Summary
When raw materials are received, the workflow validates the data, calculates total cost, and updates current stock levels in Google Sheets and Supabase—either by creating a new product entry or updating existing stock. For material issue requests, it records the request, checks stock availability, and sends an approval email with approve/reject links. Upon approval, it deducts the issued quantity from stock and updates records. After any stock change, it checks if levels fall below the minimum threshold and sends low-stock email alerts if needed.

## Output Details
The workflow updates Google Sheets and Supabase databases with receipt records, issue requests, and current stock levels, and sends Gmail notifications for approval requests and low stock alerts.

## Tags
inventory management, raw materials, stock tracking, approval workflow, Google Sheets, Supabase, Gmail, webhook, automated alerts, material issuance
