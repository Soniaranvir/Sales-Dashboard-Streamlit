# Sales Dashboard with Streamlit, Plotly, and DuckDB 🚀

## Live Dashboard
[https://sales-dashboard-app-qrkzx6tezyzewgrumtmgl5.streamlit.app/
](https://sales-dashboard-app-cuwhttwlqiv3dhgz6yffvm.streamlit.app/)
## Why This Project? 🌟

An interactive Sales Dashboard built with Streamlit, Plotly, Pandas, and DuckDB, designed for financial data visualization and analysis. This prototype (v0.4.1) provides real-time insights into sales performance, budget vs. forecast comparisons, and financial KPIs.

As someone passionate about exploring data and understanding how various tools fit into the data analytics ecosystem, I set out to create a **Sales Dashboard**. The primary goal was to learn by doing—bringing together technologies like **Streamlit**, **Plotly**, and **DuckDB** to build an interactive, data-driven web application. This project wasn’t just about coding; it was about uncovering challenges, solving errors, and seeing firsthand how these concepts work in the real world.

## What I Built 🎯

The project resulted in a dynamic sales dashboard, providing key insights into metrics like yearly sales, monthly trends, and business performance. The dashboard includes:

- **Interactive Metrics**: Displays KPIs like total accounts receivable, equity ratio, and more using **Plotly**.
- **Bar Charts and Line Graphs**: Visualizing data trends across months, scenarios, and business units.
- **Streamlit Integration**: A lightweight yet powerful framework for creating web-based data applications.
- **DuckDB Queries**: A robust SQL engine for slicing and dicing the dataset.

## Features ✨

- **Dynamic Data Loading**: Uses `@st.cache_data` to efficiently load and preview Excel-based financial data.
- **Key Metrics & Gauges**: Displays financial indicators like total accounts receivable/payable, equity ratio, and debt-equity ratio with **Plotly Indicators & Gauges**.
- **Sales Performance Analysis**:  
  - **Bar Charts**: Visualize **yearly sales per business unit**.
  - **Line Charts**: Compare **monthly budget vs. forecast** for targeted business units.
  - **Aggregated Sales Trends**: Breakdown of actual vs. forecasted sales using **DuckDB SQL queries**.
- **Fully Responsive Layout**: Utilizes Streamlit’s column-based structure for an intuitive, structured dashboard.

## Tech Stack 🛠️

- **Streamlit**: Front-end framework for interactive dashboards.
- **Pandas**: Data manipulation and transformation.
- **Plotly**: Advanced visualizations with **express & graph_objects**.
- **DuckDB**: In-memory SQL engine for **fast & efficient** data querying.

## The Journey (a.k.a. Debugging Diaries) 💡

### Starting Simple:
The project began with loading an Excel dataset, bypassing Streamlit’s file uploader for simplicity. This allowed me to focus solely on the data visualization and application logic.

### DuckDB Queries:
Leveraging DuckDB for SQL queries on the dataset was both exciting and tricky. I learned how to unpivot data (turn months into rows) and aggregate it for meaningful insights.

### Errors and Lessons Learned:

- **File Loading Issues**: Initially, the app couldn’t locate the dataset. This taught me to double-check file paths and ensure datasets are correctly preloaded.
- **Module Not Found (DuckDB)**: Despite being installed, DuckDB raised errors. I resolved this by verifying dependencies, ensuring the Python virtual environment was active, and re-checking imports.
- **Streamlit Config Order**: A misplaced `st.set_page_config()` caused crashes, reminding me to always set configuration commands at the very beginning of the script.
- **Undefined Variables**: Debugging the dreaded 'NoneType' object found error emphasized the importance of properly initializing data and ensuring SQL queries have the right inputs.

### Iterative Refinement:
Each error was a learning opportunity, leading to a better understanding of Streamlit’s layout, Plotly’s flexibility, and DuckDB’s power.

## What I Learned 📚

- **Streamlit**’s simplicity makes it a great choice for rapid prototyping and deploying interactive dashboards.
- **Plotly** is a versatile library for creating stunning, dynamic visualizations.
- **DuckDB** is a hidden gem for SQL-like operations on local data, with impressive performance.
- Debugging and troubleshooting are as integral to coding as the actual writing of code itself.

## Why It Matters 🌍

This project was more than just a dashboard—it was a stepping stone into understanding how data transforms into insights through tools and technologies. Every error taught me something new, reinforcing the value of hands-on experimentation.

## 🚀 How to Run

1️⃣ Clone this repository:
```bash
git clone https://github.com/yourusername/sales-streamlit-dashboard.git
cd sales-streamlit-dashboard
