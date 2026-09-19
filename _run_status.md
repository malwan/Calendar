# Calendar Export — Last Run Status

- **Timestamp:** 2026-09-19 13:14:40
- **Sheets processed:** Jan-June 2026, July-Dec 2026
- **Status:** HEADER ANOMALIES — see _HEADER_ALERTS.txt

## Header resolution counts

| Status | Count |
|---|---|
| exact | 0 |
| alias (known variant) | 7 |
| fuzzy (similar, used as canonical) | 14 |
| unknown (SKIPPED) | 2 |
| missing (empty header) | 0 |

## Event counts

| Calendar | Events |
|---|---|
| Atzenhoefer | 196 |
| Brochtrup | 226 |
| Fabry | 217 |
| Hanrahan | 71 |
| Iqbal | 240 |
| Janus | 284 |
| Kashyap | 319 |
| Marmer | 215 |
| Martin | 270 |
| Maurer | 244 |
| Novak | 235 |
| Organ | 85 |
| Ortman | 240 |
| Povlich | 219 |
| Schaeve | 251 |
| **MasterSchedule** | 2158 |

Total leave/vacation events (across all sheets): 152
Total "-OFF- Long Call Weekend" events (across all sheets, deduped): 51

## Work header details

| Sheet | Col | Raw header | Canonical | Status | Notes |
|---|---|---|---|---|---|
| July-Dec 2026 | C | `MD*` | `Inpatient MD` | fuzzy | closest=`Inpatient MD` conf=0.80 |
| July-Dec 2026 | D | `APP 1 Inpatient *` | `Inpatient APP1` | fuzzy | closest=`Inpatient APP1` conf=0.90 |
| July-Dec 2026 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | fuzzy | closest=`Inpatient APP2 AM` conf=0.91 |
| July-Dec 2026 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | fuzzy | closest=`Inpatient APP2 PM` conf=0.91 |
| July-Dec 2026 | G | `Rotation*` | `Rotation` | fuzzy | closest=`Rotation` conf=0.94 |
| July-Dec 2026 | H | `AM*` | `CATH AM` | fuzzy | closest=`CATH AM` conf=0.80 |
| July-Dec 2026 | I | `PM*` | `CATH PM` | fuzzy | closest=`CATH PM` conf=0.80 |
| July-Dec 2026 | J | `Night Cath*` | `Night Cath` | fuzzy | closest=`Night Cath` conf=0.95 |
| July-Dec 2026 | L | `Diagnostic AM` | `Diagnostic AM` | alias | position drift; schema expected `Diagnostic PM` here |
| July-Dec 2026 | M | `Diagnostic PM` | `Diagnostic PM` | alias | position drift; schema expected `CMH Clinic APP1 AM` here |
| July-Dec 2026 | N | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 PM` conf=0.70 |
| July-Dec 2026 | O | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 AM` conf=0.70 |
| July-Dec 2026 | P | `APP 5 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 PM` conf=0.70 |
| July-Dec 2026 | Q | `APP 5 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`MD (AM) Available` conf=0.70 |
| July-Dec 2026 | R | `MD (AM) Available` | `MD (AM) Available` | alias | position drift; schema expected `MD (PM) - Stress Echo (Running Test)` here |
| July-Dec 2026 | S | `MD (PM) - Stress Echo (Running Test)` | `MD (PM) - Stress Echo (Running Test)` | alias | position drift; schema expected `BRK APP1 (0810-0850)` here |
| July-Dec 2026 | T | `APP 3 BRK Clinic AM` | `BRK APP1 (1230-1600)` | unknown | closest=`Inpatient APP2 AM` conf=0.56 |
| July-Dec 2026 | U | `APP 3 BRK Clinic PM` | `Cath APP AM` | unknown | closest=`Inpatient APP2 PM` conf=0.56 |
| July-Dec 2026 | V | `APP 7` | `APP 7` | alias | position drift; schema expected `Cath APP PM` here |
| July-Dec 2026 | W | `APP 6 Cath AM` | `CATH AM` | fuzzy | closest=`APP 7` conf=0.70 |
| July-Dec 2026 | X | `APP 6 Cath PM` | `CATH PM` | fuzzy | closest=`LCW` conf=0.70 |
| July-Dec 2026 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| July-Dec 2026 | Z | `Admin` | `Admin` | alias |  |

## Leave header details

| Sheet | Col | Raw | Expected | Status |
|---|---|---|---|---|
| Jan-June 2026 | Z | `MA` | `` | alias |
| Jan-June 2026 | AA | `NF` | `` | alias |
| Jan-June 2026 | AB | `MH` | `` | alias |
| July-Dec 2026 | AA | `MA` | `` | alias |
| July-Dec 2026 | AB | `NF` | `` | alias |
| July-Dec 2026 | AC | `MH` | `FI` | alias |
| July-Dec 2026 | AD | `FI` | `SJ` | alias |
| July-Dec 2026 | AE | `SJ` | `KK` | alias |
| July-Dec 2026 | AF | `KK` | `SM` | alias |
| July-Dec 2026 | AG | `SM` | `JAM` | alias |
| July-Dec 2026 | AH | `JAM` | `AB` | alias |
| July-Dec 2026 | AI | `AB` | `RM` | alias |
| July-Dec 2026 | AJ | `RM` | `BN` | alias |
| July-Dec 2026 | AK | `BN` | `EO` | alias |
| July-Dec 2026 | AL | `EO` | `KO` | alias |
| July-Dec 2026 | AM | `KO` | `MP` | alias |
| July-Dec 2026 | AN | `MP` | `JS` | alias |
| July-Dec 2026 | AO | `JS` | `` | alias |
