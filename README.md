# Cybersecurity Portfolio: Charlotte

**Welcome to my playground.** 90% broken containers &amp; fixed logs, 10% success. Showcasing my thesis on Federated Learning Security monitoring and other experiments where I break things to understand how to secure them.

---

### Hi, I'm Charlotte
I am a Cybersecurity student graduating in December 2025. This portfolio documents my journey from software development to defensive security operations. 

My primary focus is understanding how systems are built, how they break, and how to detect anomalies using logs and monitoring tools. I am known for a steadfast attitude - I don't just look for easy answers; I dig deep to understand the root cause of technical problems.

---

## Featured Project: SA-FLaaS Security Monitoring (Thesis)
**Topic:** Security Monitoring & Anomaly Detection for Federated Learning System 

**Tech Stack:** Python, Docker, Grafana, Loki, Promtail, Watchdog API


<img width="886" height="443" alt="Monitoring Architecture" src="https://github.com/user-attachments/assets/e1a7700f-8761-4aac-97da-81ebb2bfa053" />



*System Architecture Diagram*

In my thesis, I designed and implemented a security monitoring prototype for a Federated Learning environment. The goal was to detect tampering attempts and ensure traceability in compliance with the EU AI Act.

**Key Highlights:**
* **Built a "Mini-SOC" Pipeline:** Configured a full monitoring stack (Promtail -> Loki -> Grafana) to collect real-time data from distributed containers.
* **Implemented Anomaly Detection:** Created a custom "Sidecar" monitor (Python Watchdog) that correlates filesystem events with application logs.
* **The "Use Case":** Successfully detected a simulated "Fake Training" attack where a client claimed to train a model but did not access the dataset.

**Visuals:**

<img width="1299" height="395" alt="eka_" src="https://github.com/user-attachments/assets/5862951b-70cd-4bf1-92cf-8b0dbae37188" />

*Valid Training Session. Note the perfect alignment between the Client Claims (Blue) and Sidecar Observations (Orange).*


<img width="886" height="264" alt="image" src="https://github.com/user-attachments/assets/7c59e8f2-3e00-407e-afe2-24b402e4d63b" />

*The "Fake Training" Anomaly (see the last bar). The dashboard reveals a mismatch: The client claims to be training (Blue bar), but the Sidecar (Orange bar) shows zero file activity. This indicates a potential Repudiation or Model Poisoning attempt.*


<img width="1299" height="284" alt="LogIntegrity" src="https://github.com/user-attachments/assets/278b03f7-de40-4f87-860e-602cf63fa2ec" />

*Log Integrity Alert (Anti-Forensics). The dashboard captures a **CRITICAL** event where the monitor detected that the audit log file size shrank (truncation), indicating an attempt to destroy evidence.*




---

## Technical Skills

* **Security Operations:** Log Analysis, Anomaly Detection, Incident Response basics (simulated).
* **Monitoring & Data:** Grafana, Loki, Promtail, ELK Stack basics.
* **Infrastructure:** Docker, Linux (Bash), Sidecar Patterns.
* **Programming:** Python (Automation, Scripting, Watchdog API). 
* **Soft Skills:** Problem-solving, Documentation, Teamwork, Regulatory Analysis (EU AI Act).

---

### Contact Me
* **Email:** charlotte.levula@gmail.com

*"I am not looking for the easy way out. I am looking for the challenge that teaches me the most."*
