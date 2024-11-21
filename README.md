# Improving Fault Tolerance in Kubernetes with Signal-Based Monitoring

Welcome to the research project repository on enhancing fault tolerance and resource efficiency in Kubernetes-managed microservices. This work introduces signal-based monitoring and Erlang-inspired supervision trees to address cascading failures and improve system resilience.

---

## 🔍 **Table of Contents**
- [Introduction](#introduction)
- [Why Fault Tolerance Matters](#why-fault-tolerance-matters)
- [Research Goals](#research-goals)
- [Proposed Solution](#proposed-solution)
- [Expected Outcomes and Insights](#expected-outcomes-and-insights)
- [Contact](#contact)

---

## 📖 **Introduction**
Ensuring high availability and fault tolerance in Kubernetes-managed microservices is a critical challenge. Current polling-based monitoring mechanisms are reactive, slow, and resource-intensive. This research pioneers the use of signal-based monitoring and hierarchical fault management, leveraging Erlang-inspired supervision trees to proactively detect and recover from failures in real time.

---

## 💡 **Why Fault Tolerance Matters**
Microservices underpin critical applications in **e-commerce**, **finance**, and **healthcare**, where downtime can lead to severe consequences:
- **E-commerce Example:** Downtime during a flash sale can result in revenue loss and customer dissatisfaction.
- **Healthcare Example:** Failures in critical systems can jeopardize patient safety.

### Limitations of Current Approaches:
- **Polling Mechanisms:** Reactive fault detection with delays proportional to polling intervals.
- **Resource Overhead:** Frequent polling increases CPU and network usage, making it inefficient for large-scale systems.

### Signal-Based Monitoring Advantages:
- **Proactive Detection:** Pods send real-time health signals to supervisors.
- **Reduced Latency:** Faster failure detection compared to polling-based methods.
- **Efficient Scaling:** Lower CPU and RAM overhead, suitable for interdependent environments.

---

## 🎯 **Research Goals**
This project redefines fault tolerance in Kubernetes-managed microservices by integrating signal-based monitoring and supervision trees. The goals include:
1. **Design Hierarchical Fault Management:**
   - Create a Kubernetes Operator with multi-level supervision trees.
   - Improve fault isolation and recovery efficiency.
2. **Optimize Resource Utilization:**
   - Replace polling with real-time signal-based monitoring to lower CPU and RAM usage.
3. **Enhance Scalability:**
   - Evaluate performance in highly interdependent microservice environments.
4. **Provide Practical Guidelines:**
   - Develop actionable deployment recommendations for real-world Kubernetes systems.

---

## 🛠️ **Proposed Solution**
This research introduces a **Supervisory Model** for Kubernetes Operators based on Erlang’s supervision trees. Key components include:

1. **Hierarchical Supervision Trees:**
   - Supervisors monitor pods and isolate faults, preventing cascading failures.
   - Multi-level structures improve fault recovery and scalability.

2. **Signal-Based Monitoring:**
   - Replaces resource-heavy polling with event-driven health signals for near-instantaneous detection.
   - Reduces latency and system overhead.

3. **Targeted Recovery Strategies:**
   - Automates fault recovery, including pod restarts and resource reallocation.
   - Tailored strategies minimize Mean Time to Recovery (MTTR) and improve Service Level Objectives (SLOs).

---

## 📊 **Expected Outcomes and Insights**
### Key Outcomes:
- **Improved Fault Isolation:** Targeted recovery strategies reduce cascading failures.
- **Resource Savings:** Signal-based monitoring lowers CPU and RAM usage compared to polling.
- **Scalability:** Efficiently handles large-scale systems with interdependent services.
- **Real-World Applicability:** Deployment guidelines for sectors requiring high availability, like finance, healthcare, and IoT.

### Key Insights:
- **Faster Detection:** Near-instantaneous failure detection reduces MTTR.
- **Resource Efficiency:** Significant savings in CPU and RAM usage.
- **Practical Feasibility:** Demonstrates scalability within Kubernetes’ operational limits.

---

## 📧 **Contact**
For further inquiries or collaborations, please reach out:
- **Kyle Thomas**  
- Email: [2548971t@student.gla.ac.uk](mailto:2548971t@student.gla.ac.uk)  

---

**Thank you for your interest in this project!**
