# Train FSM Truth Table

| Number | Arms Down | Alarm On | Northbound Present | Southbound Present | North Approach | South Approach | North Depart | South Depart | Ringing | Safety Hazard/ Transiton |Checked|
|--------|-----------|----------|--------------------|--------------------|----------------|----------------|--------------|--------------|---------|---------------|-----|
| 0      | 0         | 0        | 0                  | 0                  | 0              | 0              | 0            | 0            | 0       | 0             |  1  |
| 1      | 0         | 0        | 0                  | 1                  | 0              | 1              | 0            | 0            | 0       | 5             |  1  |
| 2      | 0         | 0        | 1                  | 0                  | 1              | 0              | 0            | 0            | 0       | 6             |  1  |
| 3      | 0         | 0        | 1                  | 1                  | 1              | 1              | 0            | 0            | 0       | 7             |  1  |
| 4      | 0         | 1        | 0                  | 0                  | 0              | 0              | 0            | 0            | 1       |               13/14/15| 1 |
| 5      | 0         | 1        | 0                  | 1                  | 0              | 1              | 0            | 1            | 1       | 13            |  1  |
| 6      | 0         | 1        | 1                  | 0                  | 1              | 0              | 0            | 0            | 1       | 14            |  1  |
| 7      | 0         | 1        | 1                  | 1                  | 1              | 1              | 0            | 0            | 1       | 15            |  1  |
| 8      | 1         | 0        | 0                  | 0                  | 0              | 0              | 0            | 0            | 0       | 0             |  1  |
| 9      | 1         | 0        | 0                  | 1                  | 0              | 0              | 0            | 1            | 0       | 17            |  1  |
| 10     | 1         | 0        | 1                  | 0                  | 0              | 0              | 1            | 0            | 0       | 17            |  1  |
| 11     | 1         | 0        | 1                  | 1                  | 0              | 0              | 1            | 1            | 0       | 17            |  1  |
| 12     | 1         | 1        | 0                  | 0                  | 0              | 0              | 0            | 0            | 0       | 16            |  1  |
| 13     | 1         | 1        | 0                  | 1                  | 0              | 1              | 0            | 1            | 1       | 8             |  1  |
| 14     | 1         | 1        | 1                  | 0                  | 1              | 0              | 0            | 0            | 1       | 8             |  1  |
| 15     | 1         | 1        | 1                  | 1                  | 1              | 1              | 0            | 0            | 1       | 8             |  1  |

---

## Invariants

| Number | Invariant                                     |
|--------|-----------------------------------------------|
| 16     | Alarm could be on or off while no train there |
| 17     | Alarm not on while train is present           |
| 18     | Arms are up/down while no train present       |
| 19     | ...                                           |