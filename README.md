# Insurance Product Rules Testing and Premium Validation

## Project Overview

This Excel project simulates the process of testing an auto insurance rating system.

I created a synthetic rate book with the rules and factors used to calculate premiums. The rate book includes:

- Coverage base rates
- Driver age
- Years of driving experience
- At-fault accidents
- Usage-based insurance results
- Annual mileage
- City and ZIP code
- Vehicle price
- Exotic vehicle status
- Difficult-to-replace parts
- Vehicle theft rates
- Advanced safety features
- Deductible selections
- Coverage limits
- Good Student discount
- Good Driver discount
- Multi-Policy discount
- Loyal Customer discount
- Organization discount
- An effective-date rate change

I then created 1,000 synthetic policies with different combinations of these characteristics.

For each policy, the workbook calculates an expected premium using the rate book and compares it with a simulated system-generated premium. Each test case is marked as PASS or FAIL based on the difference between the two premiums.

Failed cases are grouped by their likely cause and added to an issue log with a recommended action.

## Why I Built This Project

I originally created this project while preparing for an Actuarial Technician interview at AAA.

The position involved responsibilities such as reviewing rating rules, testing system calculations, validating premiums, and documenting issues. I wanted to better understand that type of work, so I created a project that allowed me to practice the process from beginning to end.

I later made the project more general so it could also show skills that apply to actuarial analyst, actuarial technician, insurance systems, quality assurance, and illustrations systems analyst positions.

## Main Question

Does the simulated rating system apply the correct base rate, rating factor, discount, coverage rule, and effective-date change to each policy?

## How the Project Works

1. The **Rate Book** stores the base rates, rating factors, discounts, and coverage rules.
2. The **Test Cases** tab contains 1,000 synthetic policy scenarios.
3. The policies are carried into the **Premium Validation** tab.
4. The applicable base rate and rating factors are retrieved for each policy.
5. An expected premium is calculated independently.
6. The expected premium is compared with the simulated system-generated premium.
7. Each policy is marked as PASS or FAIL.
8. Failed cases are assigned a likely cause.
9. The results are summarized in the **QA Summary**.
10. All failed cases are documented in the **Issue Log**.

## Premium Calculation

The expected premium is calculated by starting with the coverage base rate and multiplying it by the factors that apply to the policy.

In simplified form:

```text
Expected Premium =
Base Rate
× Driver Factors
× Driving History Factors
× Mileage Factor
× Location Factor
× Vehicle Factors
× Coverage Factors
× Discount Factors
× Rate Change Factor
