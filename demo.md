## Table 5.1: Dataset Growth and Training Visibility

| Metric                  | Value        |
|------------------------|-------------|
| Total Apps Analyzed    | 1234        |
| Total Labeled          | 1234        |
| Pending Label          | 0           |
| Ready for Training     | 4           |
| Last Trained Count     | 6           |
| Model Version          | model_v27.pkl |
| APK Count              | 937         |
| XAPK Count             | 223         |
| APKM Count             | 71          |
| APKS Count             | 1           |
| Partial XAPK Count     | 2           |


## Table 5.2: Recent Analysis History

| App ID (Short) | Type | Static | Install | Interaction | Risk Level | Prediction  | Confidence | Source        | Timestamp |
|----------------|------|--------|--------|------------|------------|------------|-----------|--------------|----------|
| f57b...1bc4    | APK  | SUCCESS | SUCCESS | BLOCKED    | LOW        | benign     | 39%       | Fallback Rule | 19:16    |
| 663f...99c2    | APK  | SUCCESS | SUCCESS | COMPLETED  | MEDIUM     | benign     | 77%       | Manual       | 17:48    |
| 663f...99c2    | APK  | SUCCESS | SUCCESS | COMPLETED  | LOW        | suspicious | 94%       | Rule-based   | 17:47    |
| 663f...99c2    | APK  | SUCCESS | SUCCESS | COMPLETED  | LOW        | suspicious | 75%       | Rule-based   | 17:46    |
| sample_05      | APK  | SUCCESS | SUCCESS | COMPLETED  | LOW        | benign     | 60%       | ML Weak      | 18:00    |
| sample_06      | APK  | SUCCESS | SUCCESS | COMPLETED  | LOW        | benign     | 56%       | ML Weak      | 18:01    |


## Table 7.1: Screenshot Summary

| View                     | Purpose                         | Key Elements Shown                     |
|--------------------------|--------------------------------|--------------------------------------|
| Upload Dashboard         | Entry point                    | File upload, device status           |
| Dataset Growth Counters  | Dataset visibility             | Counts, model version                |
| Training Panel           | Model training control         | Train button, sample count           |
| Recent Analyses          | Session history                | Status, risk, prediction             |
| Risk Result Page         | Final analysis output          | Risk score, explanation              |


## Table 7.2: Case Study Comparison

| Case Type        | Runtime Status | Risk Level | Prediction  | Key Observation                          |
|------------------|--------------|-----------|------------|------------------------------------------|
| Low Risk         | Complete     | Low       | Benign     | Minimal permissions, clean behavior      |
| Medium Risk      | Complete     | Medium    | Suspicious | Some sensitive signals present           |
| High Risk        | Complete     | High      | Suspicious | Strong indicators of risky behavior      |
| Partial Analysis | Incomplete   | Limited   | Weak       | Runtime evidence missing                 |
| XAPK Case        | Partial      | Medium    | Mixed      | Packaging limitation affected analysis   |

## Table 3.1: MTP-1 vs MTP-2 Comparison

| Aspect              | MTP-1                  | MTP-2                          |
|--------------------|------------------------|--------------------------------|
| Dataset Size       | ~100 apps              | 1234 apps                      |
| Input Support      | APK only               | APK, XAPK, APKM, APKS          |
| Static Analysis    | Basic                  | Improved                       |
| Dynamic Analysis   | Limited                | ADB-based real device          |
| UI                 | Minimal                | Full dashboard                 |
| Training Visibility| Not available          | Available                      |
| Model Tracking     | Not available          | model_v27.pkl                  |
| Risk Explanation   | Basic                  | Explainable                    |
| Partial Handling   | Not handled            | Explicit                       |
| System Maturity    | Prototype              | Handoff-ready system           |

