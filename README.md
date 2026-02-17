# Volatility Surface Builder

[![Python Version](https://img.shields.io/badge/python-3.7%2B-blue.svg)](https://www.python.org/downloads/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> A Python tool for constructing and visualizing the volatility surface for stock options.

This application fetches live option chain data, calculates the implied volatility for each option, and generates both a 2D volatility smile and a 3D volatility surface. It is designed for finance professionals, students, and anyone interested in options analytics.

## Table of Contents

- [Features](#features)
- [Understanding Implied Volatility](#understanding-implied-volatility)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

-   **Live Option Chain Data**: Fetches real-time option chain data for any stock ticker using yfinance.
-   **Implied Volatility Calculation**: Uses the Black-Scholes model and a robust numerical solver to calculate IV.
-   **Advanced Visualizations**:
    -   **Volatility Smile**: A 2D plot of implied volatility vs. strike price for a single expiration date.
    -   **Volatility Surface**: A 3D surface plot of implied volatility vs. strike price and time to maturity.
-   **Professional UI**: A dark-themed, finance-style plot generated with Matplotlib.

## Understanding Implied Volatility

**Implied Volatility (IV)** is the market's forecast of a likely movement in a security's price. It is the volatility value that, when input into an option pricing model (like Black-Scholes), returns the current market price of the option.

The **Volatility Smile** is a common pattern where options with the same expiration date but different strike prices have different implied volatilities. This creates a "smile" shape when plotted.

## Tech Stack

-   Python
-   yfinance
-   pandas
-   numpy
-   matplotlib
-   scipy

## Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/AbhiramSharma/Volatility-Surface-Builder.git
    cd Volatility-Surface-Builder
    ```

2.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

To run the volatility surface builder, execute the following command:

```bash
python main.py
```

## File Structure

-   `main.py`: The main script for fetching data, calculating IV, and generating the plots.
-   `black_scholes.py`: Contains the Black-Scholes pricing formula.
-   `iv_solver.py`: The numerical solver for calculating implied volatility.
-   `requirements.txt`: A list of the Python dependencies for the project.
-   `README.md`: This file.

## Contributing

Contributions are welcome! If you have ideas for new features or improvements, feel free to fork the repository and submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

This project is licensed under the MIT License - see the `LICENSE` file for details.

*Disclaimer: This project is for educational and research use only. It is not investment advice.*

## Contact

Abhiram Sharma - ab23.ar39@gmail.com

Project Link: [https://github.com/AbhiramSharma/Volatility-Surface-Builder](https://github.com/AbhiramSharma/Volatility-Surface-Builder)
