# Krant-e: Optimizing EV Fleet Operation

## tl;dr

**What**

An app that helps you see when an EV buggy is actually coming, which route it’s on, and how long you’ll wait, so campus trips feel less like a gamble.

**Why**

IIT Bombay’s EV fleet should be the easy way around campus, but students often bail for autos or cycles because they can’t tell if a buggy will show up in time.

**My role**

I focused on the student-facing app — the flows that help you plan a trip, see what’s coming, and feel a bit less stuck waiting for a buggy.

**Result**

A well researched concept app — live map, ETAs, route filters, and a path toward requesting a buggy when demand spikes along with new and optimized buggy routes and improved branding.

## Context

This was part of the Design General Competition at IIT Bombay — a designathon sprint of about 24 hours. IIT Bombay runs an EV fleet that shuttles between important points on campus, but the system has efficiency and trust problems. The brief was to improve performance and user experience: a new app for the student journey, a clearer identity for the service, and smarter thinking around routes.

I was a student on campus while we designed this, so a lot of the “research” was lived experience plus what the team already knew about how the fleet runs — not a formal multi-week study. Teammates: Sidharth Goutham, Tanmay Kuwalekar, Yashwant Rawat, Hayat Tamboli, Saikat Biswas.

Tools: Figma, Illustrator, Photoshop.

> attach hero / app icon on phone home screen

## Understanding the existing system

### Stakeholders

- Students and other passengers (including us, living the commute)
- EV drivers
- Fleet / campus-transport operators

### How we understood the problem

We didn’t run a formal user survey. In a 24-hour designathon that wasn’t realistic — and honestly, we _were_ the users. We started from mornings when the buggy feels unreliable, the auto or cycle fallback, and the “will I make class?” anxiety. Then we pulled in ops facts we knew about the fleet and clustered pain points on stickies during the sprint.

> attach problem sticky map / insight board  
> (relabel anything that still says “User Survey” on the Behance slides)

### Student reality

- If an EV feels uncertain, people take an auto — nobody’s waiting around romanticizing the buggy.
- Sometimes you just walk. Small groups with cycles often leave on cycles.
- Peak mornings, rain, and exam season make the gamble worse.
- Traveling with friends matters; solo vs group changes what people pick.

### How the system works (facts we designed against)

- Fleet of about **15 EVs** managed by **9 drivers**
- Charging takes roughly **3–4 hours**, depending on station capacity (**20–40 Amp**)
- Service has been around ~**1.5 years**
- Roughly **6 AM to 10 PM**, with a hoped-for arrival every **~5 minutes** at a stop
- Drivers often wait for the next EV at the last stop before leaving
- Routing has been fairly manual / supervisor-led; off-peak gets more ad-hoc
- Stop coverage feels uneven (e.g. Hostel 12 underserved)

### Problem clusters

Things that came up again and again around “commute with EVs”:

- Fewer EVs than demand, overcrowding, ambiguity
- Peak-time chaos, fixed stops, unclear routes, wait time
- Charging cycle and schedule quirks
- Group travel needs, weak communication, delays
- Queue / discipline issues, uneven stop distribution

> attach affinity / sticky problem map

## Defining the opportunity

### Problem statement

How might we make IIT Bombay’s EV buggies feel reliable and easy to use — clearer for students, less wasteful for the fleet — without pretending we can rebuild campus transit overnight?

### Design goals

- Make EV rides easier to discover and trust (availability you can actually see)
- Make routes and waiting times easier to understand
- Support slightly smarter fleet / charging awareness through demand visibility
- Give the service a recognizable, approachable identity (team branding work — kept light here)

## Naming and visual identity

Kept short on purpose — branding was a team thread; my focus was the app experience.

### Why Krant-e?

**Krant-e / क्रांति** plays on _kranti_ (revolution) plus the _e_ of electric — the shift from internal combustion to electric, and a bit of youth energy: if nothing else, at least “revolutions.”

Tagline energy from the identity work: **Krante Karo!**

### Branding snapshot

- Logo / wordmark exploration across Hindi and English
- **Colour palette:** primary blue `#072AC8`, white `#FFFFFF`, charcoal `#1D1C1C`, coral `#FF7B73`, yellow `#FFE16A`, green `#75E579`
- **Typography:** Anek (Latin + Devanagari)
- Route-colored buggy wraps so Route 1 / 2 / 3 read at a glance (coral / yellow / green)

