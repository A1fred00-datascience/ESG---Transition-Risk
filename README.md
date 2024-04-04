# ESG---Transition-Risk

## Transition Risk Evaluation Using NGFS Phase 3 Data

### Project Description

This project leverages the Network for Greening the Financial System (NGFS) Phase 3 data to evaluate transition risks under two primary scenarios: "Net Zero 2050" and "Current Policies". Our analysis aims to provide a comprehensive understanding of how different policy pathways can impact financial markets, investment strategies, and economic sectors.

### Scenarios Overview

- **Net Zero 2050**: This scenario envisions a world where concerted efforts and policies are implemented to reduce net greenhouse gas emissions to zero by the year 2050. It represents an ambitious but necessary target for mitigating the worst impacts of climate change.
- **Current Policies**: This scenario assumes the continuation of current climate policies and commitments, without additional measures to significantly reduce emissions. It serves as a baseline to understand the potential risks and impacts of inaction.

### Methodology

The methodology involves:

- **Data Integration**: Incorporating NGFS Phase 3 data into our analysis, focusing on key indicators relevant to transition risks.
- **Risk Modeling**: Developing models to quantify the financial impacts of the two scenarios on various sectors and geographies.
- **Scenario Analysis**: Comparing outcomes under the "Net Zero 2050" and "Current Policies" scenarios to identify areas of high risk and opportunity.

### Key Findings

Our preliminary findings indicate significant differences in transition risks between the two scenarios, with the "Net Zero 2050" scenario presenting both challenges and opportunities for early movers in green technologies and sustainable practices. The "Current Policies" scenario, meanwhile, suggests increased long-term risks due to the physical impacts of climate change and potential regulatory shifts.

### Implications

The analysis underscores the importance of forward-looking risk management and investment strategies that consider the long-term implications of climate policies. Financial institutions, investors, and policymakers can use these insights to align their strategies with a sustainable and resilient economic future.


## Code Overview

This project includes a Python script designed to evaluate transition risks associated with the "Net Zero 2050" and "Current Policies" scenarios, utilizing data from the Network for Greening the Financial System (NGFS) Phase 3. The script integrates financial and environmental data to assess the impact of these scenarios on different sectors, with a focus on the Power and Oil & Gas sectors.

### Key Features

- **Data Integration**: Combines NGFS Phase 3 data with sector-specific financial data to model transition risks.
- **Scenario Analysis**: Evaluates financial impacts under "Net Zero 2050" and "Current Policies" scenarios.
- **Risk Quantification**: Uses probabilistic models to quantify the risk of default under different transition scenarios.
- **Sensitivity Analysis**: Assesses how sensitive different sectors are to changes in carbon pricing, energy demand, and investment in low-carbon technologies.

### Libraries and Packages

The script utilizes the following Python libraries:

- `pandas` for data manipulation and analysis.
- `numpy` for numerical calculations.
- `scipy` for optimization and statistical functions.

### Model Parameters and Constants

The script defines several constants and parameters, including probability of default ratings, start and end years for the analysis, decay rates, and financial and environmental variables specific to the scenarios being analyzed.

### Functions

- **`client_selection`**: Filters clients based on subsector and outstanding amounts to select representative clients for analysis.
- **`climate_shock`**: Adjusts the ratings based on emissions and EBITDA to simulate the impact of climate-related financial shocks.
- **`calc_RFPs`**: Calculates Risk Factor Profiles (RFPs) using different financial and environmental variables.
- **`calc_decay`**: Calculates the decay of financial impacts over time, taking into account the sensitivities of different sectors to transition risks.
- **`error_alpha`** and **`error_sensitivities`**: Functions used in the optimization process to calibrate the model based on actual data.

### Execution Flow

1. **Data Preparation**: Reads portfolio data and NGFS data, selecting representative clients for analysis.
2. **Scenario Analysis**: Performs scenario analysis for "Net Zero 2050" and "Current Policies", adjusting ratings based on projected emissions and carbon pricing.
3. **Risk Quantification**: Calculates Risk Factor Profiles and decays of financial impacts to quantify transition risks.
4. **Output Generation**: Formats and outputs the analysis results to an Excel file for further review and decision-making.

### How to Use

To run the script, ensure you have the required data files (`CIB_Portfolio_Pre.xlsx` and `Phase_IV_Data.csv`) in the same directory as the script. Adjust the `SECTOR` and `SCENARIO` constants as needed to analyze different sectors and scenarios. Execute the script using a Python interpreter.




