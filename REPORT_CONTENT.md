# Programming in Java – Assignment 4 (CO4)
## Event-Driven GUI Design

**Student:** S Dharshini  
**Register Number:** 192511260  
**Repository:** CSA09-192511260-Assignment4  
**GitHub URL:** [Paste working repository URL]  
**Java Version:** Java 21

## Objective
Design, implement, trace and evaluate event-driven Java desktop interfaces using AWT/Swing. Keep presentation separate from service and database logic.

## Task 1 – GUI Design Review
See `Task01/README.md` for the ten design diagnoses, corrected class structure and under-100-word justification. `FeePaymentApp.java` implements the separated UI and FeeService. Payment is simulated, not a real gateway transaction.

**Test evidence to insert:** successful payment screenshot; invalid student ID screenshot; invalid amount screenshot.

## Task 2 – Requirement to Event-Driven Design
See `Task02/README.md` for event table, component containment tree, pseudocode, window trace, applet comparison and Map/database comparison. `AppointmentDesk.java` implements department-driven doctor refresh and appointment validation.

**Test evidence to insert:** department change/doctor list screenshot; successful appointment; invalid date.

## Task 3 – From Sketch to Layout
See `Task03/README.md` for nested layout tree, layout justification and alternatives. `LibrarySearch.java` implements the responsive search screen.

**Test evidence to insert:** screenshots at 650×430, 900×600 and 420×300 showing the centre results area resizing.

## Task 4 – Event-Handling Forensics
See `Task04/README.md` for listener diagnosis, repainting explanation, `@Override` and Point/BufferedImage comparison. `DrawingPad.java` stores points and redraws them from `paintComponent`.

**Test evidence to insert:** click counter and dots; same dots after minimizing/restoring.

## Task 5 – Same Screen, Different Event Styles
See `Task05/README.md` for all four listener styles, code patterns and comparison. `CurrencyConverterStyles.java` implements all four listener styles in separate tabs; each supports Enter-key conversion, result dialog and WindowAdapter close handling.

**Test evidence to insert:** valid conversion dialog; invalid amount dialog. Capture valid and invalid conversion screenshots from each of the four tabs.

## Task 6 – Campus Event Registration
See `Task06/README.md` and `Task06/schema.sql`. The Swing/JDBC implementation uses UI/service/data access separation, prepared statements, a unique database constraint, pagination and SwingWorker.

**Test evidence to insert:** valid registration; invalid input; duplicate registration; filtered table; CSV export. Include database configuration details without publishing passwords.

## Complexity analysis summary

| Task / operation | Time | Auxiliary space |
|---|---:|---:|
| Task 1 input validation/payment demo | O(1) | O(1) |
| Task 2 doctor lookup from Map | O(1) expected lookup + O(d) list population | O(d) cached doctor names |
| Task 3 filtering m sample results | O(m) | O(r) displayed results |
| Task 4 repaint stored k points | O(k) | O(k) Point objects |
| Task 5 currency conversion | O(1) | O(1) |
| Task 6 paginated query | Depends on index/query plan; returns O(p) rows | O(p) client rows |

## Final checklist
- [ ] Run each GUI on a desktop environment and capture genuine screenshots.
- [ ] Configure MySQL and run Task 6 SQL script.
- [ ] Verify valid, invalid and duplicate cases.
- [ ] Add screenshots to the matching task folders.
- [ ] Add the working GitHub URL and share repository with faculty.
- [ ] Commit each task separately.
