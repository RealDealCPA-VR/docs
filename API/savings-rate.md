# Savings Rate Documentation

## What is the Savings Rate Response?

The savings rate response is returned by the API to provide the latest available interest rate for high-yield savings accounts or similar savings products. It includes the current rate, the type of account, the timestamp when the rate was retrieved, and the data source.

## Usefulness

This response is useful for financial applications and users who want to compare savings yields, model opportunity costs, or make informed decisions about where to allocate cash. By providing up-to-date savings rate data, it supports accurate financial planning and investment analysis.

## Example Response

```json
{
  "current_rate": 5.28,
  "rate_type": "High-yield savings account",
  "retrieved_at": "2025-08-28T19:48:24.634279",
  "source": "FRED 3-Month Treasury + 1.0% premium"
}
```

## Response Fields

- **current_rate** (`number`): The current annual interest rate for the savings product (percentage).
- **rate_type** (`string`): The type of savings account or product (e.g., "High-yield savings account").
- **retrieved_at** (`string`): The ISO 8601 timestamp when the rate was retrieved.
- **source** (`string`): The data source or methodology used to determine the rate.

## Notes

- The rate may change frequently; always use the latest value for calculations.
- The `source` field provides transparency about how the rate was determined.