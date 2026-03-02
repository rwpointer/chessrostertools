# ♞ RoundReady — The TD Toolkit

**A complete chess tournament round printout tool for Tournament Directors.**

Developed by Richard Pointer · IO IA

---

## What It Does

RoundReady takes a SwissSys or ChessRoster pairings export file and generates three print-ready documents for each section — all in a single run:

1. **Pairing Slips** — One slip per board, formatted for placement at the board. White player on the left, Black player on the right, board number in the center, result circles to mark by hand, and signature lines for both players. Five slips per page, sized to fill a full 8.5×11 sheet so pages can be stacked and cut cleanly.

2. **Results Recording Sheet** — A compact table listing every board in the section with result circles (1-0, ½-½, 0-1) for the TD to record outcomes. Byes are listed separately at the bottom.

3. **Alphabetical Player Lookup Sheet** — Every player in the section sorted A–Z by last name, showing their board number and color assignment. Used for players who can't find their pairing. Automatically paginates if the section is large.

---

## How to Use

1. **Export your pairings** from SwissSys or ChessRoster as a `.txt` file
2. **Open RoundReady** in your browser at [https://rwpointer.github.io/chessrostertools](https://rwpointer.github.io/chessrostertools)
3. **Load your file** — drag and drop or click to browse
4. **Select sections** to print (all sections checked by default)
5. **Set options** — slips per page, tournament name override, round override, time control
6. **Toggle sheets** — choose whether to include the results sheet and alpha lookup sheet
7. **Click Generate** — preview appears instantly in the browser
8. **Click Print All Sheets** — use these print settings for best results:
   - Margins: **None**
   - Scale: **100%**
   - Headers and footers: **Off**

---

## Input File Format

RoundReady reads the standard SwissSys / ChessRoster tab-delimited pairings export. The file should look like this:

```
Pairings for Round 4. Tournament Name: Section Name
Bd    Team    Res    White              Team    Res    Black
1     GFCC    0      Smith, John (3.0)  KOTS    1      Jones, Emma (3.0)
2     ...
```

Multiple sections in a single file are supported. Each section starts fresh on a new page.

---

## Features

- Supports multiple sections in one file (K-12, K-6, Extra Games, etc.)
- Each section's pairing slips, results sheet, and alpha sheet are grouped together
- Blank slip placeholders on partial pages keep cut lines consistent
- Alphabetical lookup sheet paginates automatically for large sections
- Time control displayed on alpha lookup sheet header
- Works entirely in the browser — no installation, no server, no data uploaded anywhere
- Single HTML file, works offline once loaded

---

## Print Tips

- Always set print margins to **None** and scale to **100%**
- Use **Ctrl+Shift+R** (or **Cmd+Shift+R** on Mac) to hard-refresh after uploading a new version
- The dashed lines on pairing slip pages are cut guides — stack all pages and cut straight through

---

## About

RoundReady was built for Tournament Directors running scholastic chess events. It replaces manual slip preparation with a fast, reliable one-click workflow.

**Developed by Richard Pointer · IO IA**
