# SPAL Editor

## Editor

### What is SPAL?

Spal is a new file format for saving color palettes. It features the ability to set flags for autogeneration and overlapping colors from different segments.

### EDITOR CONSTRUCTION STILL IN PROGRESS

## Format

#### Segmented Color Palatte (.spal)

```
53 50 41 4C // 'SPAL' File header
71 FF FF FF // flags | r | g | b
/*
    Flags
    7 : Overlap Weight (0 - 15)
    6 : Overlap Weight (0 - 15)
    5 : Overlap Weight (0 - 15)
    4 : Overlap Weight (0 - 15)
    3 : Split channels when overlapping (produces two colors)
    2 : Allow others to overlap with self
    1 : Overlap with others
    0 : Segment break (newline)
*/
```
