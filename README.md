# Incentive Projection Dashboard

A powerful, entirely client-side web application designed to project, calculate, and manage the Fiscal Year (FY26-27) incentive distributions for sales representatives and regional managers. 

It is natively styled according to the QuantumLeap UI/UX Brand Guidelines, ensuring data density, readability, and a strict, professional aesthetic.

## 🚀 Features

- **Interactive 12-Month Matrix**: Input product sales volumes dynamically and watch the entire year extrapolate instantly without page reloads.
- **Global Financial Summary**: Track Fiscal Year totals in real-time including Total Collected Revenue, Expense Percentage, Total Incentives, and Product Volume Splits.
- **Mid-Year Salary Appraisals**: Configure distinct "Appraisal In" drop-down triggers to calculate base salary raises seamlessly midpoint through the year. 
- **Automated Incentive Slabs**: Mathematically routes team members into distinct commission slabs (e.g., 3%, 4%, 6%) based on combined Unit and Collection thresholds.
- **Manager Target Overrides**: Evaluates global team collection targets and automatically calculates manager payout overrides.
- **Persistent LocalStorage**: Retains your dashboard state completely offline entirely within the browser caching system.
- **CSV Export Engine**: Download your entire fiscal year projection spreadsheet natively to `.csv` in one click.

## 📂 Repository Structure

```text
.
├── index.html               # Main Application execution file
├── brand-guidelines.html    # QuantumLeap UI/UX CSS Documentation
├── README.md                # Project documentation
└── .gitignore               # Standard ignore configurations (macOS/system files)
```

## 🛠️ Usage & Installation

Because the architecture relies entirely on native browser features (`HTML5`, `Vanilla JS`, `Vanilla CSS`), there are strictly **no dependencies**, Node modules, or complex build pipelines needed to run the dashboard.

1. **Clone the Repository** (or download the ZIP):
   ```bash
   git clone https://github.com/your-username/incentive-projection-dashboard.git
   ```
2. **Execute**: 
   Simply double-click `index.html` to open it in any modern browser (Chrome, Edge, Safari). Alternatively, launch it using an extension like VSCode's *Live Server* for local hosting.

## 🔒 Security & Data Privacy
The application does not invoke any backend databases, external APIs, or analytics trackers. All sensitive payroll data, salaries, and roster metrics remain strictly confined locally to the user's browser via the `localStorage` API. To clear the cache, simply clear your browser site data or use a secondary browser profile.
