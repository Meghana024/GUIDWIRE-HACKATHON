# RainGuard AI — Predictive Adaptive Income Protection for Kerala Delivery Riders

---

## Problem Statement

- Delivery riders lose 25–40% of their income during monsoon.
- Loss is caused by weather disruptions.
- Two main situations:
  - Rider is online but receives zero orders.
  - Rider cannot deliver due to flooded or unsafe roads.
- Riders are willing to work but unable to earn.
- There is no existing system that protects this income loss.

---

## Persona Example

- Rahul (Delivery Rider – Kochi)
- Works: 10 AM – 8 PM
- Normal earning: ₹600/day

During rain:
- Earns only ₹200
- Loss = ₹400
- No compensation available

---

## Solution Overview

- Web-based system for income protection.
- Uses weather data and AI prediction.
- Detects real work disruption.
- Calculates actual income loss.
- Provides adaptive compensation.
- Ensures fraud-resistant payouts.

---

## Core Concepts

### Work Disruption Modeling

- Focuses on real earning impact.
- Two disruption cases:
  - Zero orders due to low demand.
  - Cannot deliver due to unsafe conditions.
- Both cases are treated as valid income loss.

---

### Partial Income Protection

- Covers reduced income, not just zero income.
- Uses the formula:
Loss = Expected Income – Actual Income

- Ensures fair and realistic compensation.

---

### Adaptive Income Protection

- Payout is dynamic, not fixed.
- Depends on:
  - Rain severity
  - Duration of disruption
  - Income loss
- Higher loss leads to higher payout.

---

### Fraud Detection Layer

- Ensures only genuine claims are approved.
- Includes:
  - Location validation
  - Weather validation
  - Network-level validation
  - Rider reliability score
- Uses a multi-signal decision system.

---

### Rider Risk Score

- Indicates weekly risk level:
  - Low
  - Medium
  - High
- Helps riders understand expected disruption.

---

## System Workflow
## System Workflow

### High-Level Flow

Onboarding → Data Collection → Prediction → Weekly Plan → Monitoring → Disruption → Loss Calculation → Validation → Payout → Dashboard

---

### Step-by-Step Flow

1. Rider enters location, working hours, and average income.

2. System collects weather data and historical patterns.

3. AI predicts risk level and expected disruption hours.

4. Weekly premium is calculated and plan is generated.

5. Rider activates the policy for the week.

6. System sends alerts for predicted high-risk periods.

7. System monitors weather conditions and rider activity.

8. Disruption is detected:
   - Zero orders  
   - Cannot deliver  

9. System calculates expected vs actual income.

10. Income loss is computed and adaptive compensation is applied.

11. Fraud validation is performed using multiple signals.

12. Decision engine approves or flags the claim.

13. Payout is processed.

14. Dashboard is updated with results and analytics.

---

## Weekly Premium Model

- Base premium: ₹89
- Dynamic component: ₹40–₹85
- Based on predicted risk
- Fixed for 7 days
- Includes a 48-hour lock-in period

---

## Parametric Triggers

- Rainfall greater than or equal to 15 mm in 3 hours
- More than 60% drop in orders
- Flood risk conditions

---

## AI/ML Integration

- Risk prediction using XGBoost
- Forecasting using time-based models
- Income estimation using regression
- Fraud detection using rule-based scoring

---

## Platform Choice

Web Application

Reasons:
- Faster development
- Easy to demonstrate
- No device dependency
- Suitable for hackathon prototype

---

## Tech Stack

- Frontend: Streamlit or React
- Backend: FastAPI
- Database: Supabase
- Weather API: Open-Meteo
- Machine Learning: XGBoost, scikit-learn
- Payments: Razorpay (test mode)

---

## Development Plan

### Phase 1 (Completed)
- Problem understanding
- Persona analysis
- System design
- Workflow definition
- ML planning

### Phase 2
- Web app development
- Weather API integration
- Prediction implementation

### Phase 3
- Fraud system improvement
- Dashboard development
- Optimization

---

## Why RainGuard AI

- Addresses a real-world problem
- Uses AI for prediction
- Provides adaptive compensation
- Covers partial income loss
- Includes fraud detection
- Supports automated payouts

---

## Final Summary
RainGuard AI is a predictive, web-based income protection system designed to support delivery riders during weather disruptions. It uses weather data and machine learning models to forecast high-risk periods, detects real work impact such as zero orders or unsafe delivery conditions, and calculates actual income loss by comparing expected and earned income. Based on this, the system provides adaptive compensation that adjusts according to the severity and duration of disruption. A multi-layer fraud detection mechanism ensures that only genuine claims are approved, and payouts are processed automatically. Overall, RainGuard AI offers a fair, intelligent, and practical solution to protect riders’ earnings during adverse weather conditions.
