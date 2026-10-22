# SafeBank AI 🛡️

### Don't just detect fraud. Stop it before the money is gone.

SafeBank AI is an adaptive banking safety prototype designed to identify suspicious transaction behaviour and help users make safer digital banking decisions before potential fraud results in financial loss.

It evaluates multiple risk signals and provides explainable risk-based decisions: **ALLOW, WARN, or PAUSE**.

## 🚀 Key Features

### 1. Adaptive Transaction Risk Engine
- Calculates a risk score from 0–100.
- Evaluates transaction amount, beneficiary, device, location, time, and transaction patterns.
- Classifies transactions into LOW, MEDIUM, and HIGH risk levels.

### 2. Explainable Risk Decisions
- **LOW → ALLOW:** Transaction can proceed.
- **MEDIUM → WARN:** Displays a warning and allows user confirmation.
- **HIGH → PAUSE:** Pauses the flow for additional verification.

### 3. Scam Scanner
Analyzes suspicious messages using pattern-based detection and provides a risk score, explanation, and recommendation.

### 4. Trusted Contact Verification
Supports an additional verification step for high-risk situations. Trusted contacts do not receive banking credentials or control the user's funds.

### 5. Transaction History
Displays stored transactions and their associated risk decisions.

### 6. Safety Alerts
Stores and displays alerts associated with suspicious or high-risk transactions.

### 7. Fraud Monitoring Dashboard
Displays transaction and risk information, including risk scores, risk levels, decisions, and monitoring filters.

### 8. Safety Center
Allows users to manage protection settings and trusted contacts.

## 🔄 Application Workflow

```text
Send Money
    ↓
Save Transaction
    ↓
Risk Assessment
    ↓
Risk Score + Explanation
    ↓
LOW / MEDIUM / HIGH
    ↓
ALLOW / WARN / PAUSE
    ↓
Confirmation or Additional Verification
    ↓
Transaction History + Safety Monitoring
```

## 🧠 Risk Engine

The MVP uses a weighted JavaScript-based scoring model.

| Risk Signal | Weight |
|---|---:|
| Transaction Amount | 25 |
| New Beneficiary | 20 |
| Device | 15