> attach logo story / colour palette / Anek type specimen / buggy wraps

## Mapping the current journey

### Existing passenger journey (late to class)

A familiar morning: need to be at the department around 10.

1. **9:30** — Leaves room (stairs, breakfast) ~15 min
2. **9:45** — Out of hostel, waits for an EV ~**13 min**, anxious
3. **9:58** — Boards
4. **10:04** — Reaches destination, pays (GPay) ~6 min ride
5. **10:06** — Walks to department ~5 min
6. Outcome: **late / absent marked**

The part we could realistically touch in a product sprint: **waiting → boarding → paying**. The rest is sticky infrastructure, capital, or hard behavior change.

> attach existing user journey diagram

### Fleet side (lightweight)

- Vehicle availability and charging cycles
- Driver allocation and “wait for the next EV” habits
- Fixed routes vs actual demand
- Peak overload vs quiet off-peak

## Designing the proposed experience

### Student-facing experience (focus)

**Intervened journey** — same morning, less panic:

1. Opens **Krant-e**, checks estimated time to department, plans a bit earlier
2. Leaves hostel with a calmer wait (~4 min in the concept flow)
3. Boards; optional path to move toward a better stop or **request** a buggy
4. Pays / arrives with roughly a **5-minute margin**
5. Outcome: **on time**

> attach user journey interventions diagram

**App flows and screens**

- Splash + light onboarding: name, role (so later screens can skip junk), usual places (Hostel, Department chips → e.g. Hostel 13, SJC, Main Gate) for predictions and frequent trips
- **Buggy monitor:** campus map with three color-coded routes and live-ish buggy positions
- Nearest-buggy card (e.g. “Nearest buggy will take 12 mins to reach IDC”)
- Route filters + static full-route map
- Buggy detail: route, charge %, ETA to a place
- Menu: Demand heatmap, About, Settings
- **Demand heatmap** with a **Request buggy** action when a spot is hot

> attach onboarding / map / buggy detail / heatmap screens

### Driver or operator experience

Light on purpose (24-hour scope). The student app’s demand view and request direction are the main bridge toward ops — not a full dispatch console.

### Route optimization

We mapped the existing three routes and proposed a clearer network view so shared hubs and overlaps are obvious (Main Building / Convocation, SBI, H10, Main Gate, etc.). The app leans on that clarity: colored routes, filters, and ETA tied to places you care about — with dynamic fleet tweaks called out as future work for all ~15 EVs.

> attach existing routes photo / proposed route map

## Prototype and evaluation

Built as a high-fidelity concept for the designathon (Figma). No multi-week usability study — feedback was sprint-speed: teammates, peers, and the lived “does this calm the wait?” test.

### What we explored

- [x] Passenger discovery and route-finding
- [x] Availability and waiting-time communication
- [ ] Full driver / operator workflows (out of scope for the sprint)
- [x] Route clarity and charging / availability awareness in the UI
- [x] Brand identity as support for recognizing the service

### Feedback and open threads

Things we flagged as next, not finished:

- Group travel / capacity when friends move together
- Smarter routing under peak load for the full fleet
- Growing “see demand” into a real call-an-EV loop
- Occupancy tracking (expensive / manual today)
- Maybe folding autos into the same mental model later

> attach prototype screens / Behance module of UI

## Outcome

In a day, we turned an opaque campus EV habit into something you can _see_: where the buggies are, which route they’re on, how long you might wait, and where demand is stacking up — wrapped in a simple identity so the fleet reads as one service. The win isn’t “we solved campus transit”; it’s making the next trip less of a coin flip.

## Reflection

Designing for a system with students, drivers, charging physics, and fixed roads — in **24 hours** — forces you to pick the highest-leverage slice. Being a student on the same commute was the research shortcut: we didn’t need a lengthy survey to know the anxiety of the wait. Clarity (map, ETA, routes, demand) beat a pile of features. Branding helped where the physical vehicles themselves were ambiguous. Next time I’d want real driver time and a thin ops view earlier — but for a designathon, making the student side legible was the right cut.

## Reference

[Krant-e: Optimizing EV Fleet Operation on Behance](https://www.behance.net/gallery/213624613/Krant-e-Optimizing-EV-Fleet-Operation)
