---
name: financial-modelling
description: Build transparent revenue, unit-economics, scenario, and sensitivity models for a bridal beauty discovery and booking marketplace.
---

# Financial Modelling

## Model discipline

- Define the grain first: city, month, customer, booking, salon, artist, or cohort.
- Separate demand funnel, supply capacity, bookings, gross booking value, take rate, add-ons, refunds, payment costs, incentives, CAC, variable fulfilment/support costs, fixed costs, and contribution margin.
- State every input with unit, source or owner, date, and confidence. Never hardcode an unexplained number.
- Use formulas that can be audited. Show base, downside, and upside cases and run sensitivity on the few drivers that control the result.
- Distinguish accounting revenue from GMV and cash collections. Treat one-off setup cost, working capital, and timing separately.
- Test local marketplace liquidity and capacity constraints; do not assume bookings scale independently of supply.
- Use conservative retention and conversion assumptions until validated by cohort evidence.

## Minimum equations

`Bookings = qualified demand × conversion × confirmed supply-availability rate`

`GMV = bookings × average order value`

`Net revenue = GMV × take rate + subscriptions + lead fees + ancillary revenue - refunds/credits`

`Contribution margin = net revenue - payment costs - incentives - variable service/support costs`

`CAC payback months = CAC ÷ monthly contribution margin per retained customer`

## Output contract

Deliver: assumptions table; funnel and capacity bridge; revenue model; unit economics; cohort/retention logic; scenarios; sensitivity; break-even; risks; validation plan. Use `templates/financial-model-spec.md`. If producing an XLSX, apply the Anthropic XLSX conventions cited in `docs/source-inventory.md`.
