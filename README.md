# LLM-Based Hospital Patient Triage & Doctor Assignment Agent

## 📌 Project Overview

This project explores the use of **Large Language Models (LLMs) and AI Agents** to support hospital patient triage and doctor assignment workflows.

The system is designed to process patient information, identify the nature and urgency of a patient's reported condition, and recommend an appropriate medical department or doctor based on the available information.

The goal is to demonstrate how **LLM-based agents, structured decision-making, and workflow automation** can be combined to assist healthcare operations.

> **Important:** This project is intended for educational and research purposes. It is not a replacement for qualified medical professionals, clinical judgment, emergency services, or hospital protocols.

## 🎯 Objectives

* Process patient information using an LLM-based agent.
* Extract relevant information from natural-language patient descriptions.
* Categorize patients according to the reported symptoms and urgency.
* Recommend an appropriate medical department.
* Match patients with suitable doctors based on predefined criteria.
* Automate parts of the patient-routing workflow.
* Demonstrate the use of LLMs for structured decision-support applications.

## 🧠 Key Features

* **Natural-language patient input**
* **LLM-based information extraction**
* **Symptom and complaint analysis**
* **Triage categorization**
* **Department recommendation**
* **Doctor assignment / recommendation**
* **Structured output generation**
* **Rule-based and AI-assisted decision logic**
* **Workflow automation**

## 🏥 System Architecture

```text id="m9b9j7"
Patient Information
        ↓
Natural Language Processing
        ↓
LLM-Based Agent
        ↓
Information Extraction
        ↓
Triage Assessment
        ↓
Urgency / Category Identification
        ↓
Department Matching
        ↓
Doctor Availability / Specialty Matching
        ↓
Doctor Recommendation
        ↓
Structured Output
```

## 🔄 Workflow

The system follows a multi-stage workflow:

### 1. Patient Input

The system receives information such as:

* Patient complaint
* Reported symptoms
* Duration of symptoms
* Relevant background information
* Other available non-sensitive patient details

### 2. Information Extraction

The LLM processes the natural-language input and extracts relevant structured information.

Example:

```text id="70frt8"
Input:
"I have been experiencing persistent chest discomfort
and shortness of breath."

        ↓

Extracted Information:
Complaint: Chest discomfort
Additional symptom: Shortness of breath
Potential urgency: Requires prompt professional assessment
```

### 3. Triage Classification

The agent categorizes the case according to the project's predefined triage framework.

For example:

```text id="8xmb2b"
Patient Input
     ↓
┌─────────────────────────┐
│    Triage Assessment    │
└─────────────────────────┘
     ↓
Urgency Category
     ↓
Department Recommendation
```

The triage output should be treated as **decision support only**, not as a clinical diagnosis.

### 4. Department Matching

Based on the extracted information, the system identifies the most relevant hospital department or specialty.

Example:

```text id="n9h5t5"
Symptoms / Complaint
        ↓
Clinical Category
        ↓
Relevant Specialty
        ↓
Available Department
```

### 5. Doctor Assignment

The system can use structured information about doctors, such as:

* Specialty
* Department
* Availability
* Experience/category
* Appointment schedule

to recommend an appropriate doctor.

## 🤖 LLM / Agent Component

The LLM acts as an intelligent processing layer between unstructured patient input and structured hospital workflow logic.

Potential responsibilities include:

* Extracting symptoms and relevant information.
* Converting natural-language descriptions into structured fields.
* Identifying the relevant specialty.
* Assigning a predefined triage category.
* Generating structured recommendations.
* Passing structured information to downstream workflow components.

A structured output format can be used to make the agent's response easier to process:

```json
{
  "patient_complaint": "...",
  "symptoms": [],
  "urgency_category": "...",
  "recommended_department": "...",
  "recommended_specialty": "...",
  "doctor_recommendation": "..."
}
```

## 🛠️ Technologies Used

Depending on the implementation, the project can use:

* **Python**
* **Large Language Models (LLMs)**
* **LLM APIs**
* **Prompt Engineering**
* **AI Agents**
* **REST APIs**
* **JSON**
* **Pandas**
* **Workflow Automation Tools**

## 📊 Evaluation

The system can be evaluated across several dimensions:

### Information Extraction

* Accuracy of extracting relevant information.
* Consistency of structured outputs.
* Robustness to different patient descriptions.

### Routing

* Correct department recommendation.
* Appropriate specialty matching.
* Correct use of available doctor information.

### Reliability

* Structured output validity.
* Handling of ambiguous inputs.
* Appropriate escalation of potentially urgent cases.
* Resistance to unsupported medical conclusions.

## 📁 Repository Structure

```text id="6pxp4z"
LLM-Based-Hospital-Patient-Triage/
│
├── README.md
├── src/
│   ├── agent.py
│   ├── triage.py
│   └── doctor_assignment.py
│
├── data/
│   └── doctors.csv
│
├── prompts/
│   └── triage_prompt.txt
│
├── tests/
│
├── requirements.txt
└── .env.example
```

> The repository structure may be updated as the project evolves.

## 🔐 Privacy & Security

Healthcare applications require careful handling of sensitive information.

This project should:

* Avoid storing unnecessary patient information.
* Never commit API keys or credentials to GitHub.
* Use anonymized or synthetic data for development.
* Apply appropriate access controls in production environments.
* Follow applicable healthcare privacy and data-protection requirements.

## ⚠️ Safety Disclaimer

This project is a **technical demonstration of LLM-based workflow automation and decision support**.

It must **not** be used to:

* Diagnose medical conditions.
* Replace a doctor or other qualified healthcare professional.
* Make autonomous emergency-care decisions.
* Override hospital triage protocols.
* Provide treatment or medication recommendations without qualified clinical oversight.

In a real hospital environment, outputs should be reviewed and governed by qualified healthcare professionals and institutional protocols.

## 🚀 Future Improvements

* Integrate real-time doctor availability.
* Add hospital appointment scheduling.
* Introduce human-in-the-loop approval.
* Add multilingual patient input.
* Improve structured output validation.
* Add audit logs for agent decisions.
* Evaluate the system against curated test cases.
* Integrate hospital information systems through secure APIs.
* Add monitoring for hallucinations and unsafe outputs.
* Develop a clinician-facing dashboard.

## 👨‍💻 Author

**Bhanu Pratap**

M.Tech — IIT Bombay

---

⭐ This project demonstrates the application of **LLMs and AI agents to healthcare workflow automation and decision-support systems**.
