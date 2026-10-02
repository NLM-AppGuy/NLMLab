# Changelog

## v1.5.1 Beta 2

### Installer / onboarding
- NLM connection setup is now built directly into the Windows installer
- Removed the separate Enable Connection helper from the normal install flow
- Installer requests Windows administrator approval only when the connection setting needs to be created
- Existing installs with the connection already configured do not need to repeat setup
- Updated beta documentation and quick-start instructions

## v1.5.1 Beta 1

### Beta release candidate
- Cross-app typography, spacing and readability pass
- Consistent table, panel, button and helper-text hierarchy
- Improved narrow-window behaviour without crushing data text
- LabLogic hover/explainer treatment on LAB columns
- Cleaner compact squad-impact labels with key/hover text
- Players to Move On now includes weekly wage and combined wages freed

### Formation Depth
- New **Formation Depth** page driven by the selected formation
- Shows natural and cover options for each required formation position
- Duplicate formation slots are grouped into a single positional depth unit
- Shows **Need**, natural count, cover count and available-now count
- Caps visible depth at five players per position with overflow count
- NAT / COVER labels and LabLogic strength colouring
- Thin / OK / Deep depth diagnosis for quick recruitment/surplus scanning

## v1.4.x

### UI / UX polish
- Defined a consistent visual hierarchy across all NLMLab pages
- Improved Squad Overview table readability and header sorting
- Football-position sorting uses GK → LB → LCB → RCB → RB → CDM → CM → CAM → LW → RW → ST
- Reworked Help / About content for beta onboarding
- Added clearer Player Search explanation and LabLogic explanation

## v1.2.x – v1.3.x

### Live squad experience
- Added squad-table filters and direct column sorting
- Availability-aware squad status
- Combined SquadLab-style UI with ScoutLab live search
- Reworked shortlist presentation and player profiles

## v1.1.0

### Availability-aware XI
- Reads NLM injury, suspension, at-work and other availability states
- **Available XI** becomes the default match-useful view
- Added **Full-strength XI** comparison
- Bench and XI recalculate around unavailable players

## v1.0.0

### First NLMLab local build
- Combined the SquadLab and ScoutLab concepts into one app
- Live NLM squad sync
- Best XI & Bench
- Formation Rater
- Players to Move On
- Raw Player Search
- LabLogic
- Asking wages
- Local shortlist with live squad-impact comparisons
- Read-only live NLM connection
