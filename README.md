# Real-Time KPI Monitoring System for Quick-Commerce

##  Business Context
Quick-commerce platforms (e.g., DoorDash, Instacart, Blinkit, Uber Eats) require real-time
visibility into order flow, revenue, and payment reliability.
Delays in detecting issues can directly impact customer experience and revenue.

## Project Objective
To build a real-time KPI monitoring system that simulates live order data,
processes it continuously, and displays business-critical metrics for
operational decision-making.

## Key KPIs Tracked
- Orders per Minute
- Total Revenue
- Average Order Value (AOV)
- Payment Success Rate
- Failed Transactions per Minute
- Active Users (Last 5 Minutes)

## System Architecture
Order Data Generator (Python)
↓
Real-Time KPI Processor (Python)
↓
SQLite Database
↓
Power BI Dashboard

## Real-Time Order Data Schema

order_id           : string
timestamp          : datetime
user_id            : string
store_id           : string
order_value        : float
payment_status     : success / failed
delivery_time_min  : int
city               : string
