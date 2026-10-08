# Calendar Export — Last Run Status

- **Timestamp:** 2026-10-08 17:05:05
- **Sheets processed:** July-Dec 2026, Jan-June 2027, July-Dec 2027
- **Status:** HEADER ANOMALIES — see _HEADER_ALERTS.txt

## Header resolution counts

| Status | Count |
|---|---|
| exact | 0 |
| alias (known variant) | 16 |
| fuzzy (similar, used as canonical) | 32 |
| unknown (SKIPPED) | 7 |
| missing (empty header) | 0 |

## Event counts

| Calendar | Events |
|---|---|
| Atzenhoefer | 271 |
| Brochtrup | 207 |
| Fabry | 272 |
| Hanrahan | 244 |
| Iqbal | 320 |
| Janus | 306 |
| Kashyap | 340 |
| Kohl | 121 |
| Marin | 1 |
| Marmer | 276 |
| Martin | 277 |
| Mauer | 2 |
| Maurer | 206 |
| Novak | 224 |
| Organ | 64 |
| Ortman | 210 |
| Povlich | 206 |
| Schaeve | 205 |
| **MasterSchedule** | 2758 |

Total leave/vacation events (across all sheets): 120
Total "-OFF- Long Call Weekend" events (across all sheets, deduped): 78

## Dynamic provider roster (provider_registry.json)

Discovered automatically from the schedule; treated like any
hardcoded provider (own .ics + master inclusion).

| Provider | Leave initials | First seen | First context |
|---|---|---|---|
| Kohl | *(not linked)* | 2027-01-04 | Jan-June 2027 / CMH Clinic APP1 AM |
| Marin | *(not linked)* | 2027-07-01 | July-Dec 2027 / CATH PM |
| Mauer | *(not linked)* | 2027-02-18 | Jan-June 2027 / APP 7 |

## Work header details

