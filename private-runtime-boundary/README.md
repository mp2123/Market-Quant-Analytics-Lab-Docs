# Private Runtime Boundary

The production/non-ML QuantStrat runtime is private and should stay private.

## Why It Stays Private

- It may contain operational runtime state.
- It may include broker/API integration surfaces.
- It may contain private configuration, token paths, monitor payloads, or account-specific assumptions.
- Public language around production trading systems carries higher overclaim and privacy risk.

## How It Can Be Mentioned Publicly

It can be referenced only as private source lineage behind the safer public research and documentation layers.

Public-facing language should say:

> Private production/runtime experiments remain internal. Public docs focus on market-data analytics, dashboard review, research validation, and privacy-safe architecture.

Do not link the private runtime repo publicly.
