# Patent Analytics – SP3H Case Study

This repository contains a **patent analytics case study** analyzing the innovation and intellectual property strategy of the French deeptech company **SP3H**, using data from the **PATSTAT** database (European Patent Office).

The project applies tools from **economics of innovation**, **data analysis**, and **patent analytics** to understand how a small technology-driven firm structures, protects, and positions its innovations over time.

This work was developed as part of a **Master’s degree in Data Science and Economics** at Université Paris Nanterre.

---

## Project Objective

The objective of this study is to characterize:
- the **innovation dynamics** of SP3H,
- its **geographical patenting strategy**,
- its **technological specialization**,
- and its **competitive positioning**  
through a structured analysis of its patent portfolio.

Rather than focusing on individual patents, the project adopts a **portfolio-level perspective**, consistent with standard approaches in patent analytics.

---

## Data Source

- **Database**: PATSTAT Global (European Patent Office)
- **Key tables used**:
  - `tls201_appln` – patent applications
  - `tls206_person` / `tls207_pers_appln` – applicants and inventors
  - `tls209_appln_ipc` – technological classifications (IPC)
  - `tls211_pat_publn` – publications
  - `tls212_citation` – citations

The portfolio was identified by filtering patent applications where **SP3H appears as applicant**.

📌 Due to licensing and size constraints, **PATSTAT data are not included** in this repository.

---

## Methodology

### 1. Portfolio Identification
- Text-based filtering on applicant names (SP3H, SP3H SAS)
- Exclusion of cases where SP3H appears only as inventor
- Construction of a clean portfolio of **99 patent applications**

### 2. Innovation Dynamics
- Analysis of patent filings over time
- Identification of **cyclical innovation patterns**
- Distinction between phases of intensive R&D and consolidation

### 3. Geographical Strategy
- Analysis of filing offices (FR, EP, WO, US, CN)
- Study of the use of **PCT procedure** as a strategic option
- Comparison between filing offices and publication offices
- Measurement of internationalization through **DOCDB family size**

### 4. Technological Profile
- Mapping of patents using **IPC classifications**
- Identification of core technological domains
- Measurement of specialization vs controlled diversification

### 5. Cooperation & Competition
- Identification of **co-deposited patents**
- Analysis of R&D collaboration patterns
- Identification of technological competitors through shared patent families

### 6. Patent Quality Indicators
- Citation analysis (with discussion of limitations)
- Use of publication offices as a proxy for patent value
- Interpretation of quality signals in the context of a PME deeptech

---

## Key Findings

- SP3H’s innovation activity is **structured in cycles**, not continuous
- The firm adopts a **selective international patenting strategy**
- A small number of **core patent families** concentrate most of the protection effort
- Strong technological specialization in **measurement, sensors, and spectroscopy**
- Limited but targeted R&D collaborations
- Patent quality is reflected more by **jurisdiction choice** than by citation counts

Overall, the portfolio reflects a **coherent and cost-aware IP strategy**, consistent with the profile of a specialized deeptech SME.

---

## Technologies & Tools

- SQL (PATSTAT queries)
- Python (data processing & visualization)
- Pandas / NumPy
- Matplotlib
- LaTeX (report writing)

---

## Repository Structure
```
├── Data/
├── Code/
├── Patent Analytics – SP3H Case Study.pdf      # Full written report
├── README.md
```

---

## Why This Project Matters

This project demonstrates the ability to:
- Work with **large, relational innovation databases**
- Translate raw patent data into **strategic insights**
- Combine **economic theory** with **data-driven analysis**
- Produce structured analyses relevant for **R&D strategy, policy, and innovation studies**

It reflects my interest in applying data science to **innovation, technology strategy, and real-world decision-making**.

---

## Author

**Sika**  
Data Scientist | Economics of Innovation & Patent Analytics  

---

## Notes

This repository is shared for educational and portfolio purposes.  
Feedback and discussions are welcome.
