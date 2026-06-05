# Simple Interest Calculator

A simple, lightweight command-line tool designed to quickly calculate the simple interest earned or owed based on principal, annual interest rate, and time period.

## Purpose
The purpose of this project is to provide a straightforward script for financial calculations, helping users understand how investments or loans accrue interest over time using a basic linear calculation model.

## Formula
The application utilizes the standard simple interest formula:

A = P(1 + rt)

Where:
- **P** = Principal amount (initial investment or loan)
- **r** = Annual interest rate (as a decimal)
- **t** = Time period (in years)

## How to Use
To run the simple interest calculator in your terminal, use the bash script provided in the repository.

1. Make the script executable (if needed):
```bash
   chmod +x simple-interest.sh
2.  Run the script:

Bash
   ./simple-interest.sh

3. Input the requested values (Principal, Rate, Time) when prompted to view your calculated interest return.


Example Code Snippet
The core logic relies on simple variables to compute the total interest accrued:

# Sample implementation logic
def calculate_simple_interest(principal, rate, time):
    # rate is passed as a percentage (e.g., 5 for 5%)
    interest = (principal * (rate / 100) * time)
    total_amount = principal + interest
    return interest, total_amount

# Example Case: $1,000 principal at 5% interest for 3 years
interest, total = calculate_simple_interest(1000, 5, 3)
print(f"Interest Earned: ${interest}") # Output: $150.0
print(f"Total Value: ${total}")        # Output: $1150.0
