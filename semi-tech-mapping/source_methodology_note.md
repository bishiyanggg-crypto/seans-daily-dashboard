# Semi Tech Industry Mapping - Source and Methodology Note

Data cut-off: 2026-06-18

## Scope

Global listed-company universe across semiconductor design, manufacturing, equipment, materials, OSAT, substrate/PCB, optical, EMS/ODM, systems, and adjacent industrial enablers. A-share, HK-listed, Taiwan, Japan, Korea, Europe, US and ASEAN names are included with a bias toward leaders and investable public comparables.

## Priority system

- Core: first-pass deep-dive list; should receive CIQ refresh and company-specific follow-up.
- Important: important regional/segment comparable or value-chain marker.
- Watchlist: long-tail, event-driven, adjacency, or listing/status needs further verification.

## Market-data policy

The fields market_cap_usd, fy_revenue_usd, gross_margin, ev_sales, pe, and consensus_revenue_growth are included in the CSV/JSON schema. In this first version they are intentionally marked needs_CIQ unless refreshed from a controlled data export. This avoids mixing stale or unsourced valuation data into a publication-style comp table.

## Debate map

The Variant Perception / Key Debates layer is designed as the bridge from industry taxonomy to investment work. It frames consensus, variant questions, winners/risks, monitoring signals and falsifiers across AI capex, ASIC vs GPU, HBM, advanced packaging, China localization, WFE, optical, AI infrastructure and auto/industrial cycles.

## Counts

- Total companies: 307
- Priority: {'Core': 139, 'Watchlist': 83, 'Important': 85}
- Segment playbooks: 16
- Segment value-pool scorecards: 16
- Segment cycle guides: 16
- Demand cycle guides: 6
- Supply-chain relationship edges: 15
- End-market crosswalks: 6
- Regional supply-chain lenses: 7
- Coverage cockpit segment summaries: 16
- Core coverage wave plan rows: 139
- End-market exposure matrix rows: 16
- Segment scenario variable rows: 16
- Official market context rows: 6
- Data governance layers: 4
- Segment KPI monitor entries: 16
- Model architecture modules: 6
- Analyst glossary terms: 20
- Variant debate map items: 9
- Coverage roadmap phases: 5
- CIQ refresh fields: 9
- Core CIQ refresh template rows: 139
- Source ledger entries: 10
- Segment counts:
  - Adjacent Infra / Industrial Enablers: 28
  - Analog / Power / Mixed Signal: 24
  - Compute / AI / Logic Chips: 13
  - EDA / IP / Design Enablement: 13
  - EMS / ODM / Systems: 18
  - Foundry / IDM Manufacturing: 11
  - Materials / Wafers / Chemicals / Gases: 33
  - Memory / Storage Semiconductors: 14
  - Mobile / RF / Connectivity: 26
  - Networking Silicon / SerDes / Data Movement: 11
  - OSAT / Advanced Packaging: 21
  - Optical / Photonics: 14
  - Passives / Components / Sensors: 12
  - Process Control / Test / Metrology: 20
  - Semicap Equipment: 27
  - Substrate / PCB / Interconnect: 22

## Suggested next CIQ merge

1. Use semi_ciq_refresh_template_core.csv as the Core-company export/import shell.
2. Use semi_core_coverage_workplan.csv as the Core-company research queue.
3. Export CIQ fields keyed by primary ticker: market cap, enterprise value, FY revenue, gross margin, EV/Sales, P/E, consensus FY1/FY2 revenue growth, country, exchange, market cap currency.
4. Preserve this file's segment_id and priority columns as the taxonomy source of truth.
5. Merge on ticker after manually resolving dual listings and post-spin / pending-acquisition rows.
6. Refresh Core first, then Important, then Watchlist.

## Public source lanes

- SIA - How are Semiconductors Made?: High-level value-chain sequence: R&D, design, front-end manufacturing, back-end manufacturing, board/system assembly. (https://www.semiconductors.org/semiconductors-101/how-are-semiconductors-made/)
- SIA - Market Data / WSTS overview: WSTS data scope, product categories, monthly shipment data, units, ASPs, regional and product breakouts. (https://www.semiconductors.org/data-resources/market-data/)
- SIA/WSTS - April 2026 global semiconductor sales release: Latest public industry cycle snapshot: April 2026 global sales, regional growth and Spring 2026 WSTS forecast context. (https://www.semiconductors.org/global-semiconductor-sales-increase-11-month-to-month-in-april/)
- SIA / Deloitte - Powering AI data-center semiconductor stack: AI rack semiconductor content, AI data-center capex framing and cross-stack chip demand mapping. (https://www.semiconductors.org/new-report-finds-semiconductors-account-for-95-of-an-ai-data-server-racks-value-encompassing-the-full-stack-of-chip-technologies/)
- WSTS homepage and forecast releases: Industry shipment data cadence and semiconductor market-monitoring framework. (https://www.wsts.org/)
- SIA - 2025 State of the U.S. Semiconductor Industry: Strategic context on US semiconductor leadership, manufacturing capacity and policy-driven supply-chain localization. (https://www.semiconductors.org/2025-state-of-the-u-s-semiconductor-industry/)
- SEMI market data / industry reports: WFE, materials, packaging, fab capacity and equipment-market framing. (https://www.semi.org/en/market-data)
- SEMI - 2025 worldwide silicon wafer shipments and revenue: Wafer-shipment cycle context, AI-driven advanced wafer demand and mature-node stabilization signals. (https://www.semi.org/en/semi-press-release/semi-reports-2025-annual-worldwide-silicon-wafer-shipments-and-revenue-results)
- Company filings and investor relations: Company business descriptions, segment exposure, products, customer concentration and listing status. (Issuer IR / annual reports / 10-K / 20-F / exchange filings)
- CIQ export refresh: Market cap, EV, FY revenue, gross margin, EV/Sales, P/E, consensus growth, identifiers and ownership. (User-provided CIQ account/export)

## Known verification items

- Some post-spin or deal-sensitive rows require refresh before publication-quality use, including Sandisk, Qnity Electronics, Kioxia, Shinko Electric, Juniper, Alphawave and similar event-driven cases.
- Dual listings are represented in a single economic-entity row where appropriate. For valuation work, choose one primary tradable line and keep ADR/local-line mapping separately.
- Private but strategically important entities are not included in the listed-company table unless embedded in public parents; they should appear in narrative chain maps if a future version adds non-listed ecosystem nodes.