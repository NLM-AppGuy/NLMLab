# NLMLab for NLM v1.5.1 Beta 2

This Beta 2 build keeps the first public NLMLab feature set and improves the install/onboarding experience: the SquadLab squad-analysis idea and ScoutLab player-search idea brought together around a **live, read-only NLM career connection**.

## The big change: no more maintaining your squad twice

NLMLab syncs your current squad directly from the running NLM career.

That live squad powers:

- **Squad Overview**
- **Best XI & Bench**
- **Formation Rater**
- **Formation Depth**
- **Players to Move On**
- shortlist / recruitment impact comparisons

Sign, release or lose a player in NLM, sync NLMLab, and the analysis updates around the new squad.

## Best XI that understands availability

NLMLab reads the availability information NLM provides for the next match.

The default **Available XI** can exclude players who are injured, suspended, at work or otherwise unavailable. You can switch to **Full-strength XI** when you want to compare the squad without temporary absences.

## Formation Depth

A new formation-driven depth chart makes squad balance visible at a glance.

For every positional unit required by the selected formation, NLMLab shows:

- how many starters the shape needs
- natural-position options
- cover-position options
- how many are available now
- up to five ranked players with LabLogic ratings
- a quick **Thin / OK / Deep** depth reading

It is designed to make things like **one natural LB but six natural CMs** obvious immediately.

## Player Search

Player Search starts from the candidate pool NLM supplies for your live career/search context, then NLMLab reads those player profiles and applies its own attribute filters.

You can search using underlying values for:

- Pace
- Finishing
- Passing
- Defending
- Physicality
- Stamina
- Aerial
- Decisions
- Goalkeeping

You can also filter by position, age and distance, load asking wages, shortlist targets and compare them directly against your current squad.

## LabLogic

LabLogic is NLMLab's position-sensitive 0–100 comparison score.

It uses the attributes that matter for the selected role and interprets them in the context of your current NLM level. The model is fixed and local to NLMLab. The exact weighting recipe is deliberately not published.

LabLogic is a comparison aid — not an official NLM ability rating or a prediction of match performance.

## Squad impact labels

Scout/search targets use compact squad-impact labels:

- `#1` — new first choice
- `XI+` — improves starting XI
- `DEPTH+` — improves squad depth
- `SAME` — no squad upgrade

## Players to Move On

Players outside the Best XI, recommended bench and key natural-position cover are shown together with their current weekly wages and the combined weekly wage tied up in the group.

## Read only

NLMLab reads the running NLM career. It does not edit the NLM save, change attributes/finances, submit offers, sign players or alter scouting knowledge.

## Windows / connection setup

This beta is **Windows only**.

**Beta 2 removes the separate connection helper.** The installer now enables NLMLab's local NLM connection automatically.

For a first install: close NLM, run the installer, approve the Windows administrator prompt if requested, then start NLM normally through Steam and load your career before opening NLMLab.

See the repository README / `CONNECTION_SETUP.md` for troubleshooting.

## Unsigned beta installer

The installer is not yet code-signed, so Windows may show an **Unknown publisher / Windows protected your PC** warning.

If you downloaded the release from this official repository:

**More info → Run anyway**

## Feedback

For beta feedback, screenshots are especially useful. Please include the NLMLab version and what you were doing when the problem happened.

**Created by NLM App Guy** 💛💚
