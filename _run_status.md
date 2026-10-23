# Calendar Export — Last Run Status

- **Timestamp:** 2026-10-23 03:05:04
- **Sheets processed:** July-Dec 2026, Jan-June 2027, July-Dec 2027, Jan-June 2028, July-Dec 2028
- **Status:** 1 LONG CALL WEEKEND ROW ISSUE(S) — see _HEADER_ALERTS.txt

## Header resolution counts

| Status | Count |
|---|---|
| exact | 0 |
| alias (known variant) | 90 |
| fuzzy (similar, used as canonical) | 0 |
| unknown (SKIPPED) | 0 |
| missing (empty header) | 0 |

## Event counts

| Calendar | Events |
|---|---|
| Atzenhoefer | 440 |
| Brochtrup | 280 |
| Fabry | 446 |
| Hanrahan | 417 |
| Iqbal | 496 |
| Janus | 342 |
| Kashyap | 428 |
| Kohl | 138 |
| Marin | 2 |
| Marmer | 453 |
| Martin | 323 |
| Mauer | 2 |
| Maurer | 270 |
| Novak | 275 |
| Organ | 76 |
| Ortman | 283 |
| Povlich | 287 |
| Schaeve | 281 |
| **MasterSchedule** | 3387 |

Total leave/vacation events (across all sheets): 127
Total "-OFF- Long Call Weekend" events (across all sheets, deduped): 129

## Long call weekend (LCW) row issues

Week-header rows carrying the `LCW` marker that could not be turned
into an OFF day cleanly. Rows listed as DROPPED produced no event.

