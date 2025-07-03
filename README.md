# Fund Compare Tool [Try It](http://sternetj.github.io/fund-compare-tool/index.html)

A tool for comparing ETF and mutual fund investment scenarios with interactive charts and detailed projections.

## Overview

The Fund Compare Tool is a single-page web application that allows users to model and compare different investment funds based on key parameters like initial investment, rate of return, expense ratios, sales loads, and annual contributions. It provides both visual (interactive charts) and tabular data to help users make informed investment decisions.

## Features

### 📊 Interactive Fund Comparison
- Add multiple funds with different investment parameters
- Real-time chart visualization using Chart.js
- Side-by-side comparison of fund performance over time

### 💰 Comprehensive Investment Modeling
- **Initial Investment**: Starting amount for each fund
- **Rate of Return**: Expected annual return percentage
- **Expense Ratio**: Annual fund management fees
- **Sales Load**: One-time commission or load fees when purchasing new funds
- **Annual Contributions**: Regular yearly investments
- **Projection Period**: Customizable time horizon (default: 30 years)

## How to Use

1. **Add a Fund**: Fill in the fund parameters and click "Add Fund"
2. **Compare Funds**: Add multiple funds to see side-by-side comparisons
3. **Edit Existing Funds**: Click on any fund in the chart legend to load its parameters for editing
4. **View Details**: Hover over legend items to see fund details in a popup
5. **Adjust Timeline**: Change the "Years to Project" value to see different time horizons

## Technical Details

- **Frontend**: Pure HTML, CSS, and JavaScript
- **Charts**: Chart.js library for interactive visualizations
- **Storage**: Browser localStorage for data persistence
- **No Dependencies**: Self-contained single HTML file
- **Cross-Platform**: Works in any modern web browser

## Investment Calculations

The tool calculates fund growth using the following formula:
- Initial value = `Initial investment` × (1 - `Sales load`)
- Annual growth = `Previous value` × (1 + `Rate of return` - `Expense ratio`)
- Annual contribution = `Yearly contribution` × (1 - `Sales load`)

This accounts for the impact of fees and loads on long-term investment performance.

## License

This tool is provided as-is for educational and personal use.
