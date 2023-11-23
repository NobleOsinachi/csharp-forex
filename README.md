# Forex Trading System

## Overview

This repository contains a simple console application for processing and matching buy and sell orders in a Forex trading system. The application reads orders from a text file, matches them based on specified criteria, and logs the successfully executed orders and pending orders.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [File Structure](#file-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/joshuaejiofor/csharp-forex/
    ```

2. Navigate to the project directory:

    ```bash
    cd csharp-forex
    ```

3. Build the solution using your preferred development environment.

## Usage

1. Ensure that you have the required dependencies installed (see [Dependencies](#dependencies)).
2. Run the compiled application.
3. The application will read orders from the provided "Orders.txt" file, process the orders, and display the successfully executed orders and pending orders.

## File Structure

- **/Data**: Contains the sample "Orders.txt" file used for input data.
- **/Forex.Models**: Defines the `Order` class.
- **Program.cs**: Main program file containing the logic for order processing.

## Dependencies

- [Newtonsoft.Json](https://www.newtonsoft.com/json): Used for JSON serialization.

Install dependencies using NuGet Package Manager:

```bash
nuget install Newtonsoft.Json
```

# Sample Output 

```bash
Successfully Executed Orders
{"OrderNo":4,"Type":"buy","Quantity":0.0,"Price":101.00,"Date":"2018-08-06T23:33:37+04:00"}
{"OrderNo":7,"Type":"sell","Quantity":0.0,"Price":100.45,"Date":"2018-08-06T23:45:55+04:00"}
{"OrderNo":9,"Type":"buy","Quantity":0.0,"Price":100.75,"Date":"2018-08-06T23:48:55+04:00"}



Pending Orders
{"OrderNo":1,"Type":"buy","Quantity":1.00000000,"Price":100.00,"Date":"2018-08-06T23:26:26+04:00"}
{"OrderNo":2,"Type":"sell","Quantity":1.32350000,"Price":104.00,"Date":"2018-08-06T23:27:31+04:00"}
{"OrderNo":3,"Type":"sell","Quantity":4.20000000,"Price":103.50,"Date":"2018-08-06T23:30:34+04:00"}
{"OrderNo":5,"Type":"sell","Quantity":2.25000000,"Price":100.75,"Date":"2018-08-06T23:35:12+04:00"}
{"OrderNo":6,"Type":"buy","Quantity":0.71600000,"Price":100.55,"Date":"2018-08-06T23:40:07+04:00"}
{"OrderNo":8,"Type":"sell","Quantity":2.20000000,"Price":103.50,"Date":"2018-08-06T23:48:55+04:00"}

D:\Applications\Forex\Forex\bin\Debug\netcoreapp3.1\Forex.exe (process 23996) exited with code 0.
To automatically close the console when debugging stops, enable Tools->Options->Debugging->Automatically close the console when debugging stops.
Press any key to close this window . . .
```

## Contributing

Contributions are welcome! Please follow the [contribution guidelines](CONTRIBUTING.md) when submitting pull requests.

## License

This project is licensed under the [MIT License](LICENSE).