| Sheet | Row | Issue | Detail |
|---|---|---|---|
| Jan-June 2028 | 6 | empty provider cell in column D | week of 2027-12-27 — no OFF event created |

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
| July-Dec 2026 | C | `MD*` | `Inpatient MD` | alias |  |
| July-Dec 2026 | D | `APP 1 Inpatient *` | `Inpatient APP1` | alias |  |
| July-Dec 2026 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | alias |  |
| July-Dec 2026 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | alias |  |
| July-Dec 2026 | H | `AM` | `CATH AM` | alias |  |
| July-Dec 2026 | I | `PM` | `CATH PM` | alias |  |
| July-Dec 2026 | M | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | alias |  |
| July-Dec 2026 | N | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 PM` | alias |  |
| July-Dec 2026 | O | `APP 5 CMH Clinic AM` | `CMH Clinic APP2 AM` | alias |  |
| July-Dec 2026 | P | `APP 5 CMH Clinic PM` | `CMH Clinic APP2 PM` | alias |  |
| July-Dec 2026 | S | `APP 3 BRK Clinic AM` | `BRK APP1 (0810-0850)` | alias |  |
| July-Dec 2026 | T | `APP 3 BRK Clinic PM` | `BRK APP1 (1230-1600)` | alias |  |
| July-Dec 2026 | U | `APP 7 AM` | `APP 7 AM` | alias | position drift; schema expected `Cath APP AM` here |
| July-Dec 2026 | V | `APP 7 PM` | `APP 7 PM` | alias | position drift; schema expected `Cath APP PM` here |
| July-Dec 2026 | W | `APP 6 Cath AM*` | `Cath APP AM` | alias | position drift; schema expected `APP 7` here |
| July-Dec 2026 | X | `APP 6 Cath PM*` | `Cath APP PM` | alias | position drift; schema expected `LCW` here |
| July-Dec 2026 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| July-Dec 2026 | Z | `Admin` | `Admin` | alias | position drift; schema expected `APP 7 AM` here |
| Jan-June 2027 | C | `MD` | `Inpatient MD` | alias |  |
| Jan-June 2027 | D | `APP 1 Inpatient` | `Inpatient APP1` | alias |  |
| Jan-June 2027 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | alias |  |
| Jan-June 2027 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | alias |  |
| Jan-June 2027 | H | `AM` | `CATH AM` | alias |  |
| Jan-June 2027 | I | `PM` | `CATH PM` | alias |  |
| Jan-June 2027 | M | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | alias |  |
| Jan-June 2027 | N | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 PM` | alias |  |
| Jan-June 2027 | O | `APP 5 CMH Clinic AM` | `CMH Clinic APP2 AM` | alias |  |
| Jan-June 2027 | P | `APP 5 CMH Clinic PM` | `CMH Clinic APP2 PM` | alias |  |
| Jan-June 2027 | S | `APP 3 BRK Clinic` | `BRK APP1 (0810-0850)` | alias |  |
| Jan-June 2027 | T | `APP 3 BRK Clinic` | `BRK APP1 (1230-1600)` | alias |  |
| Jan-June 2027 | U | `APP 7 AM` | `APP 7 AM` | alias | position drift; schema expected `Cath APP AM` here |
| Jan-June 2027 | V | `APP 7 PM` | `APP 7 PM` | alias | position drift; schema expected `Cath APP PM` here |
| Jan-June 2027 | W | `Cath APP 6 AM` | `Cath APP AM` | alias | position drift; schema expected `APP 7` here |
| Jan-June 2027 | X | `Cath APP 6 PM` | `Cath APP PM` | alias | position drift; schema expected `LCW` here |
| Jan-June 2027 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| Jan-June 2027 | Z | `Admin` | `Admin` | alias | position drift; schema expected `APP 7 AM` here |
| July-Dec 2027 | C | `MD` | `Inpatient MD` | alias |  |
| July-Dec 2027 | D | `APP 1 Inpatient` | `Inpatient APP1` | alias |  |
| July-Dec 2027 | E | `APP 4 Inpatient AM` | `Inpatient APP2 AM` | alias |  |
| July-Dec 2027 | F | `APP 4 Inpatient  PM` | `Inpatient APP2 PM` | alias |  |
| July-Dec 2027 | H | `AM` | `CATH AM` | alias |  |
| July-Dec 2027 | I | `PM` | `CATH PM` | alias |  |
| July-Dec 2027 | M | `APP 2 CMH Clinic AM` | `CMH Clinic APP1 AM` | alias |  |
| July-Dec 2027 | N | `APP 2 CMH Clinic PM` | `CMH Clinic APP1 PM` | alias |  |
| July-Dec 2027 | O | `APP 5 CMH Clinic AM` | `CMH Clinic APP2 AM` | alias |  |
| July-Dec 2027 | P | `APP 5 CMH Clinic PM` | `CMH Clinic APP2 PM` | alias |  |
| July-Dec 2027 | S | `APP 3 BRK Clinic` | `BRK APP1 (0810-0850)` | alias |  |
| July-Dec 2027 | T | `APP 3 BRK Clinic` | `BRK APP1 (1230-1600)` | alias |  |
| July-Dec 2027 | U | `APP 7 AM` | `APP 7 AM` | alias | position drift; schema expected `Cath APP AM` here |
| July-Dec 2027 | V | `APP 7 PM` | `APP 7 PM` | alias | position drift; schema expected `Cath APP PM` here |
| July-Dec 2027 | W | `Cath APP 6 AM` | `Cath APP AM` | alias | position drift; schema expected `APP 7` here |
| July-Dec 2027 | X | `Cath APP 6 PM` | `Cath APP PM` | alias | position drift; schema expected `LCW` here |
| July-Dec 2027 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| July-Dec 2027 | Z | `Admin` | `Admin` | alias | position drift; schema expected `APP 7 AM` here |
| Jan-June 2028 | C | `MD` | `Inpatient MD` | alias |  |
| Jan-June 2028 | D | `APP Inpatient 1` | `Inpatient APP1` | alias |  |
| Jan-June 2028 | E | `APP Inpatient 2 AM` | `Inpatient APP2 AM` | alias |  |
| Jan-June 2028 | F | `APP Inpatient 2 PM` | `Inpatient APP2 PM` | alias |  |
| Jan-June 2028 | H | `AM` | `CATH AM` | alias |  |
| Jan-June 2028 | I | `PM` | `CATH PM` | alias |  |
| Jan-June 2028 | M | `CMH Clinic APP 1 AM` | `CMH Clinic APP1 AM` | alias |  |
| Jan-June 2028 | N | `CMH Clinic APP 1 PM` | `CMH Clinic APP1 PM` | alias |  |
| Jan-June 2028 | O | `CMH Clinic APP 2 AM` | `CMH Clinic APP2 AM` | alias |  |
| Jan-June 2028 | P | `CMH Clinic APP 2 PM` | `CMH Clinic APP2 PM` | alias |  |
| Jan-June 2028 | S | `BRK APP  (0810-0850)` | `BRK APP1 (0810-0850)` | alias |  |
| Jan-June 2028 | T | `BRK APP  (1230-1600)` | `BRK APP1 (1230-1600)` | alias |  |
| Jan-June 2028 | U | `APP 7 AM` | `APP 7 AM` | alias | position drift; schema expected `Cath APP AM` here |
| Jan-June 2028 | V | `APP 7 PM` | `APP 7 PM` | alias | position drift; schema expected `Cath APP PM` here |
| Jan-June 2028 | W | `Cath AM` | `Cath APP AM` | alias | position drift; schema expected `APP 7` here |
| Jan-June 2028 | X | `Cath PM` | `Cath APP PM` | alias | position drift; schema expected `LCW` here |
| Jan-June 2028 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| Jan-June 2028 | Z | `Admin` | `Admin` | alias | position drift; schema expected `APP 7 AM` here |
| July-Dec 2028 | C | `MD` | `Inpatient MD` | alias |  |
| July-Dec 2028 | D | `APP Inpatient 1` | `Inpatient APP1` | alias |  |
| July-Dec 2028 | E | `APP Inpatient 2 AM` | `Inpatient APP2 AM` | alias |  |
| July-Dec 2028 | F | `APP Inpatient 2 PM` | `Inpatient APP2 PM` | alias |  |
| July-Dec 2028 | H | `AM` | `CATH AM` | alias |  |
| July-Dec 2028 | I | `PM` | `CATH PM` | alias |  |
| July-Dec 2028 | M | `CMH Clinic APP 1 AM` | `CMH Clinic APP1 AM` | alias |  |
| July-Dec 2028 | N | `CMH Clinic APP 1 PM` | `CMH Clinic APP1 PM` | alias |  |
| July-Dec 2028 | O | `CMH Clinic APP 2 AM` | `CMH Clinic APP2 AM` | alias |  |
| July-Dec 2028 | P | `CMH Clinic APP 2 PM` | `CMH Clinic APP2 PM` | alias |  |
| July-Dec 2028 | S | `BRK APP  (0810-0850)` | `BRK APP1 (0810-0850)` | alias |  |
| July-Dec 2028 | T | `BRK APP  (1230-1600)` | `BRK APP1 (1230-1600)` | alias |  |
| July-Dec 2028 | U | `APP 7 AM` | `APP 7 AM` | alias | position drift; schema expected `Cath APP AM` here |
| July-Dec 2028 | V | `APP 7 PM` | `APP 7 PM` | alias | position drift; schema expected `Cath APP PM` here |
| July-Dec 2028 | W | `Cath AM` | `Cath APP AM` | alias | position drift; schema expected `APP 7` here |
| July-Dec 2028 | X | `Cath PM` | `Cath APP PM` | alias | position drift; schema expected `LCW` here |
| July-Dec 2028 | Y | `LCW` | `LCW` | alias | position drift; schema expected `Admin` here |
| July-Dec 2028 | Z | `Admin` | `Admin` | alias | position drift; schema expected `APP 7 AM` here |

