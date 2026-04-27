# AI-Based Detection of Parameters from Asset Nameplate Images

**Service:** AI-Based Detection of Parameters from Asset Nameplate Images  
**Document Type:** Technical Manual & Service Specification  
**Author:** ELES  
**Version:** 1.0  
**Last Updated:** 12 Feb 2026  

---

# 1. Business Context & Definitions

The purpose of this service is to process and analyse asset nameplate images and apply AI techniques to detect the technical information and parameters of the assets. The generated results will enable faster and more accurate asset data inventory and support the digitalization of processes.

The service will also improve the quality of the existing database, as some parameters are not currently listed in the EAM.

## Key Terms

| Term | Definition |
|---|---|
| Asset Nameplate | A physical plate or label on substation assets that contains essential basic, technical, and operational information or parameters |

## 1.1 ELES (Asset Nameplate Images Owner) Context

The service is intended for ELES, the combined transmission and distribution system operator of the Republic of Slovenia. With a professional approach, know-how, and advanced technology, ELES has been providing safe, reliable, and uninterrupted electric power transmission throughout Slovenia and across its borders for 100 years. The company connects people and ensures quality of life while strategically planning, constructing, and maintaining Slovenia’s high-voltage transmission network at 400 kV, 220 kV, and part of the 110 kV network.

ELES owns numerous substation assets, each equipped with a nameplate containing key parameters and information. These nameplates serve as a valuable information source for the EAM but currently require manual parameter identification by field employees. This service enables digitalization of this process, allowing faster and more efficient data collection.

---

# 2. Problem Statement

The primary goal of the service is to provide a mature, production-ready platform or algorithm that takes raw asset nameplate images as input and returns digitalized attributes with values extracted from recognized information or parameters on the nameplates.

The service must meet high professional standards as it will serve as a key tool for digitalization of asset parameters.

---

# 3. Data Description

No real data are available due to sensitivity concerns.

- The algorithm or platform must be trained and tested using dummy images  
- The design should allow future integration of real asset nameplate images  

---

# 4. Analytics, Scope & Update Frequency

## Temporal Scope
The number of asset nameplate images will be defined at a later stage.

## Update Frequency
- The service will initially analyse a predefined dataset of dummy nameplate images  
- The production version will process each new image automatically as it is received  

## Output Format

Results are stored in structured tables.

Each table (per analysed image) includes:
- All detected attributes from the asset nameplate  
- Corresponding values for each attribute  

---

# 5. Evaluation Protocols & Metrics

The service must be evaluated to verify whether detected attributes and values match the actual information on nameplates.

Special consideration:
- Nameplates are not standardized  
- Formats vary significantly across assets  

## 5.1 Data Usage & Analytical Protocol

- The service shall process a predefined number of nameplate images  
- The system must support future real-time operation on incoming images  
- All outputs must be reproducible with:
  - Documented model versions  
  - Configuration parameters  
  - Input datasets  

## 5.2 Data Gaps and Exceptions

- The service must detect all attributes and their corresponding values  
- The system shall provide feedback when image quality is insufficient for analysis  

## 5.3 Service Evaluation Metrics & KPIs

| Metric | Description |
|---|---|
| Classification accuracy | Measures correct detection and classification of asset information and parameters |
| Reduction in digitalization time (%) | Efficiency improvement vs manual process (KPI = (manual_time – tool_time) / manual_time × 100%) |

---

# 6. Deliverables & Submissions

The provider shall deliver three reports aligned with the service lifecycle, along with technical specifications and deployment artefacts.

## 6.1 Deliverable Reports

1. **Pre-Service Deliverable – Service Design & Setup Report**  
   Includes:
   - Analytical approach  
   - Detection methodology  
   - Baseline definition  
   - Data requirements  
   - System architecture  
   - Security measures  
   - Integration plan  
   - Operational schedule and procedures  

2. **Intermediate Deliverable – Interim Performance & Operations Report**  
   Includes:
   - Service operation summary  
   - Data coverage  
   - Preliminary results (structured tables)  
   - KPI performance  
   - Issues and refinements  

3. **Final Deliverable – Final Evaluation & Recommendations Report**  
   Includes:
   - Final performance results  
   - Process insights  
   - Identified inefficiencies  
   - Improvement recommendations  
   - Lessons learned  
   - Guidance for scaling  

## 6.2 Technical Specifications & Submissions

- **Service Interface Documentation**
  - API documentation  
  - Structured tables and data formats  
  - Authentication  
  - Access control  

- **Deployment Artefacts**
  - Description of deployment approach  

- **Configuration, Versioning & Handover**
  - Configuration parameters  
  - Model and data versioning  
  - Handover procedures  

- **Security & Data Protection Documentation**
  - Data handling procedures  
  - Cybersecurity measures  
  - Access control  
  - Compliance with data protection requirements  

---

The above specification is not final. Both the service provider and the customer may modify parts of the specification prior to or during development if required for proper service performance.
