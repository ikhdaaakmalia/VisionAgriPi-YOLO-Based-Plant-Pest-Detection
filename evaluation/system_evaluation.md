# System Evaluation

## Laboratory Testing

| Test | Distance | Raspberry Pi 4 | Raspberry Pi 5 |
|------|----------|----------------|----------------|
| 1    | 30 cm    | Detected       | Detected       |
| 2    | 45 cm    | Detected       | Detected       |
| 3    | 60 cm    | Random objects | Detected       |

## Field Testing (Bright Outdoor Conditions)

| Test | Distance | Raspberry Pi 4 | Raspberry Pi 5 |
|------|----------|----------------|----------------|
| 1    | 30 cm    | Not detected   | Detected       |
| 2    | 45 cm    | Not detected   | Not detected   |
| 3    | 60 cm    | Not detected   | Not detected   |

## Discussion
Laboratory testing showed stable detection performance for both devices at short and medium distances. However, Raspberry Pi 4 struggled to maintain detection accuracy at longer distances, while Raspberry Pi 5 demonstrated superior processing capability.

Under field conditions, detection performance degraded significantly, particularly on Raspberry Pi 4. Raspberry Pi 5 maintained limited detection at close range, indicating better robustness under real-world environmental variability.
