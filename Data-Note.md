# Week 2 Data Note

This data note documents the datasets collected and inspected for my healthcare accessibility project in Agege, Lagos State. The datasets were opened and inspected in QGIS before being used for further spatial analysis.

## 1. Agege Health Facilities

**Dataset:** GRID3 NGA - Health Facilities v2.0

**Source:** GRID3 Data Hub

**Source Link:** https://data.grid3.org/

**Number of Features:** 94

**Geometry Type:** Point

**Key Columns:**

- `facility_name` - name of the healthcare facility
- `state` - state where the facility is located
- `lga` - Local Government Area
- `ward` - ward where the facility is located
- `nhfr_uid` - National Health Facility Registry identifier
- `nhfr_facility_code` - health facility code

- **Data Quality Observations:**

Some records contain NULL or missing values in fields such as `nhfr_uid` and `nhfr_facility_code`. The inspected records contain useful information such as facility names, state, LGA and ward.


## 2. Agege Roads

**Dataset:** Agege Roads

**Source:** OpenStreetMap (OSM) via QuickOSM plugin in QGIS

**Source Link:** https://www.openstreetmap.org/

**Number of Features:** 1,305

**Geometry Type:** Line

**Key Columns:**
- `osm_id` - unique OpenStreetMap identifier for the road feature
- `osm_type` - type of OpenStreetMap object
- `highway` - classification of the road, such as residential, secondary, tertiary or unclassified
- `alt_name` - alternative name of the road, where available

- **Data Quality Observations:**
The `highway` field contains road classifications for the features. Several other fields, including `construction`, `footway`,`tactile_paving`, `incline`, `tunnel`, `covered` and `alt_name`, contain many NULL values. But a NULL value does not necessarily mean that the road itself is missing from the dataset.
