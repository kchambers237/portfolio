# Quant Risk Manager • Physicist & Computer Sciencist


## Education
* B.Sc Physics & Computer Science     University of Buea(Cameroon)
* Fundamental of Mech. Eng.(Rail Vehicle Engineering)  FH Aachen(Germany)

## Work Experience
### Risk Manager-Quant Analyst Methods and Models @ TRIANEL (Apr 2025 - Oct 2025), Germany
* Develop and refine risk models, valuation frameworks, and quantitative KPIs.
* Omn and maintain core risk tools to ensure reliable, production-grade performance.
* Run complex statistical and quantitative analyses to support high-stakes decisions.
* Optimize valuation workflows and build effizient, scalable data pipelines.

### IT-Specialist @ Aachen Institute of Applied Sciences (Dec 2024 - Apr 2025), Germany
* Ensured system stability, data integrity, and efficient operation of core IT systems.
* Performed technical analyses, diagnostics, maintenance, and supported the integration of solutions.
* Collaborated with cross-functional teams to implement IT-driven solutions and optimize business processes.

### Academic Tutor @ Aachen Institute of Applied Sciences (Apr 2023 - present), Germany
* Guide and support students in exercises, seminars, and tutorials to deepen understanding of course content.
* Deliver subject-matter explanations, answered technical questions, and assisted with assignments and project work.
* Create and structure learning materials, summaries, and solution guides.
* Assist in organizing courses, seminars, and eximinations.
* Encourage independent learning through target group support and structtured guidance.

### Software & Hardware Developer @ Aerial Photovoltaic Inspection GmbH (Aug 2021 - Jun 2022)
* Engineered embedded software and hardware for GPS-based photoltaic measurement systems, with a strong focus on data quality and system reliability.
* Processed and analysed large sensor datasets (mining, cleaning, visualization, modelling) to extract actionable insights and support algorithm development.
* Developed microcontroller-based IR modules, including requirements analysis, module configuration, power designm and implementation of low-level control logic.

# Projects
## Hourly Price Forward Curve  
### A market-consistent, two-stage modelling 
![HPFC](assests/hpfc/images/hpfc.png)
[HPFC modelling](hpfc.pdf)
[HPFC code](hpfc.ipynb)
Objective:
Develop a market-consistent hourly forward curve for electricity prices, suitable for risk assessment and valuation.
### Approach:
•	Two-stage linearized model separating intraday shape from weekly price level
•	Stage 1: Predict peak/off-peak shapes on normalized prices
•	Stage 2: Reintroduce weekly prices via weekly scaling 
•	Integrate solar production effects with seasonal bucketing
### Key Features:
•	Exact preservation of weekly base prices
•	Stable and interpretable estimation
•	Explicit structural constraints
•	Fully auditable, modular Python implementation
Validation:
•	HPFC vs observed price diagnostics
