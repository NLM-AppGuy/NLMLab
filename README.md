# NLMLab for NLM

**NLMLab for NLM** is a free Windows companion app for **Non League Manager**, created by **NLM App Guy**.

It combines live squad analysis and player search in one place: sync your current NLM squad, build a Best XI, rate formations, check depth, identify surplus players, search NLM's live player pool using underlying player attributes, compare targets against your current squad and see what players are asking for in wages.

> NLMLab is an independent fan-made companion and is not affiliated with or endorsed by the developers of Non League Manager.

## What NLMLab does

### Squad

- Syncs your **current live NLM squad** — no duplicate squad maintenance
- Builds an **availability-aware Best XI & Bench**
- Excludes players NLM says are injured, suspended, at work or otherwise unavailable for the next match
- Lets you switch between **Available XI** and **Full-strength XI**
- **Formation Rater** compares supported formations against the squad you actually have
- **Formation Depth** shows natural and cover options by formation position
- **Players to Move On** highlights players outside the XI, recommended bench and key cover, including weekly wages tied up in that group
- Squad Overview supports filters, availability, roles and football-position sorting

### Scout

- Search the live NLM player candidate pool by name, position, age, distance and underlying player attributes
- Filter on Pace, Finishing, Passing, Defending, Physicality, Stamina, Aerial, Decisions and Goalkeeping
- **LabLogic** gives a position-sensitive 0–100 comparison score for your current NLM level
- Shows **asking wage** where NLM makes it available
- Add players to a local NLMLab shortlist
- Shortlisted/search players are compared directly with your live squad using compact impact labels:
  - `#1` — new first choice
  - `XI+` — improves the starting XI
  - `DEPTH+` — improves squad depth
  - `SAME` — no squad upgrade

## Where Player Search results come from

NLMLab does **not** blindly load every player in the whole NLM database.

NLM supplies a live **candidate pool** for your current career, club, level and search context. NLMLab then reads the returned player profiles and applies its own attribute filters and analysis.

So if a fresh goalkeeper search says **642 candidates**, that means NLM returned 642 keepers to that live search context. The number can change with your club, level, career state and filters.

In short:

**NLM supplies the candidate pool. NLMLab does the analysis.**

## LabLogic

LabLogic is NLMLab's position-sensitive player rating.

It combines the attributes that matter for a role into a single **0–100 comparison score**, interpreted relative to the level of your current NLM career. Different positions value different attributes, so the same player can rate differently depending on where you use him.

The model was designed with AI-assisted football logic, but it is a **fixed local model** inside NLMLab — your player data is not sent to an AI service every time a rating is calculated.

The exact weighting recipe is intentionally not published. LabLogic is a decision aid for comparing players, not a claim to reproduce NLM's internal player ability or predict match performance.

## Read only

NLMLab is intentionally **read only**.

It reads information from the running NLM career but does not:

- edit the NLM save
- change player attributes
- alter finances
- sign or release players
- submit bids or contract offers
- alter scouting knowledge

NLM stays in control of the career.

## Beta

**Current platform:** Windows PC  
**Current release:** v1.5.1 Beta 2

This is beta software. NLM updates can change the live interface NLMLab reads, so a future NLM update may temporarily break a feature until NLMLab is updated.

## Download

Go to the **Releases** section of this repository and download:

**`NLMLab-v1.5.1-beta.2-Windows.zip`**

Extract the ZIP before running the installer.

## NLM connection

NLMLab reads the locally running NLM WebView on your own PC. **The Windows installer now enables this connection automatically** — there is no separate setup script to run.

### First install

1. **Close NLM completely**
2. Run the NLMLab installer
3. Approve the Windows administrator prompt when requested
4. Start NLM normally through Steam
5. Load your career
6. Open NLMLab

NLMLab should show **Connected to NLM** and sync your squad.

If NLM was open during installation, close and reopen NLM once so the connection setting takes effect.

The connection is local to your PC. NLMLab does not require an NLMLab account or cloud squad database. More detail and troubleshooting are in [CONNECTION_SETUP.md](CONNECTION_SETUP.md).

## Updating

Install the newer NLMLab release directly over the existing version.

NLMLab's local shortlist/settings are designed to remain in place across updates.

## Windows warning

Current beta installers are not yet code-signed, so Windows SmartScreen may show **Unknown publisher** / **Windows protected your PC**.

If you downloaded NLMLab from this official repository:

1. Select **More info**
2. Select **Run anyway**

## Privacy

NLMLab is local-first. See [PRIVACY.md](PRIVACY.md).

## Beta testing

Please read [BETA_TESTING.md](BETA_TESTING.md) before reporting issues.

Bug reports and feature suggestions can be submitted through the **Issues** tab. Screenshots are especially useful.

## The story so far

NLMLab grew out of a very simple problem: keeping a squad-management spreadsheet useful alongside NLM.

**Google Sheet → SquadLab → Bulk Entry → ScoutLab → live NLM sync → NLMLab**

SquadLab started as a way to rank a manually entered squad and work out a Best XI. It became a standalone app, added formation analysis and bulk entry, but the biggest problem remained: maintaining the same squad in both NLM and SquadLab.

ScoutLab proved that the running NLM career could be read safely and used for richer player searching. NLMLab brought the two ideas together: live squad sync on one side, player discovery on the other, with the same LabLogic and squad-impact model across both.

## About NLM App Guy

I'm a football-management fan who has always ended up building something alongside the game. I've played football management games since **CM 01/02** and still play it today.

Over the years that has meant databases, utilities and far too many homemade spreadsheets. NLMLab is the latest version of the same habit: take the information the game gives you and make squad and recruitment decisions easier to see.

## Support NLMLab

NLMLab is completely free and built in my spare time for the NLM community.

If you're enjoying it and want to support future updates, you can buy me a coffee. There is absolutely no obligation.

**Ko-fi:** https://ko-fi.com/nlm_appguy

Any voluntary support goes towards my grassroots football project, **Fitness Football Nuneaton (FFN)**.

**FFN:** https://www.ffnuneaton.co.uk

---

**Created by NLM App Guy**
