---
name: calculate-tax
description: "Calculate a client invoice that leaves the requested take-home amount after tax. Use for requests such as 'calculate tax 60000', 'tax calculation', or 'how much should I invoice the client'; the default tax is 7% of the invoice total."
---

# Calculate Tax

The user receives a client payment and pays 7% tax on the entire invoice. In a short request such as “calculate tax 60000,” the number means the desired take-home amount, and the task is to calculate the client invoice. Do not ask what the amount means or which rate to use for this request: those defaults are already agreed.

- The default rate is 7%, and the default currency is Russian rubles (RUB). Explicit parameters in the current request take precedence.
- Invoice = desired take-home amount / (1 − rate / 100). Simply adding 7% is incorrect.
- Round the invoice up to the nearest kopeck (0.01 RUB) so the amount left after tax is at least the requested amount. Calculate tax from the rounded invoice and round it to the nearest kopeck using ordinary monetary rounding (half up). Verify the remainder as invoice minus tax; use decimal arithmetic or exact fractions.
- If the user explicitly supplies an invoice amount that has already been issued, calculate tax and the remainder directly. If they request whole rubles, round the invoice up to the next whole ruble.
- Respond briefly in Russian: invoice amount first, then tax and take-home amount. Do not add questions, legal commentary, or searches for current tax rates: the rate here is a supplied arithmetic parameter.

Example, shown in English: “calculate tax 60000” → “Invoice **RUB 64,516.13**. Tax at 7%: **RUB 4,516.13**. Take-home amount: **RUB 60,000**.”
