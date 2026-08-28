# Calendar Export — Last Run Status

- **Timestamp:** 2026-08-28 17:05:04
- **Sheets processed:** Jan-June 2026, July-Dec 2026
- **Status:** HEADER ANOMALIES — see _HEADER_ALERTS.txt

## Header resolution counts

| Status | Count |
|---|---|
| exact | 0 |
| alias (known variant) | 4 |
| fuzzy (similar, used as canonical) | 9 |
| unknown (SKIPPED) | 2 |
| missing (empty header) | 0 |

## Event counts

| Calendar | Events |
|---|---|
| Atzenhoefer | 187 |
| Brochtrup | 227 |
| Fabry | 207 |
| Hanrahan | 67 |
| Iqbal | 231 |
| Janus | 280 |
| Kashyap | 316 |
| Marmer | 205 |
| Martin | 266 |
| Maurer | 244 |
| Novak | 235 |
| Organ | 85 |
| Ortman | 240 |
| Povlich | 219 |
| Schaeve | 251 |
| **MasterSchedule** | 2159 |

Total leave/vacation events (across all sheets): 150

## Work header details

| Sheet | Col | Raw header | Canonical | Status | Notes |
|---|---|---|---|---|---|
| July-Dec 2026 | C | `MD` | `Inpatient MD` | alias |  |
| July-Dec 2026 | D | `APP 1 Inpatient` | `Inpatient APP1` | fuzzy | closest=`Inpatient APP1` conf=0.97 |
| July-Dec 2026 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | fuzzy | closest=`Inpatient APP2 AM` conf=0.91 |
| July-Dec 2026 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | fuzzy | closest=`Inpatient APP2 PM` conf=0.91 |
| July-Dec 2026 | H | `AM` | `CATH AM` | alias |  |
| July-Dec 2026 | I | `PM` | `CATH PM` | alias |  |
| July-Dec 2026 | M | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 AM` conf=0.70 |
| July-Dec 2026 | N | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 PM` conf=0.70 |
| July-Dec 2026 | O | `APP 5 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 AM` conf=0.70 |
| July-Dec 2026 | P | `APP 5 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 PM` conf=0.70 |
| July-Dec 2026 | S | `APP 3 BRK Clinic AM` | `BRK APP1 (0810-0850)` | unknown | closest=`Inpatient APP2 AM` conf=0.56 |
| July-Dec 2026 | T | `APP 3 BRK Clinic PM` | `BRK APP1 (1230-1600)` | unknown | closest=`Inpatient APP2 PM` conf=0.56 |
| July-Dec 2026 | U | `APP 7` | `APP 7` | alias | position drift; schema expected `Cath APP AM` here |
| July-Dec 2026 | V | `APP 6 Cath AM` | `CATH AM` | fuzzy | closest=`Cath APP PM` conf=0.70 |
| July-Dec 2026 | W | `APP 6 Cath PM` | `CATH PM` | fuzzy | closest=`APP 7` conf=0.70 |

## Leave header details

| Sheet | Col | Raw | Expected | Status |
|---|---|---|---|---|
| Jan-June 2026 | Z | `MA` | `` | alias |
| Jan-June 2026 | AA | `NF` | `` | alias |
| Jan-June 2026 | AB | `MH` | `` | alias |
| July-Dec 2026 | Z | `MA` | `` | alias |
| July-Dec 2026 | AA | `NF` | `` | alias |
| July-Dec 2026 | AB | `MH` | `` | alias |
