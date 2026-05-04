# LA Crime Data Analysis using Elasticsearch & Kibana ML

**Course:** CIS3200-01 — Big Data Technologies  
**Instructor:** Prof. Jongwook Woo  
**Authors:** Daniel Ramirez, Arlyn Garcia-Martinez, Matthew Mendoza, Natalie Sanchez  
**Date: May 3 2026

## Dataset
- **Source:** City of LA Open Data Portal
- **Link:** https://data.lacity.org/resource/2nrs-mtv8.csv
- **Size:** 25.8 MB — 90,000 rows (2023 LAPD Crime Data)

## Elasticsearch Endpoint
https://824e614adae3444bb290f09002a9403b.us-central1.gcp.cloud.es.io:443

## Kibana Dashboard
[Paste your dashboard share link here]

## ML Results
| Metric | Test | Train |
|--------|------|-------|
| MSE | 183 | 173 |
| RMSE | ~13.5 | ~13.2 |
| R-squared | 0.623 | 0.643 |

**Top Influencers:**
1. vict_descent
2. crm_cd_desc
3. premis_desc
4. time_occ
5. area_name

## How to Reproduce
1. Download dataset using Socrata API (see tutorial)
2. Upload CSV to Elasticsearch via Kibana Data Visualizer
3. Create geo_point mapping using reindex script
4. Build dashboard with 4 visualizations
5. Run regression ML job to predict victim age

## References
- https://data.lacity.org/Public-Safety/Crime-Data-from-2020-to-2024/2nrs-mtv8
- https://www.elastic.co/guide/en/elasticsearch/reference/current/index.html
- https://www.elastic.co/guide/en/kibana/current/xpack-ml.html