## Leave header details

| Sheet | Col | Raw | Expected | Status |
|---|---|---|---|---|
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
| July-Dec 2027 | AA | `MA` | `` | alias |
| July-Dec 2027 | AB | `NF` | `` | alias |
| July-Dec 2027 | AC | `MH` | `FI` | alias |
| July-Dec 2027 | AD | `FI` | `SJ` | alias |
| July-Dec 2027 | AE | `SJ` | `KK` | alias |
| July-Dec 2027 | AF | `KK` | `SM` | alias |
| July-Dec 2027 | AG | `SM` | `JAM` | alias |
| July-Dec 2027 | AH | `JAM` | `AB` | alias |
| July-Dec 2027 | AI | `AB` | `RM` | alias |
| July-Dec 2027 | AJ | `RM` | `BN` | alias |
| July-Dec 2027 | AK | `BN` | `EO` | alias |
| July-Dec 2027 | AL | `EO` | `KO` | alias |
| July-Dec 2027 | AM | `KO` | `MP` | alias |
| July-Dec 2027 | AN | `MP` | `JS` | alias |
| July-Dec 2027 | AO | `JS` | `` | alias |
| Jan-June 2028 | AA | `MA` | `` | alias |
| Jan-June 2028 | AB | `NF` | `` | alias |
| Jan-June 2028 | AC | `MH` | `FI` | alias |
| Jan-June 2028 | AD | `FI` | `SJ` | alias |
| Jan-June 2028 | AE | `SJ` | `KK` | alias |
| Jan-June 2028 | AF | `KK` | `SM` | alias |
| Jan-June 2028 | AG | `SM` | `JAM` | alias |
| Jan-June 2028 | AH | `JAM` | `AB` | alias |
| Jan-June 2028 | AI | `AB` | `RM` | alias |
| Jan-June 2028 | AJ | `RM` | `BN` | alias |
| Jan-June 2028 | AK | `BN` | `EO` | alias |
| Jan-June 2028 | AL | `EO` | `KO` | alias |
| Jan-June 2028 | AM | `KO` | `MP` | alias |
| Jan-June 2028 | AN | `MP` | `JS` | alias |
| Jan-June 2028 | AO | `JS` | `` | alias |
| July-Dec 2028 | AA | `MA` | `` | alias |
| July-Dec 2028 | AB | `NF` | `` | alias |
| July-Dec 2028 | AC | `MH` | `FI` | alias |
| July-Dec 2028 | AD | `FI` | `SJ` | alias |
| July-Dec 2028 | AE | `SJ` | `KK` | alias |
| July-Dec 2028 | AF | `KK` | `SM` | alias |
| July-Dec 2028 | AG | `SM` | `JAM` | alias |
| July-Dec 2028 | AH | `JAM` | `AB` | alias |
| July-Dec 2028 | AI | `AB` | `RM` | alias |
| July-Dec 2028 | AJ | `RM` | `BN` | alias |
| July-Dec 2028 | AK | `BN` | `EO` | alias |
| July-Dec 2028 | AL | `EO` | `KO` | alias |
| July-Dec 2028 | AM | `KO` | `MP` | alias |
| July-Dec 2028 | AN | `MP` | `JS` | alias |
| July-Dec 2028 | AO | `JS` | `` | alias |
