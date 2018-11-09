# JudgeAssignerManager (JAM)

The JudgeAssignerManager, JAM for short, is designed to select judges from a given pool and assign them to tournaments.
JAM takes input in the form of a CSV file, and outputs similarly.
The goal is to evenly distribute shifts among different people, so that no one judge has to judge more than another.

## Example CSV

### Judge Names (Input)

| Competitor Last Name | Competitor First Name | Judge Last Name | Judge First Name | Judge Email |
|-|-|-|-|-|
| Marco | Snella | Marco | James | hey@example.com |
| Smith | Kat | Smith | Lilith | hello@example.com |
| Trimm | Leigh | Crimie | Kristen | sup@example.com |

### Competitors (Input)

| Competitor Last Name | Competitor First Name | Tournaments |
|-|-|-|
| Marco | Snella | scu,league1,berkely |
| Smith | Kat | league1,league2 |
| Trimm | Leigh | league2,superdebate2 |

### Tournament (Input, Output, The current tournaments to generate for)

| Shift | Event | Judge Last Name | Judge First Name | Judge Email | Competitor Last Name | Competitor First Name |
|-------|-------|-----------------|------------------|-------------|----------------------|-----------------------|
| AM    |       |                 |                  |             |                      |                       |
| AM    |       |                 |                  |             |                      |                       |
| PM    |       |                 |                  |             |                      |                       |
|  ...  |       |                 |                  |             |                      |                       |
| PM    |       |                 |                  |             |                      |                       |