| Sheet | Col | Raw header | Canonical | Status | Notes |
|---|---|---|---|---|---|
| July-Dec 2026 | C | `MD*` | `Inpatient MD` | fuzzy | closest=`Inpatient MD` conf=0.80 |
| July-Dec 2026 | D | `APP 1 Inpatient *` | `Inpatient APP1` | fuzzy | closest=`Inpatient APP1` conf=0.90 |
| July-Dec 2026 | E | `Rotation*` | `Rotation` | fuzzy | closest=`Inpatient APP2 AM` conf=0.94 |
| July-Dec 2026 | F | `AM*` | `CATH AM` | fuzzy | closest=`Inpatient APP2 PM` conf=0.80 |
| July-Dec 2026 | G | `PM*` | `CATH PM` | fuzzy | closest=`Rotation` conf=0.80 |
| July-Dec 2026 | H | `Night Cath*` | `Night Cath` | fuzzy | closest=`CATH AM` conf=0.95 |
| July-Dec 2026 | J | `Diagnostic AM` | `Diagnostic AM` | alias | position drift; schema expected `Night Cath` here |
| July-Dec 2026 | K | `Diagnostic PM` | `Diagnostic PM` | alias | position drift; schema expected `Diagnostic AM` here |
| July-Dec 2026 | L | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`Diagnostic PM` conf=0.70 |
| July-Dec 2026 | M | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 AM` conf=0.70 |
| July-Dec 2026 | N | `APP 5 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 PM` conf=0.70 |
| July-Dec 2026 | O | `APP 5 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 AM` conf=0.70 |
| July-Dec 2026 | P | `MD (AM) Available` | `MD (AM) Available` | alias | position drift; schema expected `CMH Clinic APP2 PM` here |
| July-Dec 2026 | Q | `MD (PM) - Stress Echo (Running Test)` | `MD (PM) - Stress Echo (Running Test)` | alias | position drift; schema expected `MD (AM) Available` here |
| July-Dec 2026 | R | `APP 3 BRK Clinic AM` | `MD (PM) - Stress Echo (Running Test)` | unknown | closest=`Inpatient APP2 AM` conf=0.56 |
| July-Dec 2026 | S | `APP 3 BRK Clinic PM` | `BRK APP1 (0810-0850)` | unknown | closest=`Inpatient APP2 PM` conf=0.56 |
| July-Dec 2026 | T | `APP 7` | `APP 7` | alias | position drift; schema expected `BRK APP1 (1230-1600)` here |
| July-Dec 2026 | U | `APP 6 Cath AM*` | `CATH AM` | fuzzy | closest=`Cath APP AM` conf=0.67 |
| July-Dec 2026 | V | `APP 6 Cath PM*` | `CATH PM` | fuzzy | closest=`Cath APP PM` conf=0.67 |
| July-Dec 2026 | W | `LCW` | `LCW` | alias | position drift; schema expected `APP 7` here |
| July-Dec 2026 | X | `Admin` | `Admin` | alias | position drift; schema expected `LCW` here |
| Jan-June 2027 | C | `MD` | `Inpatient MD` | alias |  |
| Jan-June 2027 | D | `APP 1 Inpatient` | `Inpatient APP1` | fuzzy | closest=`Inpatient APP1` conf=0.97 |
| Jan-June 2027 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | fuzzy | closest=`Inpatient APP2 AM` conf=0.91 |
| Jan-June 2027 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | fuzzy | closest=`Inpatient APP2 PM` conf=0.91 |
| Jan-June 2027 | H | `AM` | `CATH AM` | alias |  |
| Jan-June 2027 | I | `PM` | `CATH PM` | alias |  |
| Jan-June 2027 | M | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 AM` conf=0.70 |
| Jan-June 2027 | N | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 PM` conf=0.70 |
| Jan-June 2027 | O | `APP 5 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 AM` conf=0.70 |
| Jan-June 2027 | P | `APP 5 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 PM` conf=0.70 |
| Jan-June 2027 | S | `APP 3 BRK Clinic` | `BRK APP1 (0810-0850)` | unknown | closest=`Inpatient APP1` conf=0.47 |
| Jan-June 2027 | T | `APP 3 BRK Clinic` | `BRK APP1 (1230-1600)` | unknown | closest=`Inpatient APP1` conf=0.47 |
| Jan-June 2027 | U | `APP 7         AM` | `APP 7` | fuzzy | closest=`Cath APP AM` conf=0.77 |
| Jan-June 2027 | V | `APP 7         PM` | `APP 7` | fuzzy | closest=`Cath APP PM` conf=0.77 |
| Jan-June 2027 | W | `Cath APP 6 AM` | `Cath APP AM` | fuzzy | closest=`APP 7` conf=0.92 |
| Jan-June 2027 | X | `Cath APP 6 PM` | `Cath APP PM` | fuzzy | closest=`LCW` conf=0.92 |
| Jan-June 2027 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| Jan-June 2027 | Z | `Admin` | `Admin` | alias |  |
| July-Dec 2027 | C | `MD` | `Inpatient MD` | alias |  |
| July-Dec 2027 | D | `APP 1 Inpatient` | `Inpatient APP1` | fuzzy | closest=`Inpatient APP1` conf=0.97 |
| July-Dec 2027 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | fuzzy | closest=`Inpatient APP2 AM` conf=0.91 |
| July-Dec 2027 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | fuzzy | closest=`Inpatient APP2 PM` conf=0.91 |
| July-Dec 2027 | H | `AM` | `CATH AM` | alias |  |
| July-Dec 2027 | I | `PM` | `CATH PM` | alias |  |
| July-Dec 2027 | K | `0` | `Diagnostic AM` | unknown | closest=`BRK APP1 (0810-0850)` conf=0.10 |
| July-Dec 2027 | M | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 AM` conf=0.70 |
| July-Dec 2027 | N | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP1 PM` conf=0.70 |
| July-Dec 2027 | O | `APP 5 CMH Clinic AM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 AM` conf=0.70 |
| July-Dec 2027 | P | `APP 5 CMH Clinic PM` | `CMH Clinic APP1 AM` | fuzzy | closest=`CMH Clinic APP2 PM` conf=0.70 |
| July-Dec 2027 | S | `APP 3 BRK Clinic` | `BRK APP1 (0810-0850)` | unknown | closest=`Inpatient APP1` conf=0.47 |
| July-Dec 2027 | T | `APP 3 BRK Clinic` | `BRK APP1 (1230-1600)` | unknown | closest=`Inpatient APP1` conf=0.47 |
| July-Dec 2027 | U | `APP 7` | `APP 7` | alias | position drift; schema expected `Cath APP AM` here |
| July-Dec 2027 | V | `Cath APP 6 AM` | `Cath APP AM` | fuzzy | closest=`Cath APP PM` conf=0.92 |
| July-Dec 2027 | W | `Cath APP 6 PM` | `Cath APP PM` | fuzzy | closest=`APP 7` conf=0.92 |

## Leave header details

| Sheet | Col | Raw | Expected | Status |
|---|---|---|---|---|
| July-Dec 2026 | Y | `MA` | `` | alias |
| July-Dec 2026 | Z | `NF` | `` | alias |
| July-Dec 2026 | AA | `MH` | `` | alias |
| July-Dec 2026 | AB | `FI` | `` | alias |
| July-Dec 2026 | AC | `SJ` | `FI` | alias |
| July-Dec 2026 | AD | `KK` | `SJ` | alias |
| July-Dec 2026 | AE | `SM` | `KK` | alias |
| July-Dec 2026 | AF | `JAM` | `SM` | alias |
| July-Dec 2026 | AG | `AB` | `JAM` | alias |
| July-Dec 2026 | AH | `RM` | `AB` | alias |
| July-Dec 2026 | AI | `BN` | `RM` | alias |
| July-Dec 2026 | AJ | `EO` | `BN` | alias |
| July-Dec 2026 | AK | `KO` | `EO` | alias |
| July-Dec 2026 | AL | `MP` | `KO` | alias |
| July-Dec 2026 | AM | `JS` | `MP` | alias |
| Jan-June 2027 | AA | `MA` | `` | alias |
| Jan-June 2027 | AB | `NF` | `` | alias |
| Jan-June 2027 | AC | `MH` | `FI` | alias |
| Jan-June 2027 | AD | `FI` | `SJ` | alias |
| Jan-June 2027 | AE | `SJ` | `KK` | alias |
| Jan-June 2027 | AF | `KK` | `SM` | alias |
| Jan-June 2027 | AG | `SM` | `JAM` | alias |
| Jan-June 2027 | AH | `JAM` | `AB` | alias |
| Jan-June 2027 | AI | `AB` | `RM` | alias |
| Jan-June 2027 | AJ | `RM` | `BN` | alias |
| Jan-June 2027 | AK | `BN` | `EO` | alias |
| Jan-June 2027 | AL | `EO` | `KO` | alias |
| Jan-June 2027 | AM | `KO` | `MP` | alias |
| Jan-June 2027 | AN | `MP` | `JS` | alias |
| Jan-June 2027 | AO | `JS` | `` | alias |
| July-Dec 2027 | Z | `MA` | `` | alias |
| July-Dec 2027 | AA | `NF` | `` | alias |
| July-Dec 2027 | AB | `MH` | `` | alias |
