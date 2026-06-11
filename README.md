# Interactive Sankey Diagram for Forensic Case Tracking for Train Crash Sikew, Nakhonratchasima

## Overview

This interactive Sankey diagram visualizes the relationship between:

```text
Body Bag
    ↓
PM Number + Body Condition
    ↓
ID Mask
```

The graph is designed for forensic case tracking while protecting personal information.

---

## Features

### Privacy Protection

* Personal names in body bag labels are automatically masked.
* Example:

```text
1.(4 ชาย บก.2 นายสมชาย ใจดี)
↓
1.(4 ชาย บก.2 ...)
```

* Anonymous labels such as:

```text
18.(เศษชิ้นส่วน)
```

remain unchanged.

---

## Interactive Functions

### Click a Body Bag

Highlights:

* Related PM Number with Body Condition
* Related ID Mask

```text
Bag
 ↓
PM
 ↓
ID
```

---

### Click a PM Number with Body Condition

Highlights:

* Related Body Bag(s)
* Related ID Mask(s)

```text
Bag ← PM → ID
```

---

### Click an ID Mask

Highlights:

* Related PM Number with Body Condition
* Related Body Bag

```text
Bag
 ↑
PM
 ↑
ID
```

---

## Highlight Behavior

### Selected Nodes

* Keep original color.

### Related Links

* Highlight in red.

### Unrelated Nodes

* Fade to light gray.

### Unrelated Links

* Become nearly transparent.

---

## Reset

Click the **Reset Highlight** button at the upper-left corner to restore the original graph.

---

## Graph Layout

| Dimension                  | Position |
| -------------------------- | -------- |
| Body Bag                   | Left     |
| PM Number + Body Condition | Center   |
| ID Mask                    | Right    |

---

## Data Aggregation

Identical body bag values are merged into a single node.

Example:

```text
18.(เศษชิ้นส่วน)
18.(เศษชิ้นส่วน)
18.(เศษชิ้นส่วน)
```

will be displayed as one node with multiple outgoing relationships.

---

## Intended Use

This visualization is intended for:

* Forensic case management
* Disaster victim identification (DVI)
* Mass casualty investigations
* Body tracking workflow analysis
* Relationship exploration between forensic entities

---

## Notes

* The graph is fully interactive.
* The HTML file can be opened directly in any modern web browser.
* The layout automatically adjusts to different screen sizes.
* No internet connection is required after the HTML file is generated.
