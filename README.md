# CBAC-Rag-LLM-CSE453


# RAG Security: Preventing Sensitive Information Disclosure using Access Control Mechanisms

## Objectives

1. **Prevent Sensitive Information Disclosure**
   - Design a Retrieval-Augmented Generation (RAG) application to minimize the exposure of Personally Identifiable Information (PII) using advanced redaction methodologies and access control systems.

2. **Implement Automated PII Reduction**
   - Utilize machine learning algorithms to detect and mask sensitive information in real time, ensuring the privacy of both queries and document collections.

3. **Design and Integrate Specialized Access Control Systems**
   - Use Context-Based Access Control (CBAC) to restrict data access based on user permissions, request context, and data sensitivity.

4. **Evaluate Security and Performance of the RAG System**
   - Develop a multi-layered security framework, including differential privacy and model auditing, to ensure compliance with data privacy regulations while maintaining system effectiveness.



## Problem Statement

As Large Language Models (LLMs) are increasingly deployed in sensitive fields such as healthcare, finance, and law, the risk of disclosing confidential or PII becomes a significant concern. This project addresses these issues by developing a secure RAG application focusing on:

- **PII Redaction**
- **Context-Based Access Control Systems**

### Key Features
- Automatic detection and redaction of PII from queries and documents.
- Dynamic access control based on user roles and query context.
- A robust security framework ensuring safe LLM deployment in privacy-sensitive environments.



## Literature Review

### Key Insights
1. **Real-Time Data Masking**
   - Studies, such as Khoje (2024), highlight the use of anonymized placeholders to maintain privacy while enabling third-party analytics.

2. **Cybercrime Risks**
   - Kshetri (2023) emphasizes risks like phishing and scams facilitated by LLMs and suggests using content filtering and encryption.

3. **Prompt Injection Attacks**
   - Das et al. (2024) discuss vulnerabilities such as prompt injection and jailbreaking attacks, advocating defenses like differential privacy.

4. **Comprehensive Threat Categorization**
   - Yao et al. (2024) propose methods to address vulnerabilities across hardware, OS, and network levels.


## Methodology

Our multi-layered approach prioritizes both data privacy and performance:

1. **Vector Database Setup**
   - Tools like Pinecone or FAISS store document embeddings categorized by specific access levels (e.g., HR or finance).

2. **Context-Based Access Control (CBAC)**
   - Dynamically evaluates both user roles and query context for adaptable data access.

3. **Robust Testing Framework**
   - Includes adversarial prompts and high-volume query simulations to assess privacy leakage rates.


<div align="center">
    <img src="https://github.com/user-attachments/assets/d359bf1e-83b1-4b4b-95e6-84aec37c176b" alt="System Overview" height = "900px" width="70%">
    <p><b>Figure 1:</b> Methodology Overview</p>
</div>


## Results

### System Performance
- **Privacy Leakage Rates**: Below 2% across adversarial prompts.
- **Response Time**: Maintained sub-second latency with high query volumes.

### Security Enhancements
- Successfully implemented differential privacy and dynamic CBAC.
- Improved resilience against prompt injection and jailbreaking attacks.


<div align="center">
    <img src="https://github.com/user-attachments/assets/d4ee94ee-db23-4988-9de5-ffc378361985" alt="Privacy Leakage Rates" width="70%">
    <p><b>Figure 2:</b> Privacy Leakage Rates</p>
</div>

<div align="center">
    <img src="https://github.com/user-attachments/assets/09777c05-12ea-4de6-99e5-69b15dc0056a" alt="Response Time Performance" width="70%">
    <p><b>Figure 3:</b> Response Time Performance</p>
</div>

<div align="center">
    <img src="https://github.com/user-attachments/assets/1c7405d3-f72b-43f3-8140-8284ebbce3b1" alt="Dynamic CBAC Implementation" width="70%">
    <p><b>Figure 4:</b> Dynamic CBAC Implementation</p>
</div>

<div align="center">
    <img src="https://github.com/user-attachments/assets/4b88abaf-ce81-4d96-9401-77a2d4ce4703" alt="Resilience Against Attacks" width="70%">
    <p><b>Figure 5:</b> Resilience Against Attacks</p>
</div>


## Future Work

1. Expand the system to support multi-modal data (e.g., text, images, videos).
2. Incorporate federated learning for distributed privacy-preserving computations.
3. Evaluate performance with larger datasets and diverse adversarial scenarios.



## Conclusion

This project demonstrates the potential for secure RAG systems to balance data utility and privacy in sensitive environments. By integrating advanced redaction techniques and dynamic access control, our solution addresses key challenges in deploying LLMs safely.


