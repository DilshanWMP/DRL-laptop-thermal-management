### DRL Laptop Thermal Management
### EC6301 Artificial Intelligence | University of Ruhuna

## Project Title
Adaptive Deep Reinforcement Learning for Intelligent Thermal Management and Performance Optimization in Laptops

## Team Members
- Dilshan W.M.P (EG/2022/5016)
- Dissanayake D.M.K.M. (EG/2022/5016)
- Gunarathne G.D.H. (EG/2022/5047)
- Ranasinghe U.G.P.B. (EG/2022/5276)

## Project Overview
This project develops a Deep Reinforcement Learning (DRL) agent to intelligently manage laptop thermal conditions. Instead of traditional static rule-based controllers, our PPO agent learns to optimally balance temperature, performance, and energy efficiency.

## Key Results
| Metric | Value |
|---|---|
| World Model R² | 0.9925 |
| PPO Mean Reward | 1310.40 |
| Average Temperature | 66.1°C (optimal zone) |
| Time in Optimal Zone | 97.4% |
| Overheating Steps | 0 |

## Benchmark Comparison
| Controller | Avg Reward | Zone % |
|---|---|---|
| PPO Agent (Ours) | 1303.90 | 97.4% |
| Static Rules | 841.35 | 72.0% |
| PID Controller | 348.85 | 48.0% |

## Tech Stack
- Python, PyTorch, OpenAI Gymnasium
- Stable-Baselines3 (PPO)
- Streamlit Dashboard
- Google Colab + Google Drive

## Project Phases
1. Data Loading & Exploration
2. Data Preprocessing
3. ANN World Model Training (R²=0.99)
4. Custom Gym Environment
5. PPO DRL Agent Training
6. Benchmarking vs Baselines
7. Streamlit Dashboard

## Dataset
Kaggle: Laptop Motherboard Health Monitoring Dataset (2000 rows, 8 features)
"""

with open('/content/DRL-laptop-thermal-management/README.md', 'w') as f:
    f.write(readme)

!git add README.md
!git commit -m "docs: update README with project details and results"
!git push origin main

print("✅ README updated!")
