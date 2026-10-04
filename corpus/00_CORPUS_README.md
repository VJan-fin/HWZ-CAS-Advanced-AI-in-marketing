# Züricom RAG Workshop Corpus

## Purpose

A fictional Swiss telecommunications marketing knowledge base designed for a hands-on RAG workshop. The documents are intentionally heterogeneous and include realistic product facts, policy language, marketing guidance, customer research and dated competitor snapshots.

## Documents

| File | Role |
|---|---|
| 01 | Current Unlimited Plan product facts |
| 02 | Current roaming policy |
| 03 | Travel Add-on product note |
| 04 | Family product information |
| 05 | Frequent Traveler persona |
| 06 | Family persona |
| 07 | Brand voice and positioning |
| 08 | Email channel guidance |
| 09 | LinkedIn channel guidance |
| 10 | Approved claims / restricted claims |
| 11 | Customer research on travel behaviour |
| 12 | Customer research on switching and price sensitivity |
| 13 | HelvetiTel 2025 archived competitor snapshot |
| 14 | HelvetiTel 2026 current competitor snapshot |
| 15 | Alpinetel 2026 current competitor snapshot |

## Deliberate design features

- The corpus contains **current and archived information**.
- Product/policy documents are more authoritative than customer research for factual product claims.
- Marketing guidance contains legitimate constraints that can conflict with a generic “write compelling copy” prompt.
- Several documents are relevant to a single query, so `top_k` matters.
- Some documents contain distractor information that can be retrieved when `top_k` is too high.
- The two HelvetiTel snapshots intentionally contain **conflicting prices** (CHF 49 in 2025 vs CHF 59 in 2026).
- Geographic wording is intentionally precise: EU countries are not treated as synonymous with “Europe”.
