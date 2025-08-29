# Mortgage Rate Documentation

## What is the Mortgage Rate Response?

The mortgage rate response is returned by the API to provide the latest available mortgage interest rate information, typically used for real estate and financial calculations. It includes the current rate, the type of mortgage, and the timestamp when the rate was retrieved.

## Usefulness

This response is useful for applications and users who need up-to-date mortgage rate data for loan calculations, affordability analysis, or investment modeling. By providing real-time rate information, it enables more accurate financial projections and decision-making in real estate transactions.

## Example Response

```json
{
  "current_rate": 6.56,
  "rate_type": "30-year fixed",
  "retrieved_at": "2025-08-28T19:47:47.469819"
}
```

## Response Fields

- **current_rate** (`number`): The current mortgage interest rate (annual percentage).
- **rate_type** (`string`): The type of mortgage rate (e.g., "30-year fixed", "15-year fixed").
- **retrieved_at** (`string`): The ISO 8601 timestamp when the rate was retrieved.

## Notes

- The rate may change frequently; always use the latest value for calculations.
- The `retrieved_at` field allows consumers to verify the freshness of the rate data.