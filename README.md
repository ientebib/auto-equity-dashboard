# Auto Equity Funnel Analysis Dashboard

A modern, interactive Streamlit dashboard for analyzing Auto Equity funnel data, focusing on how user attributes and loan terms affect progression through various conversion stages.

![Dashboard Screenshot](https://i.imgur.com/placeholder.png)

## Features

- **Modern UI/UX Design**: Clean, Apple-inspired interface with translucent backgrounds and intuitive navigation
- **Comprehensive Funnel Analysis**: Visualize user progression through the entire sales funnel
- **Customer Type Breakdown**: Analyze performance differences between new and existing customers
- **Stage-to-Stage Comparison**: Compare key metrics across funnel stages
- **Drop-off Analysis**: Identify where and why users leave the funnel
- **Key Insights Tab**: Summary of critical metrics and actionable recommendations
- **Detailed Metric Analysis**: Compare interest rates, monthly payments, installment periods, and more
- **Fully Responsive Design**: Works on desktop, tablet, and mobile devices

## Installation

1. Clone this repository:
```bash
git clone https://github.com/ientebib/auto-equity-dashboard.git
cd auto-equity-dashboard
```

2. Create a virtual environment (optional but recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install the required packages:
```bash
pip install -r requirements.txt
```

## Usage

1. Ensure you have your funnel data CSV file ready
2. Update the file path in `app.py` if needed (default location is desktop)
3. Run the Streamlit app:
```bash
streamlit run app.py
```
4. The dashboard will automatically open in your default web browser at http://localhost:8501

## Dashboard Structure

The dashboard is divided into four main tabs:

1. **Funnel Overview**: 
   - Overall funnel progression
   - Customer type distribution
   - Stage-by-stage user counts
   
2. **Stage Comparison**:
   - Profiling status across stages
   - Monthly payment distribution by stage
   - Installment period analysis
   
3. **Drop-off Analysis**:
   - Detailed analysis of key drop-off points
   - Conversion metrics between stages
   - Factor comparison between successful and unsuccessful conversions
   
4. **Key Insights**:
   - Success rate metrics
   - Comparative analysis of key user cohorts
   - Recommendations based on data analysis

## Data Requirements

The dashboard expects a CSV file with the following columns:
- `final_funnel_stage`: The final stage the user reached in the funnel
- `growth_customer_type`: Type of customer (new or existing)
- `profiling_status`: User's profile approval status
- `interest_rate`: Interest rate offered (for applicable stages)
- `monthly_payment`: Monthly payment amount (for applicable stages)
- `installment_period`: Loan period in months
- `monthly_income`: User's monthly income

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.