# Calendar Export — Last Run Status

- **Timestamp:** 2026-06-14 17:05:02
- **Sheets processed:** Jan-June 2026, July-Dec 2026
- **Status:** Clean

## Header resolution counts

| Status | Count |
|---|---|
| exact | 0 |
| alias (known variant) | 34 |
| fuzzy (similar, used as canonical) | 0 |
| unknown (SKIPPED) | 0 |
| missing (empty header) | 0 |

## Event counts

| Calendar | Events |
|---|---|
| Atzenhoefer | 184 |
| Brochtrup | 264 |
| Fabry | 206 |
| Hanrahan | 69 |
| Iqbal | 228 |
| Janus | 177 |
| Kashyap | 217 |
| Marmer | 199 |
| Martin | 171 |
| Maurer | 275 |
| Novak | 269 |
| Organ | 102 |
| Ortman | 285 |
| Povlich | 273 |
| Schaeve | 282 |
| **MasterSchedule** | 1633 |

Total leave/vacation events (across all sheets): 130

## Work header details

| Sheet | Col | Raw header | Canonical | Status | Notes |
|---|---|---|---|---|---|
| Jan-June 2026 | G | `Inpatient APP2 PM` | `Inpatient APP2 PM` | alias | position drift; schema expected `Rotation` here |
| Jan-June 2026 | H | `Rotation` | `Rotation` | alias | position drift; schema expected `CATH AM` here |
| Jan-June 2026 | I | `CATH AM` | `CATH AM` | alias | position drift; schema expected `CATH PM` here |
| Jan-June 2026 | L | `CATH PM` | `CATH PM` | alias | position drift; schema expected `Diagnostic PM` here |
| Jan-June 2026 | M | `Night Cath` | `Night Cath` | alias | position drift; schema expected `CMH Clinic APP1 AM` here |
| Jan-June 2026 | N | `Diagnostic AM` | `Diagnostic AM` | alias | position drift; schema expected `CMH Clinic APP1 PM` here |
| Jan-June 2026 | O | `Diagnostic PM` | `Diagnostic PM` | alias | position drift; schema expected `CMH Clinic APP2 AM` here |
| Jan-June 2026 | P | `CMH Clinic APP1 AM` | `CMH Clinic APP1 AM` | alias | position drift; schema expected `CMH Clinic APP2 PM` here |
| Jan-June 2026 | Q | `CMH Clinic APP1 PM` | `CMH Clinic APP1 PM` | alias | position drift; schema expected `MD (AM) Available` here |
| Jan-June 2026 | R | `CMH Clinic APP2 AM` | `CMH Clinic APP2 AM` | alias | position drift; schema expected `MD (PM) - Stress Echo (Running Test)` here |
| Jan-June 2026 | S | `CMH Clinic APP2 PM` | `CMH Clinic APP2 PM` | alias | position drift; schema expected `BRK APP1 (0810-0850)` here |
| Jan-June 2026 | T | `MD (AM) Available` | `MD (AM) Available` | alias | position drift; schema expected `BRK APP1 (1230-1600)` here |
| Jan-June 2026 | U | `MD (PM) - Stress Echo (Running Test)` | `MD (PM) - Stress Echo (Running Test)` | alias | position drift; schema expected `Cath APP AM` here |
| Jan-June 2026 | V | `BRK APP1  (0810-0850)` | `BRK APP1 (0810-0850)` | alias | position drift; schema expected `Cath APP PM` here |
| Jan-June 2026 | W | `BRK APP1  (1230-1600)` | `BRK APP1 (1230-1600)` | alias | position drift; schema expected `APP 7` here |
| Jan-June 2026 | X | `Cath APP AM` | `Cath APP AM` | alias | position drift; schema expected `LCW` here |
| Jan-June 2026 | Y | `Cath APP PM` | `Cath APP PM` | alias | position drift; schema expected `Admin` here |
| Jan-June 2026 | Z | `APP 7` | `APP 7` | alias |  |
| Jan-June 2026 | AA | `LCW` | `LCW` | alias |  |
| Jan-June 2026 | AB | `Admin` | `Admin` | alias |  |
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
| Jan-June 2026 | AC | `MA` | `FI` | alias |
| Jan-June 2026 | AD | `NF` | `SJ` | alias |
| Jan-June 2026 | AE | `MH` | `KK` | alias |
| Jan-June 2026 | AF | `FI` | `SM` | alias |
| Jan-June 2026 | AG | `SJ` | `JAM` | alias |
| Jan-June 2026 | AH | `KK` | `AB` | alias |
| Jan-June 2026 | AI | `SM` | `RM` | alias |
| Jan-June 2026 | AJ | `JAM` | `BN` | alias |
| Jan-June 2026 | AK | `AB` | `EO` | alias |
| Jan-June 2026 | AL | `RM` | `KO` | alias |
| Jan-June 2026 | AM | `BN` | `MP` | alias |
| Jan-June 2026 | AN | `EO` | `JS` | alias |
| Jan-June 2026 | AO | `KO` | `` | alias |
| Jan-June 2026 | AP | `MP` | `` | alias |
| Jan-June 2026 | AQ | `JS` | `` | alias |
| July-Dec 2026 | Z | `MA` | `` | alias |
| July-Dec 2026 | AA | `NF` | `` | alias |
| July-Dec 2026 | AB | `MH` | `` | alias |
