# Calendar Export — Last Run Status

- **Timestamp:** 2026-05-04 17:05:03
- **Sheets processed:** Jan-June 2026, July-Dec 2026
- **Status:** HEADER ANOMALIES — see _HEADER_ALERTS.txt

## Header resolution counts

| Status | Count |
|---|---|
| exact | 0 |
| alias (known variant) | 14 |
| fuzzy (similar, used as canonical) | 3 |
| unknown (SKIPPED) | 16 |
| missing (empty header) | 2 |

## Event counts

| Calendar | Events |
|---|---|
| Atzenhoefer | 118 |
| Brochtrup | 161 |
| Fabry | 135 |
| Hanrahan | 60 |
| Iqbal | 149 |
| Janus | 93 |
| Kashyap | 122 |
| Marmer | 130 |
| Martin | 93 |
| Maurer | 156 |
| Novak | 189 |
| Organ | 83 |
| Ortman | 188 |
| Povlich | 181 |
| Schaeve | 170 |
| **MasterSchedule** | 956 |

Total leave/vacation events (across all sheets): 95

## Work header details

| Sheet | Col | Raw header | Canonical | Status | Notes |
|---|---|---|---|---|---|
| Jan-June 2026 | F | `` | `` | missing |  |
| Jan-June 2026 | G | `Inpatient APP2 PM` | `Rotation` | unknown | closest=`Inpatient APP2 PM` conf=1.00 |
| Jan-June 2026 | H | `Rotation` | `CATH AM` | unknown | closest=`Rotation` conf=1.00 |
| Jan-June 2026 | I | `CATH AM` | `CATH PM` | fuzzy | closest=`CATH PM` conf=0.86 |
| Jan-June 2026 | J | `` | `` | missing |  |
| Jan-June 2026 | K | `CATH PM` | `Diagnostic AM` | unknown | closest=`CATH PM` conf=1.00 |
| Jan-June 2026 | L | `Night Cath` | `Diagnostic PM` | unknown | closest=`Night Cath` conf=1.00 |
| Jan-June 2026 | M | `Diagnostic AM` | `CMH Clinic APP1 AM` | unknown | closest=`Diagnostic AM` conf=1.00 |
| Jan-June 2026 | N | `Diagnostic PM` | `CMH Clinic APP1 PM` | unknown | closest=`Diagnostic PM` conf=1.00 |
| Jan-June 2026 | O | `CMH Clinic APP1 AM` | `CMH Clinic APP2 AM` | fuzzy | closest=`CMH Clinic APP2 AM` conf=0.94 |
| Jan-June 2026 | P | `CMH Clinic APP1 PM` | `CMH Clinic APP2 PM` | fuzzy | closest=`CMH Clinic APP2 PM` conf=0.94 |
| Jan-June 2026 | Q | `CMH Clinic APP2 AM` | `MD (AM) Available` | unknown | closest=`CMH Clinic APP2 AM` conf=1.00 |
| Jan-June 2026 | R | `CMH Clinic APP2 PM` | `MD (PM) - Stress Echo (Running Test)` | unknown | closest=`CMH Clinic APP2 PM` conf=1.00 |
| Jan-June 2026 | S | `MD (AM) Available` | `BRK APP1 (0810-0850)` | unknown | closest=`MD (AM) Available` conf=1.00 |
| Jan-June 2026 | T | `MD (PM) - Stress Echo (Running Test)` | `BRK APP1 (1230-1600)` | unknown | closest=`MD (PM) - Stress Echo (Running Test)` conf=1.00 |
| Jan-June 2026 | U | `BRK APP1  (0810-0850)` | `Cath APP AM` | unknown | closest=`BRK APP1 (0810-0850)` conf=1.00 |
| Jan-June 2026 | V | `BRK APP1  (1230-1600)` | `Cath APP PM` | unknown | closest=`BRK APP1 (1230-1600)` conf=1.00 |
| Jan-June 2026 | W | `Cath APP AM` | `APP 7` | unknown | closest=`Cath APP AM` conf=1.00 |
| Jan-June 2026 | X | `Cath APP PM` | `LCW` | unknown | closest=`Cath APP PM` conf=1.00 |
| Jan-June 2026 | Y | `APP 7` | `Admin` | unknown | closest=`APP 7` conf=1.00 |
| Jan-June 2026 | Z | `LCW` | `MA` | unknown | closest=`LCW` conf=1.00 |
| July-Dec 2026 | C | `MD` | `Inpatient MD` | alias |  |
| July-Dec 2026 | D | `APP Inpatient 1` | `Inpatient APP1` | alias |  |
| July-Dec 2026 | E | `APP Inpatient 2 AM` | `Inpatient APP2 AM` | alias |  |
| July-Dec 2026 | F | `APP Inpatient 2 PM` | `Inpatient APP2 PM` | alias |  |
| July-Dec 2026 | H | `AM` | `CATH AM` | alias |  |
| July-Dec 2026 | I | `PM` | `CATH PM` | alias |  |
| July-Dec 2026 | M | `CMH Clinic APP 1 AM` | `CMH Clinic APP1 AM` | alias |  |
| July-Dec 2026 | N | `CMH Clinic APP 1 PM` | `CMH Clinic APP1 PM` | alias |  |
| July-Dec 2026 | O | `CMH Clinic APP 2 AM` | `CMH Clinic APP2 AM` | alias |  |
| July-Dec 2026 | P | `CMH Clinic APP 2 PM` | `CMH Clinic APP2 PM` | alias |  |
| July-Dec 2026 | S | `BRK APP  (0810-0850)` | `BRK APP1 (0810-0850)` | alias |  |
| July-Dec 2026 | T | `BRK APP  (1230-1600)` | `BRK APP1 (1230-1600)` | alias |  |
| July-Dec 2026 | U | `Cath AM` | `Cath APP AM` | alias |  |
| July-Dec 2026 | V | `Cath PM` | `Cath APP PM` | alias |  |

## Leave header details

| Sheet | Col | Raw | Expected | Status |
|---|---|---|---|---|
| Jan-June 2026 | AC | `NF` | `FI` | alias |
| Jan-June 2026 | AD | `MH` | `SJ` | alias |
| Jan-June 2026 | AE | `FI` | `KK` | alias |
| Jan-June 2026 | AF | `SJ` | `SM` | alias |
| Jan-June 2026 | AG | `KK` | `JAM` | alias |
| Jan-June 2026 | AH | `SM` | `AB` | alias |
| Jan-June 2026 | AI | `JAM` | `RM` | alias |
| Jan-June 2026 | AJ | `AB` | `BN` | alias |
| Jan-June 2026 | AK | `RM` | `EO` | alias |
| Jan-June 2026 | AL | `BN` | `KO` | alias |
| Jan-June 2026 | AM | `EO` | `MP` | alias |
| Jan-June 2026 | AN | `KO` | `JS` | alias |
| Jan-June 2026 | AO | `MP` | `` | alias |
| Jan-June 2026 | AP | `JS` | `` | alias |
