---
type: Concept
title: Stretched Paradox (lengthening the design)
description: Scaling the Paradox hull up in length — Matt Layden's rule of thumb for scaling scantlings, worked dimensions for a 10% stretch, a square-root method for scaling sail area, Pete Hodges's 1.1x-scale build, chine-runner curvature and drag at larger scale, the bilge-keel debate, and the still-undrawn idea of a genuinely larger Layden sharpie.
tags: [paradox, design, modification, length, stretch, scantlings, virtual-remodelling]
timestamp: 2026-07-03T00:00:00Z
---

# Stretched Paradox

Stretching the Paradox's **overall length** is the one recorded proposal in
the archive to change the hull's principal dimension, rather than a detail
like the chine, rudder, or rig. It stands apart from the documented,
designer-led iterations tracked in
[rudder and chine experiments](/design/rudder.md) and
[chine runners](/chine-runners/how-they-work.md),
both of which kept the hull length fixed.

## Matt Layden's scaling rule: multiply the scantlings by the enlargement factor

**Matt Layden's** governing rule for stretching a Paradox is simple:
**multiply the scantlings by the enlargement factor**. Up to roughly a
**25% enlargement**, a builder "shouldn't have any problem" applying the
straight multiplication; beyond that, the builder must **rethink bulkhead
placement and scantlings** from scratch rather than simply scaling.
**Dave Gerr's book *The Elements of Boat Strength*** is the recommended
reference for working out revised scantlings at any scale.

Scaling must be applied to the **whole design** — length, beam, and rig
together — to preserve the proportions; scaling length alone would "alter
the overall qualities of the design and come out with something new" rather
than produce a true enlargement. Under uniform scaling, sail area scales
with the *square* of the linear factor, so a stretch that lengthens the hull
10% grows the sail's area by more than 10%.

## Concrete dimensions for a 10% stretch

Working the rule through for a **10% stretch** (a factor Matt Layden had
already blessed) gives concrete numbers from the stock **13' 10" LOA**, and
these dimensions at 1.1× scale:

| Dimension | Stock | ×1.1 |
|---|---|---|
| LOA | 13' 10" | **15' 2 5/8"** |
| Beam (BOA) | — | **4' 4 13/16"** |
| Draft | — | **9 7/8"** |
| Headroom under the hatch | 36 1/2" (one builder's own boat) | **40"** |

The main timbers (chine logs, sheer clamps) need **not** be enlarged at the
bigger scale, since they are already generous relative to the boat's size
("a real dock rammer"). Working in **metric** makes the 1.1× multiplication
easy to apply to every dimension except timber sizes. The method holds up to
roughly a **15%** enlargement — a slightly more conservative ceiling than the
25% figure for straight scantling multiplication above — before a scantlings
reference such as Dave Gerr's *The Elements of Boat Strength* is needed to
check the structure.

### Angles don't change; plywood-sheet fit becomes the real constraint

Not every dimension is a simple length: parts on **angles** — the
bulkheads, stem, the pipe used in the roller-furling rig, and cabin
supports — need re-lofting or trigonometry rather than a flat
multiplication, since **angles do not change when uniformly scaling up**
(only the linear dimensions do, so pipe sizes and similar off-the-shelf
hardware can stay the same size at the new scale). And because a uniform
10% **linear** enlargement increases **sail area** (and hence plywood-panel
area) by significantly more than 10%, a concrete material problem follows:
at the stock size, the hull's **bottom panel width already equals a full
sheet of plywood**, so widening it by even 10% (about 4 extra inches) pushes
the bottom panel **wider than a standard 4×8 ft sheet**, forcing a
seamed/joined bottom panel.

[Chris Becker](/people/chris-becker.md), building
[Walden](/boats/walden.md), confirmed the plywood concern with a practical
data point: at a **110%** scale, the **side panels** still just fit within
two 8 ft sheets of plywood, but the **bottom panel** is not wide enough at
110% to fit a standard sheet — though, as he put it, "ply is cheap,"
making a seamed bottom panel an acceptable trade-off rather than a
dealbreaker.

### Scaling the sail area correctly (square-root method)

Because a linear enlargement of every sail dimension over-enlarges the
sail's **area** (area scales with the *square* of the linear factor), a
**100 → 110 sq ft** sail-area increase needs a separate correction: take the
**square root of the target area** (√110 ≈ 10.49, rounded to 10.5) to find
the side length of an equivalent square of the new area (10.5 × 10.5 =
110.25 sq ft), then apply that same scaling logic to each side of the actual
sail by conceptually dividing it into squares. This gives approximate
resulting dimensions for a Paradox sail enlarged this way (original units,
presumably mm):

| Sail edge | Original | Scaled (~10% area increase) |
|---|---|---|
| Foot | 3350 | 3514 |
| Luff | 2850 | 2989 |
| Head | 2600 | 2727 |
| Leech | 3500 | 3671 |

The full triangle-area computation needed to verify these figures precisely
(a lugsail's area is the sum of two triangles) was not carried out; they
stand as a close approximation. The sail-design software **SailCut**
(`sailcut.com`) is available as an alternative resource for working out
enlarged sail dimensions directly.

A real-world comparison point for 10%-scale sail area: [Little
Cruiser](/matt-layden/little-cruiser.md)'s sail is about 120 sq ft on a
15'1" hull — close to a 10%-stretched Paradox's dimensions — and, per
[Dave Bolduc](/people/bolduc/dave.md), who has sailed both boats,
considerably more complex to build than Paradox's; see [Little
Cruiser](/matt-layden/little-cruiser.md) for the full sail dimensions and
assessment.

## Pete Hodges's 10% stretch: "Paradox 1.1"

[Pete Hodges](/people/pete-hodges.md) built a fully stretched Paradox at the
1.1× scale rather than pursuing piecemeal headroom modifications (see
[crew size and cabin fit](/operations/crew-size-and-fit.md) for the headroom
alternatives considered and set aside — lowering the sole, steel-strap
ballast, raising the cabin roof). Under the project name "Paradox 1.1," the
build confirmed the 10% upsizing and worked through the practical problem
already flagged above: at 110% scale the **bottom panel** no longer fits a
standard 4×8 ft sheet of plywood without the chine-log material added. Two
layout options were considered — scarfing extra material onto each side of
a 4×8 sheet to provide for the chines, or scarfing two ~2'6" × 8' sections
together lengthwise to form the portion of the bottom exceeding 4 ft.

The favored approach scarfs the edges only, with a further refinement:
rather than a true scarf, a simple **butt-block-type addition** suffices,
since the chine-runner area has to be built up with solid timber
regardless — the added pieces are small enough to offer little resistance
to bending even if merely edge-glued to the main bottom panel. As a
practical assembly aid, a strip of 1/4 in plywood can be temporarily
screwed across the joint to hold it flat until timber is fitted on the top
side after installation, then removed before final-finishing the bottom.
This directly extends the
[panel layout and nesting](/construction/panel-layout.md) guidance (which
already documents plywood-fit problems at 100% scale) to the enlarged-scale
build.

Pete Hodges's 10%-scale "Paradox 1.1" is the clearest instance on record of
a builder actually beginning construction at a stretched scale, rather than
only discussing the idea — see [Pete Hodges](/people/pete-hodges.md) for
further build reports as they appear.

## Metal chine-runner shoes as ballast/armor — a materials tangent

In the course of the "Paradox 1.1" build, a speculative idea was floated:
fitting a **steel shoe on the bottom** — a **1/4 in steel plate rolled to
the radius of the boat's deepest point** — reasoning that this would put
ballast weight exactly where it is wanted, and, if the plate extended all
the way to the edge of the
[chine runners](/chine-runners/construction.md), would
also brace them structurally.

This prompted a materials-research tangent into facing the chine runners or
hull bottom in metal, both for ballast placement and as armor/antifouling.
Candidate materials researched include lead, ferrocement, steel, and
copper-nickel plate, with comparative cost and strength figures (Cor-Ten
steel at $0.35/lb and 16 ksi yield versus 90/10 copper-nickel at $12.50/lb
and 25 ksi yield); 3M 5200 is recommended as the fastening method for
sheathing ply, with galvanized epoxy-bedded fasteners added for a full metal
panel. See [Mat ("mat_man22")](/people/mat-man22.md) for the full detail. No
metal-clad chine runner was ever built or tested; the idea remains a
materials tangent. A separate observation anticipates the bilge-keel debate
below: keels built of ferrocement or lead (rather than Paradox's plywood
[chine runners](/chine-runners/construction.md)) could
let a hull heel to a more vertical angle.

(For how the stock, plain-timber chine runners are actually built — as
opposed to this metal-shoe alternative-materials tangent — see
[chine runner construction technique](/chine-runners/construction.md).)

## Why the chine runners stay, and bilge keels don't fit Paradox

The case against modifying Paradox's underwater shape toward bilge keels
rests on Paradox being a purpose-built, unique micro sailing system that has
already proved itself at sea — a would-be modifier is better served looking
to another design entirely than compromising this one. The reasoning:

- Bilge keels would add **drag**, slowing the boat, and would need **extra
  internal structure** to mount.
- A bilge-keeled hull would **draw more water when heeled** and show **more
  leeway** — whereas photos taken looking aft while under sail show minimal
  leeway, evidence the
  [chine runners](/chine-runners/windward-performance.md)
  "really work."
- Paradox's **flat-bottomed hull shape is "really wrong" for bilge keels**;
  a chine-keel boat would suit the purpose better if bilge keels were
  wanted.
- A bilge-keeled boat would be **much harder to launch from a trailer**
  than a flat-bottomed hull like Paradox.
- On the metal-shoe idea, the underlying motive (antifouling? stability?
  bottom protection?) matters: the UK product **"Copperbot"** — an
  epoxy/copper antifouling coating claiming roughly 10 years of protection —
  achieves copper's antifouling benefit without adding hull weight or
  structure.

### Chine-runner curvature and drag

Paradox's chine runners are shaped as they are because, being so long, they
are **curved to follow the hull's shape** (a design detail illustrated in a
sketch at `http://home.triad.rr.com/lcruise/Sketch1.htm`). If the runners
could be built **without the curve**, they would have **less drag**; built
with a **better angle when the boat is heeled** (ideally straight up and
down at the heel angle actually sailed), they could be made **smaller** and
would have even less drag. Paradox is, on this assessment, **"by far the
strongest 14 ft sharpie"** seen to date, which addresses any concern about
the extra internal structure bilge keels would need. Matt Layden's own
longer-chine-runner trial (see
[chine runners and windward performance](/chine-runners/windward-performance.md))
reads as an attempt to **improve on an already-good design**, not a sign
the stock runners were deficient.

### How the chine runners work at heel

The chine runners' function is not lateral resistance in the keel sense but
acting as a **fence** that stops water breaking away from the hull sides and
running underneath it — the primary cause of leeway on a flat-bottomed
hull. Fitted chine runners keep the water running along the hull sides
instead of slipping under the bottom, and on this theory should function at
**any angle of heel**.

A direct empirical test was proposed to settle the comparison: sailing
[Paradox](/paradox.md) and [Little Cruiser](/matt-layden/little-cruiser.md)
(with her centerboard raised) together on a reach, to see how much
difference the chine runners actually make relative to a raised
centerboard. [Dave Bolduc](/people/bolduc/dave.md), who has sailed both
boats extensively, offers the closest real-world data point: over two and a
half months sailing together, he and Matt Layden **never noticed an
appreciable downwind speed difference** between Little Cruiser and
Paradox, but in **shallow water (under 18 in)** Paradox had a **definite
windward advantage** over Little Cruiser, because Little Cruiser's
centerboard could not be lowered deep enough to be effective — support for
the chine runners' practical value in the very shallow water Paradox is
designed for.

Enlarging Paradox to fit a large sailor's body, rather than for speed or
headroom, is covered in full at
[enlarging Paradox for a tall/heavy sailor](/design/variants/enlarging-for-a-large-sailor.md),
including a from-scratch 16 ft stitch-and-glue redesign,
**[Paramour](/design/variants/paramour-design.md)**.

## Virtual remodelling: Photoshop concept sketches and a 20-footer

A speculative, purely visual exercise explored reshaping Paradox's stern: a
**Photoshop "virtual remodelling"** of the Paradox — based on a photograph
of "[Whisper](/boats/whisper.md)" — aimed at making the stern less of a
flat wall to breaking waves from astern. A second remodelling followed the
same day.

The exercise surfaced a genuine design interest beyond the visual tweak: a
**20 ft** (or, per an unconfirmed secondhand claim, **23 ft**) enlarged
Paradox capable of longer open-ocean passages, drawing enthusiastic
agreement from an established Paradox owner ("I really like the Idea of a
20 ft Paradox!!"). The 23 ft figure — attributed secondhand to
**[Dave and Mindy Bolduc](/people/bolduc/dave.md)** having "a first draft"
on their website — is well beyond any stretch percentage otherwise
discussed for Paradox, and is an unconfirmed claim; no corroboration or
design work on either figure is on record.

## Scaling Paradox to 18-20 ft, and the bilge-keel question revisited

Whether Paradox could be **scaled up indefinitely** — to an **18-20 ft**
boat — without hurting her performance, assuming ballast, sail plan, and
other factors scaled with the hull, was answered from several angles.

Chine runners are still a **relatively new, experimental** concept —
"every new design which uses them is somewhat of an experiment" — probably
workable on **sharpies with plenty of rocker and ballast**, though few naval
architects focus on the innovation, so a builder wanting a larger
chine-runner boat is effectively experimenting on a scaled-up hull form of
their own. The concept is judged likely to **work** on larger boats, though
no example has actually been built and sailed at that size; four
**larger sharpie designs** serve as reference points for what such a hull
form might look like at bigger scale: Parker Marine's "Shegret" 28 and
"Exuma" plan pages, an "islesdesign" Liberdad page, and B&B Yacht Designs'
Princess 26. For the self-righting side of the question, see
[blue-water suitability and comparison to Sven Yrvind's boats](/design/blue-water-suitability.md)
for the fullest discussion on record of Paradox's self-righting claim and a
rival designer's own bilge-keel/capsize concern, and the bilge-keel
argument above for the case against bilge keels specifically.

This scaling work has already been attempted directly: a set of lines for
an enlarged Paradox, independently praised as "pretty nice," ties directly
into the same from-scratch **"Paramour"** redesign (see
[Paramour](/design/variants/paramour-design.md)) referenced elsewhere on
this page.

A more technical scaling rule holds that, as a **general rule**, a hull can
be scaled **±10% in length only** without complication; beyond that, "it
gets much more complicated" and a professional designer should be
consulted. For a larger scale, a rule from Lars Larsson's book *Principles
of Yacht Design* applies — scale **length by 1.5** and **beam/freeboard by
1.33** — with a caution that for chine runners specifically, a design
should **not** go too beamy, since the runners depend on the boat achieving
the correct amount of heel to work properly (stability rises with the
**cube** of the beam). As a general seaworthiness rule, an **externally
ballasted** boat is more seaworthy than one with internal ballast, and a
**dory** hull more seaworthy than a ballasted sharpie — with Jay Benford's
**26 ft bilge-keeled dory** and a hoped-for 23 ft "Sourdough" version, and
Benford's smaller **"HAPPY" 14 ft cruiser** design, offered as reference
points.

Consistent with the established figures above, the list's conclusion on
scaling holds: length can safely be extended **up to 10%**, keeping other
dimensions the same. On self-righting, a **graph, either with the plans or
with Don's articles**, shows that a correctly ballasted Paradox will
**self-right from 165 degrees** of heel — meaning only a 15° window is
stable upside down. This is the first record of the **165°
self-righting figure appearing on a builder's own plans/articles**
paperwork, independently corroborating the same number given years later on
microcruising.com (see
[weight, ballast, and displacement](/design/weight-and-ballast.md)
and
[blue-water suitability](/design/blue-water-suitability.md)).

Jay Benford's dory design also drew a comparison from a keelboat owner's
perspective: a used fiberglass Tanzer 28 (first encountered in Annie Hill's
book *Voyaging on a Small Income*) is "fast and seaworthy but not in 3' of
water" — an oblique nod to Paradox's own shoal-draft appeal. Separately, the
general-seaworthiness question drew a mention of an 18 ft 1979 Cape Dory
Typhoon and praise for Paradox's flat bottom as "a great feature" — see
[Paradox building plans — a fifteenth recurrence](/references/building-plans.md)
for the fuller exchange, which really continues the "buy Paradox plans"
thread rather than the scaling question itself.

Pete Hodges's 10%-scale "Paradox 1.1," begun in January 2002, remains the
closest the archive comes to a completed stretched build.

## No official larger plans exist

No larger-than-14ft Paradox plan set has ever been published — a question
newcomers ask repeatedly (most recently a prospective US builder wanting more
room for two, see [building plans](/references/building-plans.md#source-and-cost)).
Builders wanting more length or interior room are left to scale the stock
plans themselves using the methods on this page, or to consider
[Little Cruiser](/matt-layden/little-cruiser.md) instead, which likewise has
no formal plans of its own.

Because the stock plans are drawn in **metric**, scaling them up is
straightforward arithmetic: increasing every dimension by **15%** still
keeps the parts nested within two sheets of plywood while opening up enough
room for a two-person berth without crowding the cabin. Separately, Matt
Layden himself gave the "all clear" for scaling the boat **20%** on the same
scantlings, with worked figures posted to the Files section under "larger
paradox" — consistent with the 15-20% enlargement range already established
elsewhere on this page.[61][62]

## Wanting something bigger than Paradox: Little Cruiser, and Matt's own unrealized larger-sharpie idea

The enlargement question is sometimes framed from a different angle
entirely: Paradox as **"just too small,"** with the interest instead in
**[Matt Layden](/matt-layden/biography.md)'s** 15'2" sibling design,
[Little Cruiser](/matt-layden/little-cruiser.md) — or something marginally
bigger (15'11" would suit) — raising the question of whether Little
Cruiser plans might ever become available, how hard it would be to design
a Layden-style sharpie from scratch, or how to take a Paradox and increase
it to Little Cruiser size.

**No real plans were ever drawn up for Little Cruiser** (see
[Little Cruiser — no plans exist](/matt-layden/little-cruiser.md)), though
**[Dave Bolduc](/people/bolduc/dave.md)** has some basic measurements Matt
gave him personally. In the Bolducs' experience, **Little Cruiser is not
that much bigger than Paradox**, since she too was designed fundamentally
as a **solo boat**; the Bolducs are simply, in Dave's words, "used to
squeezing into small spaces like tents, micro-cruisers and compact cars for
long periods of time." The concrete recommendation for a builder wanting
more room: **scale the 4.2 m Paradox up 10-20%**, yielding a boat **4.6 m to
5 m** long. As an alternative to scaling Paradox at all, an **existing
larger design** — the **NIS18**
(`duckflatwoodenboats.com/OldPages/nispix/nis18.htm`) — is one possibility.

Dave Bolduc has **talked to Matt Layden several times about drawing up a set
of plans for a larger sharpie**, but Matt "hasn't come up with anything that
I am aware of" — with an admiring aside characteristic of Matt: "the kind of
person who accomplishes amazing things quickly when he is in the mood...
Still you never know." This is the clearest confirmation on record that a
**larger Layden sharpie has been discussed directly with Matt himself**,
distinct from the purely speculative proposals (the 20 ft/23 ft "virtual
remodelling" idea and the from-scratch "Paramour," both above) — and that,
as of this exchange, nothing had come of it.

A real-world scaling data point independent of Matt Layden's rule: a
**naval architect** has advised that scaling a small boat up **~10%** —
whether length alone, or length and beam together — has "very little effect
on the character of the boat." Two sharpies have been **built** on that
principle with good results; a **kayak building book** describes a formula
(possibly related to a sine wave) for spreading out a design's stations to
preserve consistent flow around the hull when scaling. The overall verdict:
**"I think you could scale up a Paradox to little cruiser size with no
problem."**

Pete Hodges's 10%-scale "Paradox 1.1" remains the closest the archive comes
to a completed stretched build, and Matt Layden's own larger-sharpie idea
remains, in Dave Bolduc's words, something that simply "hasn't come up with
anything."

### "Jeff UK" gives concrete scaled-up dimensions

One direct numeric answer on record (from a correspondent identified only as
"Jeff UK," possibly but not confirmed to be the same person as the
established [Jeff (UK, "doryman_uk")](/people/jeff-doryman.md)): scaling
Paradox up "all round" produces a boat **15' 10" LOA x 4' 7" beam**, just
over **10 in draught**, and a displacement **around 1,600 lb** — figures
close to, but somewhat larger than, Little Cruiser's own particulars
(15' 2", 4' 7" beam, 9 in draft, 1,600 lb displacement; see
[Little Cruiser](/matt-layden/little-cruiser.md#design-particulars)). A
same-day correction brought the scale factor to **1.15**, not a plain
"all round" scale-up, bringing the figures roughly in line with the
**10-20%** stretch range recommended above.

This is the only concrete, fully worked set of scaled dimensions — LOA,
beam, draft, and displacement together, rather than a single ratio or rule
of thumb — produced for this enlargement question, though whether the
figures came from drawings or a by-hand calculation is not stated, and no
boat built to them is recorded. Whether "Jeff UK" is the same person as
Jeff (UK, "doryman_uk") — who separately proposed his own from-scratch 16
ft "Paramour" redesign (see
[Paramour](/design/variants/paramour-design.md)) and had already been
identified as the list's resident scaling expert — remains an open
question; no linking detail (shared boat name, "that's me"
cross-reference) resolves it, so the two are tracked separately per the
project's standing identity-merge caution.

### Sharpie hull-form variants and design literature

Whether a sharpie's underwater profile is simply a smooth flat-bottomed arc
with flared sides opens onto the broader sharpie-design literature: Paradox
falls into the "classic" sharpie shape, but other sub-types exist —
**Modified/NonPareil sharpies** (a slight V bottom) and **Huntington
sharpies** (a slight round to the bottom, both in length and beam) —
developed to reduce pounding in short, steep seas while keeping the type's
inexpensive construction. **Reuel B. Parker's** *The Sharpie Book* covers
these variants; Paradox herself is unlikely to pound much, given her
relatively deep-sitting, heavily rockered bottom.

Elaborating on sharpie hull shape from Parker's book: the bottom's
fore-and-aft arc often flattens toward the stern (with the lowest point
somewhat forward of amidships, part of the stern sometimes riding clear of
the water), and side flare is commonly specified at **3½-4 in per foot of
rise**, tapering to vertical at the bow.

Parker's other relevant title is not a sequel but was written **four years
earlier**: ***The New Cold-Molded Boatbuilding* (from lofting to
launching)** (hardbound 1990, paperback 1992, ISBN 0-8742-358-X). It
describes a cold-molded method — two layers of planking run at 45 degrees
to each other to build up an arched bottom, typically on **35-50 ft**
boats — a technique with results comparable to strip-planking applied on a
small skiff or kayak, at about two days build time for the bottom. This
remains a bibliographic/technique tangent, disconnected from Paradox's own
construction, but grew directly out of the scaling discussion above.

### Comparing Paradox's lines to Bolger's Jessie Cooper, and whether chine runners scale to 25 feet

A direct lines comparison put Paradox, Little Cruiser, and **Phil Bolger's
Jessie Cooper** side by side, finding Jessie Cooper's underwater shape
similar enough to both Layden designs to raise the chine-runner scaling
question again, this time at a genuinely large size: whether a **25 ft**
hull on these lines could sail to windward on chine runners at all, given
Bolger's own account of a centerboard jamming in thin water on the
similarly-shaped hull. A centerboard mounted off to one side of the
walkway — sketched among Matt Layden's own concepts for a larger cruiser —
was floated as a possible alternative to chine runners at that scale.

The same hull lineage traces through Bolger's own design history, using
**Chuck Merrell's** Jessie Cooper-derived redesign (built with a MICRO-type
keel) as a cautionary data point: that boat's 480 lb of internal ballast
proved insufficient, needing 1,200 lb to bring her near her designed
waterline — suggesting that immersing a hull like this deeply enough to
make chine runners effective would need enough added weight to risk
digging the bow in instead. Bolger's own response to that shortfall was to
abandon the type: he moved to **leeboard, water-ballasted designs**
instead, first the **Martha Jane** and then the **AS19** (internal ballast,
a fast but oddly scoop-bowed hull), followed by the **AS29** (swinging
bilge keels) and **AS38** (centerboard). Bolger's later designs converge on
a centerboard set well forward with a large rudder — the same general
arrangement as **[the "BRIS Paradox"](/boats/bris-paradox.md)**. No
chine-runner boat at 25 ft scale is recorded as ever having been built to
test the question directly.

## A UK-scale stretch proposal (16 ft, same beam/draft/displacement)

A larger Paradox has also been proposed around a UK-specific detail:
because the UK has **no equivalent of the US "fourteen foot rule"** (the US
trailering/registration length threshold that constrains Paradox's stock
13'10" LOA), designing a **new 16 ft hull from scratch** — rather than
scaling the existing one — while keeping the **beam, draft, and
displacement approximately the same** as stock and reusing Paradox's **rig
as drawn**, would yield a boat an estimated **half a knot faster**. No
design work beyond this proposal is recorded.

## A Scandinavian newcomer's scaling question

The now-familiar scaling question recurred afresh from a **Norwegian**
newcomer in December 2003: whether the boat could be scaled up **20%**
(longer, wider, and higher together), what problems that might cause, and
whether 14 ft was really large enough for two people sailing — alongside
general questions about build time and cost. The answer pointed to the
group's **"Larger Paradox"** files folder, which already gives figures for
a 20% enlargement and records that **Matt Layden himself feels it would
work fine** — consistent with the established scaling guidance above,
though at the upper edge of the 15-25% range the relayed scantling rule
allows before scantlings must be rethought from scratch. The clearest
**build-time generalization** on record: cost varies chiefly by location,
but most builders finish in about a year of part-time work, with finishing
typically taking as long as the building itself. A network of
**Scandinavian builders** — in Norway, Denmark, and Sweden, working in
plywood and epoxy — is a better resource for local cost and sourcing
questions than the archive generally; a builder near **Oslo** had also
built a 25 ft schooner.

## Enlarging for a tall sailor, and three named stretch methods

The scaling question recurs for taller sailors specifically: a prospective
builder over 6 ft tall, worried about cabin room in the stock 14-footer,
asked in January 2004 whether a straight 1.2× (20%) enlargement was really as
simple as multiplying every dimension by the same factor. At 6'1", the stock
interior is comfortable enough, and the larger-Paradox numbers already
circulating in the group's files section cover exactly this case. A
practical, two-up-cruising argument also favors going bigger: a solo Paradox
owner cannot invite a visitor aboard without both parties getting rained on,
since there is no room to ask a guest inside without closing the hatch, and
two-up cruising in humid climates (as found aboard
"[Zero](/boats/aussie-paradox.md)") is uncomfortable at the stock size —
though this is minor nit-picking against a design that "cannot be improved
for what it was designed to do."

The fullest breakdown on record of *named* stretch methods, distinct from the
single-factor scaling rule established above, cautions that **any of them
should stay under about a 10% enlargement** before the boat's proportions
stop being "in harmony" and a builder is really designing a new boat:

- **"Big Paradox"** — the already-circulated larger-Paradox lines (see
  above), giving a boat closer in feel to [Little
  Cruiser](/matt-layden/little-cruiser.md), suited to two people.
- **"Stretch Paradox"** — lengthen only, by spreading out the station
  spacing uniformly, keeping the sail plan, mast, and fittings close to
  stock. A longer waterline drives more easily under the existing rig
  (except possibly in very light air, from the added wetted surface) and
  would be faster in moderate-to-heavy air; displacement grows only
  linearly rather than with the cube of the scale factor, making this a
  smaller boat overall than "Big Paradox."
- **"Pug Paradox"** — a non-uniform stretch, elongating the hull more
  amidships than at the ends (for example 1", 2", 2", 1" between
  consecutive stations, reversing past amidships, in a ratio such as
  1:2:3:3:2:1), a technique common in kayak design (credited to Eric
  Schrade of Guillemot Boats) for fining a hull's ends while keeping the
  sheer line fair, so long as the increments follow a regular pattern and
  stay a small fraction of the station spacing. Applied to Paradox it would
  give the bigger main cabin of "Big Paradox" in a shorter overall length,
  with performance falling between the stock and "Stretch" versions.

## A group-level enlarged Paradox under consideration

Beyond these individual builders' scaling proposals, the archive records
that the wider building community was at one point (late November 2003)
"in the progress of considering developing plans for a somewhat enlarged
version of Paradox." No further detail — dimensions, a target enlargement
factor, or who would draw it — is recorded.

## "Big Cruiser": Matt Layden's own unfinished enlargement cartoons

Separately from any list-side scaling proposal, Matt Layden made his own,
still-unpublished attempt at a stretched/enlarged Paradox, informally named
**"Big Cruiser."** Cartoons for it exist in the `microcruising` Yahoo
group's files section (folder `Big%20Cruiser/`) but never reached final
plans; see [Matt Layden (biography) — asides and
footnotes](/matt-layden/biography.md#asides-and-footnotes).

## A recurring question: has anyone actually built a scaled-up Paradox?

Even after years of scaling rules, worked dimensions, and Pete Hodges's
"Paradox 1.1," the underlying question recurs in its simplest form: has
anyone actually gone ahead and built an enlarged Paradox sized to sleep two
comfortably, and if so, how did it turn out? No further completed larger
build beyond Pete Hodges's 10%-scale "Paradox 1.1" is on record in answer.[65]

## A steel enlargement idea, and the case against it

Following a renewed call to enlarge Paradox by 20% (see
[blue-water suitability — a 2004 revisiting: Paradox against Sven Yrvind's
"Sofia"](/design/blue-water-suitability.md#a-2004-revisiting-paradox-against-sven-yrvinds-sofia)),
[Jack Gardiner](/people/jack-gardiner.md) — already the archive's leading
voice for building a whole Paradox hull in steel (see
[aluminum and steel Paradox (speculative)](/design/aluminum-construction-idea.md)) —
floated building his next, larger "ultimate cruiser" in steel, undecided
between a **16 ft and a 19 ft** hull.[63]

The enlargement idea itself found support — carrying Matt Layden's
"apparent, tacit blessing," given how freely the designer's own scaling rule
had already been shared — but steel was argued against as the material at
these larger sizes: the added weight throughout the structure would work
against a fresh look at weight distribution, displacement, and ultimate
stability that a stretched design deserves. If Matt Layden himself could be
drawn into such a project, the result might be a genuinely tough,
coastal-cruising "world beater" — worth the effort regardless of which
material was ultimately chosen.[64]

## A 17 ft Paradox variant and a related "KS2" design, in development

A **17 ft Paradox variant**, together with a related design referred to as
**"KS2,"** was reported in active development by a boat-design professional
in mid-2005, with "final touches" being put on the details.[66] The work
drew visible interest from the wider list — one correspondent framed a 17 ft
Paradox as squarely on target for what he had personally been aiming for,
though he judged adapting the stock 13'10" plans himself beyond his own
skill, and asked that progress be shared with the group as it develops.[67][68]

The design was posted in full as the **"KSDuo,"** an enlarged, two-person
microcruiser expanding both the solo **KS2** and the Paradox out to
**17 ft LOA with a 66 in beam overall**, with a two-person cockpit and
sleeping/microcruising accommodation for two adults with "a modicum of
comfort." A second variant, the **KSDuoX**, traded 20.5 in of extra cabin
length for a reduced cockpit — enough for two adults, though "they probably
won't be sitting on the same side at the same time" unless particularly
small. Design displacement is **2,300 lb**, with strip-built Western Red
Cedar (or another suitable wood) construction and epoxy/glass laminate on
both sides.[69]

The KSDuo's other design features: a main cabin hatch elongated into a
raised pop-top for full standing headroom; a cockpit deck angled 3 degrees
aft and raised well above the waterline for efficient self-draining; an aft
compartment sized for a 5 hp outboard, fuel, and an aft anchor; main-cabin
side windows fitted with folding solar cells (adjustable for sun angle
underway) over screened ventilation panels, with the forward hatch and
popped-up main hatch also screened; a fully enclosed dodger/bimini/side-panel
cockpit enclosure for all-weather sailing; a remote-wing tiller worked
through stainless cables run through the aft compartment; formed bilge keels
toed in 2 degrees for upwind assistance, giving very low draft and letting
the boat dry out upright on tidal flats or beaches; a flip-up, bungee-tensioned
rudder to avoid obstacles in thin water; molded-in toe rails with built-in
scuppers along both gunwales for footing and deck drainage, doubling as
tie-off points stem to stern; and a separate, watertight forward anchor
compartment protected by a foam-filled crush zone at the bow. The rig drawn
for the design is a **gaff yawl** with carbon-fiber spars and a roller-furling
jib, balanced to sail under the full rig, jib and mizzen alone, main alone,
or any reefed combination — though the designer left the door open to other
rig types depending on a builder's own interest.[69]

# Citations

[1] Archive message page_090 (Charles Wilson, `paradoxbuilders`, 2001-11-10) — "Stretch Paradox": asks whether stretching to 16 ft is a good or bad idea, and whether anyone else has tried it.
[2] Archive message page_103 (Glen Maxwell, `paradoxbuilders`, 2001-11-18) — "Re: Stretch Paradox": relays Matt Layden's rule (multiply scantlings by the enlargement factor, 15% in Charles's case; fine to 25%, beyond which bulkhead placement/scantlings must be rethought); recommends Dave Gerr's *The Elements of Boat Strength* for scantling recommendations.
[3] Archive message page_106 (Charles Wilson, `paradoxbuilders`, 2001-11-19) — "Re: Stretch Paradox": thanks Glen, confirms the answer matched what he suspected, will review earlier posts on the topic.
[4] Archive message page_131 (Pete Hodges, `paradoxbuilders`, 2001-11-27) — "Re: Stretch Paradox": also interested in a ~10% stretch; asks whether mast height or sail area needs to increase along with hull length.
[5] Archive message page_132 (Glen Maxwell, `paradoxbuilders`, 2001-11-27) — "Re: Stretch Paradox": confirms yes, multiply everything (including sail area) by the same factor; notes the extra ~10 sq ft may not make much difference but he'd want it anyway; Paradox can reef quickly if oversailed.
[6] Archive message page_133 (Jeff Forrest, `paradoxbuilders`, 2001-11-25) — "Re: Stretch Paradox": introduces himself as new to the group, plans ordered but not yet received; also interested in a 10–15% stretch; asks whether "multiply by the factor" applies to length only or also beam.
[7] Archive message page_134 (Glen Maxwell, `paradoxbuilders`, 2001-11-27) — "Re: Stretch Paradox": clarifies that enlarging means scaling everything (not just length) to keep proportions and avoid producing a different design.
[8] Archive message page_135 (Jeff Forrest, `paradoxbuilders`, 2001-11-27) — "Stretching Paradox": thanks Glen; asks whether anyone in the group has actually stretched their Paradox, by what percentage, and how they feel about the result — no reply is recorded.
[9] Archive message page_192 (orpdh / Pete Hodges, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": proposes enlarging the whole boat ~5% for extra headroom; notes bulkheads/stem are not vertical, complicating uniform scaling; alternatives considered: lowering the sole an inch (less water ballast, less standing-can storage), steel-strap ballast (~3/16 in × 5/8 in) along the outside of the keel bottom epoxied over and faired, raising the cabin roof 1 in forward/2 in aft; estimates ~3 in more headroom forward and 4 in aft if all changes combined.
[10] Archive message page_193 (Glen Maxwell, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": simpler answer — multiply everything by 1.1 (10%, blessed by Matt Layden); resulting dimensions 15' 2 5/8" LOA, 4' 4 13/16" BOA, 9 7/8" draft, 40" headroom under the hatch (his own boat is 36 1/2"); do not enlarge chine logs/sheer clamps, already generous; recommends working in metric; method good to about 15%, beyond which consult Dave Gerr's *The Elements of Boat Strength*; mentions finishing a sea-trials write-up and a comfortable Coleman inflatable twin-size mattress.
[11] Archive message page_195 (orpdh / Pete Hodges, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": 1.1× works for height/width but not for angled parts (bulkheads, stem, roller-rigging pipe, cabin supports), which need lofting or trigonometry; sail area would increase by more than 10% under a flat 1.1× linear scaling; the stock bottom panel's width already equals a full plywood sheet, so a 10% wider hull would exceed a standard sheet's width.
[12] Archive message page_196 (Glen Maxwell, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": angles do not change when scaling up; leave pipe sizes etc. the same at the new scale.
[13] Archive message page_194 (c_i_becker / Chris Becker, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": confirms the plywood-fit concern — at 110% scale the side panels still just fit two 8 ft sheets, but the bottom panel is not wide enough at 110% for a standard sheet; "ply is cheap."
[14] Archive message page_197 (orpdh / Pete Hodges, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": asks whether anyone knows the correct method to increase the sail size (since linear scaling over-grows area).
[15] Archive message page_198 (migchelsen / Barend Migchelsen, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": points to `sailcit.com` for sail sizing (later corrected).
[16] Archive message page_199 (migchelsen / Barend Migchelsen, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": correction — the site is `sailcut.com`, not "sailcit.com."
[17] Archive message page_200 (Glen Maxwell, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": worked example scaling a 100 sq ft sail to 110 sq ft via the square-root method (√110 ≈ 10.5, 10.5×10.5 = 110.25); approximate scaled sail dimensions Foot 3514 (was 3350), Luff 2989 (was 2850), Head 2727 (was 2600), Leech 3671 (was 3500); notes the full triangle-area computation was not carried out to verify.
[18] Archive message page_201 (orpdh / Pete Hodges, `paradoxbuilders`, 2001-12-21) — "Re: Wearing the Boat": thanks Glen; decides to "give a 1.1 version a shot"; jokes about what to do with the extra space.
[19] Archive message page_202 (boldav38 / Dave Bolduc, `paradoxbuilders`, 2001-12-22) — "Little Cruiser's sail": Little Cruiser (15'1", ~120 sq ft sail) offered as a real-world comparison point for a ~10%-stretched Paradox's sail area.
[20] Archive message page_212 (orpdh / Pete Hodges, `paradoxbuilders`, 2001-12-31) — "Paradox 1.1": has decided to build a Paradox with a 10% upsizing; asks whether to lay out the enlarged bottom by scarfing extra material onto each side of a 4×8 sheet, or by scarfing two ~2'6"×8' sections together lengthwise; separately floats the idea of a 1/4 in steel shoe rolled to the deepest-point radius, doubling as ballast and chine-runner bracing (unanswered).
[21] Archive message page_220 (Glen Maxwell, `paradoxbuilders`, 2002-01-05) — "Re: Paradox 1.1": favors scarfing the edges only; suggests a butt-block-type addition instead of a true scarf, since the chine-runner area is built up with timber regardless; small added pieces offer little resistance even if edge-glued; recommends temporarily screwing a 1/4 in ply strip across the joint until timber is fitted on top, then removing it before final-finishing the bottom.
[22] Archive message page_232 (mat_man22 / Mat, `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": considered lead or ferrocement chine runners fastened with 5200, now prefers a steel shoe; notes Phil Bolger's copper-sheathed sharpies.
[23] Archive message page_233 (mat_man22 / Mat, `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": proposes copper-nickel plate as the ideal shoe material, citing Nigel Warren's *Metal Corrosion in Boats*.
[24] Archive message page_234 (orpdh / Pete Hodges, `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": asks how high the Cu/Ni cost is, where to source it, and how to fasten copper-nickel or ferrocement/steel chines to the hull.
[25] Archive message page_235 (mat_man22 / Mat, `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": answers Pete — marine.copper.org links; cost/strength figures (Cor-Ten $0.35/lb vs. 90/10 Cu/Ni $12.50/lb; 16 ksi vs. 25 ksi yield); fastening — 5200 only for sheathing ply, 5200 plus (galvanized, epoxy-bedded) fasteners for a full metal panel or metal chines.
[26] Archive message page_236 (orpdh / Pete Hodges, `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": jokes about coating the boat in gold; posts a second, contemporary (14 Mar 2001) Cu/Ni price list from Bestweld Inc. (copper $1.00/lb, nickel $8.00/lb, 90/10 alloy $1.70/lb, 70/30 alloy $3.10/lb) and pipe prices.
[27] Archive message page_239 (mat_man22 / Mat, `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": "I'm building a real gold plater" quip; suggests ferrocement/lead keels could heel more vertically than Paradox's chine runners; links an external twin-keel article.
[28] Archive message page_240 (Jeff Please / "doryman_uk", `paradoxbuilders`, 2002-01-10) — "Re: Paradox 1.1": argues against bilge keels for Paradox (drag, extra structure, more leeway/draft when heeled, wrong hull shape, poor trailer launching); questions the motive for a metal bottom shoe; cites UK "Copperbot" epoxy/copper antifouling coating (~10 years without antifouling); proposes designing a new 16 ft hull from scratch (same beam/draft/displacement, same rig) since the UK has no 14 ft trailering-rule constraint, estimating ~0.5 kt more speed.
[29] Archive message page_243 (mat_man22 / Mat, `paradoxbuilders`, 2002-01-10/11) — "Re: Paradox 1.1": explains chine runners are curved to follow the hull because of their length; a straight (uncurved) runner, or one at a better heel angle, would have less drag and could be smaller; calls Paradox "by far the strongest 14 ft sharpie" he's seen; speculates Matt's longer-chine-runner trial aimed to improve an already-good design.
[30] Archive message page_244 (Jeff Please / "doryman_uk", `paradoxbuilders`, 2002-01-11) — "Re: Paradox 1.1": addressed to "Matt" — theorizes chine runners work at any heel angle by fencing water from running under the hull (the main cause of leeway on a flat bottom); proposes sailing Paradox and Little Cruiser (centerboard raised) together on a reach to compare, and asks whether Dave Bolduc/Matt have tried this.
[31] Archive message page_594 (benoitbeauchemin / Benoit Beauchemin, `paradoxbuilders`, msgnum 595, 2002-07-27) — "Paradox virtual remodelling...": posts a Photoshop-modified image of Paradox based on a photo of "Whisper," aiming to reduce the stern's "wall"-like exposure to breaking waves; posted to the Photos folder; invites comment.
[32] Archive message page_595 (dlb / buster38801 / David Beard, `paradoxbuilders`, msgnum 596, 2002-07-27) — "Re: Paradox virtual remodelling...": "I dont mind at all," regarding the use of his boat's photo.
[33] Archive message page_596 (benoitbeauchemin / Benoit Beauchemin, `paradoxbuilders`, msgnum 597, 2002-07-27) — "Paradox virtual remodelling 2": posts a second virtual remodelling, not taken too seriously; he and friends plan to build a genuine, unmodified Paradox that winter in Montreal, Quebec, Canada, drawn to the area's abundant shallow water; separately says he would love a 20-footer based on the same design for longer passages (the Pacific, Patagonia); cites a secondhand, unconfirmed claim that Dave and Mindy Bolduc have "a first draft of a 23 foot Paradox" on their website.
[34] Archive message page_597 (David Beard, `paradoxbuilders`, msgnum 598, 2002-07-27) — "Re: Paradox virtual remodelling 2": "I really like the Idea of a 20 ft Paradox!!"
[35] Archive message page_818 (servo_bot, `paradoxbuilders`, msgnum 832, 2003-01-10) — "Scaling Paradox and Other Questions": asks whether scaling Paradox (with ballast/sailplan scaled too) to an 18-20 ft boat would hurt performance; asks whether a ballast keel or bilge keels could be added for stability/self-righting at the cost of shallow-water capability without destroying the boat's theoretical performance, and whether Paradox is self-righting as designed; attending boat-building school starting August 2003.
[36] Archive message page_820 (admin / Paul V., `paradoxbuilders`, msgnum 834, 2003-01-10) — "Re: Scaling Paradox and Other Questions": chine runners are a relatively new concept, every new design using them is somewhat of an experiment; probably works on sharpies with good rocker and ballast; few naval architects focus on this innovation; points to four larger sharpie design websites (Parker Marine "Shegret" 28 and "Exuma," an islesdesign "Liberdad" page, B&B Yacht Designs Princess 26); believes the chine-runner concept will work on larger boats but has not seen an example.
[37] Archive message page_821 (lwhited / Larry Whited, `paradoxbuilders`, msgnum 835, 2003-01-10) — "Re: Scaling Paradox and Other Questions": points to Jeff (UK) as already working on scaling up Paradox, having posted a nice-looking set of lines; directs servo_bot to Jeff's partially-obscured e-mail in message 416 to ask directly; expects strong interest in a proven scaled-up version; would be happy to build the prototype or the next one; judges Don (Elliott) most qualified to do the initial build.
[38] Archive message page_822 (mat_man22 / Mat, `paradoxbuilders`, msgnum 836, 2003-01-10) — "Re: Scaling Paradox and Other Questions": general rule is ±10% length scaling without complication, beyond which a designer should be consulted; if forced to scale larger, cites Lars Larsson's *Principles of Yacht Design* — scale length by 1.5, beam/freeboard by 1.33; warns against too much beam for chine runners, since they need the correct heel angle to work (stability rises with the cube of the beam); as a general rule an externally ballasted boat is more seaworthy than an internally ballasted one, and a dory more seaworthy than a ballasted sharpie; points to Jay Benford's 26 ft bilge-keeled dory and a hoped-for 23 ft "Sourdough" version.
[39] Archive message page_823 (mat_man22 / Mat, `paradoxbuilders`, msgnum 837, 2003-01-10) — "HAPPY 14' Cruiser (Benford)": shares a link to Benford's new web page for the "HAPPY" 14 ft cruiser design, without further comment.
[40] Archive message page_824 (openboat / Alastair, `paradoxbuilders`, msgnum 838, 2003-01-10) — "Re: Scaling Paradox and Other Questions": recalls the list's earlier conclusion that length can safely be extended up to 10%, other dimensions unchanged; received a graph, either with the plans or with Don's articles, showing a correctly ballasted Paradox self-rights from 165 degrees of heel (only 15 degrees stable upside down); will take this on trust rather than test it; "Hoping for calm nights."
[41] Archive message page_829 (admin / Paul V., `paradoxbuilders`, msgnum 843, 2003-01-10) — "Re: Scaling Paradox and Other Questions": likes Mat's Benford-dory reference, first seen in Annie Hill's *Voyaging on a Small Income*; owns a used fiberglass Tanzer 28 keelboat, not a dory, as something similar; would also like something for shallow water, since his own boat is "fast and seaworthy but not in 3' of water."
[42] Archive message page_928 (whisper / David LeBlanc, `paradoxbuilders`, msgnum 943, 2003-04-29) — "Lil Cruiser Plans": finds Paradox too small, more interested in Lil Cruiser or something marginally bigger (15'11" would suit); asks whether Lil Cruiser plans might ever be available, how hard it would be to design a Layden-style sharpie from scratch, or to enlarge a Paradox to Lil Cruiser size.
[43] Archive message page_929 (mbolduc / "boldav38" / Dave Bolduc, `paradoxbuilders`, msgnum 944, 2003-04-30) — "Re: Lil Cruiser Plans": no real plans were ever drawn for Little Cruiser, though he has basic measurements Matt gave him; LC isn't much bigger than Paradox, both fundamentally solo boats; recommends scaling Paradox 10-20% (4.6-5 m) or building an existing larger design (points to the NIS18); has talked to Matt Layden several times about drawing up plans for a larger sharpie, but Matt hasn't come up with anything yet — "Still you never know... Matt's the kind of person who accomplishes amazing things quickly when he is in the mood."
[44] Archive message page_930 (LJGeib / Larry ("LJGeib"), `paradoxbuilders`, msgnum 945, 2003-04-30) — "Re: Lil Cruiser Plans": a naval architect once told him scaling a small boat up ~10% (length alone, or length and beam) has very little effect on the boat's character; has built two sharpies on that principle and was pleased with the results; recalls a kayak-building book's station-spacing formula (thinks it's related to a sine wave) for preserving flow when scaling, will try to find it; "I think you could scale up a Paradox to little cruiser size with no problem."
[45] Archive message page_932 (apcf14 / "Jeff UK", `paradoxbuilders`, msgnum 947, 2003-04-30) — "Re: Lil Cruiser Plans": scaling Paradox up all round gives 15' 10" LOA x 4' 7" beam, just over 10 in draught, displacement around 1,600 lb.
[46] Archive message page_933 (apcf14 / "Jeff UK", `paradoxbuilders`, msgnum 948, 2003-04-30) — "Re: Lil Cruiser Plans": "Sorry Dave. I should have said scale by 1.15. I got distracted."
[47] Archive message page_934 (LJGeib / Larry ("LJGeib"), `paradoxbuilders`, msgnum 949, 2003-04-30) — "Re: Lil Cruiser Plans": Paradox falls into the classic Sharpie shape; Modified/NonPareil sharpies have a slight V bottom, Huntington sharpies a slight round bottom in length and beam, both developed to reduce pounding in short steep seas; cites Reuel B. Parker's Sharpie books (the second deals mostly with these variants); Paradox probably won't pound much given her relatively deep, heavily rockered bottom.
[48] Archive message page_935 (pathooker / Patrick Hooker, `paradoxbuilders`, msgnum 950, 2003-04-30) — "Re: Lil Cruiser Plans": studying Parker's "The Sharpie Book" intently; the bottom's fore-aft arc often flattens toward the stern (lowest point forward of amidships, stern sometimes clear of the water); side flare typically 3½-4 in per foot of rise, tapering to vertical at the bow; signs "Patrick(Alaska!) << an avid Sharpie fan, hoping to build a 48 footer some day."
[49] Archive message page_936 (pathooker / Patrick Hooker, `paradoxbuilders`, msgnum 951, 2003-04-30) — "Re: Lil Cruiser Plans": "Reuel as written a second book!!!!! What's the title? Where can I find it?"
[50] Archive message page_937 (LJGeib / Larry ("LJGeib"), `paradoxbuilders`, msgnum 952, 2003-05-01) — "Re: Lil Cruiser Plans": Parker's "second" book was actually written four years before The Sharpie Book — "The New Cold-Molded Boatbuilding" (1990 hardbound/1992 paperback, ISBN 0-8742-358-X), found at Powell's City of Books, Portland OR; describes the 45-degree-crossed double-plank cold-molded method for 35-50 ft boats; has used a similar strip-planking method himself on kayaks and once on a small skiff with good results, about two days to build the bottom.
[51] Archive message page_1466 (arvent / "Nels", `paradoxbuilders`, msgnum 1486, 2003-11-30) — "Welcome New Members": full text and citation at [people/glen-maxwell/list-founder-and-moderator.md](/people/glen-maxwell/list-founder-and-moderator.md#welcoming-newcomers).
[52] Archive message page_1486 (fredrilu / Fredrik, `paradoxbuilders`, msgnum 1506, 2003-12-09) — "scaling the boat": new member from Norway, hopes to build during the next year; asks whether the boat can be scaled 20% bigger (longer, wider, higher) and what problems might arise; wonders whether 14 ft is a little small for two; asks how much time and money building usually takes.
[53] Archive message page_1487 (arvent / "Nels", `paradoxbuilders`, msgnum 1507, 2003-12-09) — "Re: scaling the boat": welcomes Fredrik; points to the "Larger Paradox" files folder, which gives figures for a 20% increase and records that Matt Layden feels it would work fine; points to other folders on materials and to links-section resources; building time depends on skill/time/tools/space, finishing typically takes as long as building, most builders take about a year part-time; cost depends heavily on location; recommends contacting local builders, naming Norway, Denmark, and Sweden as countries with builders working in plywood and epoxy; asks what part of Norway Fredrik is from and whether he is near Oslo, recalling a fellow there who built a 25 ft schooner and used to post to the group.
[54] Archive message page_1489 (arvent / "Nels", `paradoxbuilders`, msgnum 1509, 2003-12-10) — "Re: scaling the boat": "I sent you some information direct to your email address."
[55] Archive message page_1841 (jasonstancil / "smithriverranger" / Jason Stancil, `paradoxbuilders`, msgnum 1864, 2004-01-21) — "enlarged paradox?": has been considering a build for two years; asks whether anyone has actually built or begun a scaled-up Paradox, and whether a straight 20% (1.2×) dimension multiplication is really as simple as it sounds; at 6'2" tall, worries about being cramped in the stock 14-footer.
[56] Archive message page_1842 (kd7ixk / "DC", `paradoxbuilders`, msgnum 1865, 2004-01-21) — "Re: enlarged paradox?": at 6'1", 225 lb, has plenty of room in the as-designed interior; points Jason to Glen Maxwell's larger-Paradox numbers already posted in the files section.
[57] Archive message page_1844 (arvent / "Nels", `paradoxbuilders`, msgnum 1867, 2004-01-22) — "Re: enlarged paradox?": about 5 in shorter than Jason, shares some of his reservations; recalls Glen's article describing a visitor who had to be talked to in the rain since there was no room to invite him aboard with the hatch closed — not a problem in Florida but relevant living mostly in Canada; quotes Andrew Graham's "Zero" cruise report that humid weather made two-up cruising uncomfortable; concludes a larger boat would offer more two-up possibilities without much added investment, while stressing the design itself "cannot be improved for what it was designed to do."
[58] Archive message page_1845 (LJGeib / "Larry", `paradoxbuilders`, msgnum 1868, 2004-01-21) — "Re: enlarged paradox?": names and describes three stretch methods, cautioning against more than about a 10% enlargement for any of them — "Big Paradox" (the already-circulated larger lines, closer in feel to Little Cruiser, a nice 2-person boat), "Stretch Paradox" (lengthen only, spreading the stations, keeping the standard sail plan/mast/fittings, easier to drive on the longer waterline except possibly in light air, faster in moderate/heavy air, displacement growing linearly), and "Pug Paradox" (a non-uniform stretch concentrated amidships, in inch ratios such as 1:2:3:3:2:1, 1:2:4:2:1, or 1:4:2:4:2:4:1, a technique from Eric Schrade's kayak-building book, giving a bigger cabin in a shorter length with performance between the standard and stretched versions); the "Pug" name is a misnomer coined by a friend to annoy him.
[59] Archive message page_1964 (paull01 / "paull01" / Paul, Seattle WA, `paradoxbuilders`, msgnum 1987, 2004-03-15) — "Lines Comparison": has traced the lines of Paradox, Little Cruiser, and Bolger's Jessie Cooper, uploaded to the "Larger Paradox" files folder; finds Jessie Cooper's lines similar to both Layden designs; at 25 ft, wonders how such a hull would sail with chine runners, noting Bolger's own complaint of a centerboard jamming in thin water; floats a centerboard off to one side of the walkway, as sketched among Matt Layden's own concepts for a bigger cruiser, as a possible alternative.
[60] Archive message page_1965 (arvent / "Nels", `paradoxbuilders`, msgnum 1988, 2004-03-15) — "Re: Lines Comparison": points to Chuck Merrell's website on his own Jessie Cooper-derived redesign, built with a MICRO-type keel; its 480 lb of internal ballast proved insufficient, needing 1,200 lb to reach the designed waterline, suggesting chine runners at this scale would need enough added weight to risk digging the bow in; recounts Bolger's own move away from the type to leeboard/water-ballasted designs — the Martha Jane, then the AS19 (internal ballast, fast but a "kinda weird" scoop bow), then the AS29 (swinging bilge keels) and AS38 (centerboard); Bolger's newest designs converge on a centerboard set well forward with big rudders, like BRIS.
[61] Archive message page_2221 (arvent / "Nels", `paradoxbuilders`, msgnum 2248, 2004-08-31) — "Re: New Member": since the plans are metric, scaling up is easy — increasing all dimensions by 15% still keeps the parts inside two sheets of plywood and gives room for a two-person berth without crowding.
[62] Archive message page_2222 (jasonstancil / "smithriverranger" / Jason Stancil, `paradoxbuilders`, msgnum 2249, 2004-08-31) — "Re: New Member": Matt Layden gave the "all clear" on scaling the boat 20% on the same scantlings; worked figures are posted in the Files section under "larger paradox."
[63] Archive message page_2419 (alex29 / "John Gardiner" / Jack Gardiner, `paradoxbuilders`, msgnum 2447, 2004-11-07) — "Re: Amelie": floats building his next "ultimate cruiser" possibly in steel, undecided yet between a 16 ft and a 19 ft hull.
[64] Archive message page_2420 (Chris / "wedgesail" / Chris Ostlind, `paradoxbuilders`, msgnum 2448, 2004-11-07) — "Re: Amelie": supports enlarging Matt Layden's original design (with his apparent, tacit blessing) but argues steel is inappropriate at these sizes even with scaled stretch, since the added weight throughout would work against a fresh look at weight distribution, displacement, and stability; if Matt himself could be drawn into the project the result could be a tough, coastal-cruising world-beater, worth the effort regardless of material.
[65] Archive message page_2735 (knobmaker / "rhaldridge" / Ray, `paradoxbuilders`, msgnum 2766, 2005-06-08) — "scaled-up Paradox": recalls, from the archives, several builders having proposed scaling Paradox up into a slightly larger boat able to sleep two comfortably; asks whether anyone has actually done this, and if so how it turned out. Unanswered on record. No boat or build of his own on record; new below-threshold correspondent (see also [chine-runners/how-they-work.md](/chine-runners/how-they-work.md) and [operations/crew-size-and-fit.md](/operations/crew-size-and-fit.md) for his other questions this batch).
[66] Archive message page_2892 (Chris / "wedgesail" / Chris Ostlind, `paradoxbuilders`, msgnum 2923, 2005-07-04) — "Re: New file uploaded to paradoxbuilders": replying to Paul Reppeto's wish to see more work on a 17 ft Paradox or "KS2" — "It's coming, Paul, just putting the final touches on the details." Signed "Chris."
[67] Archive message page_2891 (reppeto / "ldjonerik" / Paul Reppeto, `paradoxbuilders`, msgnum 2922, 2005-07-04) — "Re: New file uploaded to paradoxbuilders": "I just wanna see more work on a 17' foot Paradox or KS2." Signed "Paulr."
[68] Archive message page_2897 (frogpondoflakeanna / "Dan", `paradoxbuilders`, msgnum 2928, 2005-07-07) — "Re: New file uploaded to paradoxbuilders": a 17 ft Paradox sounds like exactly what he had been aiming for, though he judges himself not clever enough to adapt the stock 13'10" plans himself and expects he "would probably kill myself before my feet got dry at sea-trials"; asks that progress be shared with the group as it develops. Signed "Dan."
[69] Archive message page_2903 (Chris / "wedgesail" / Chris Ostlind, `paradoxbuilders`, msgnum 2934, 2005-07-15) — "17' KSDuo design images posted": full technical announcement of the KSDuo/KSDuoX design — photos posted to the "Paradox Builders 2" Yahoo group's files section under "17'KSDuo"; 17 ft LOA, 66 in beam overall, 2,300 lb design displacement, strip-built in Western Red Cedar (or suitable available wood) with epoxy/glass laminate both sides; raised pop-top main hatch, 3-degree aft-angled self-draining cockpit deck, aft compartment for a 5 hp outboard/fuel/anchor, folding solar-cell side windows over screened ventilation, enclosed dodger/bimini/side-panel option, cable-actuated remote-wing tiller, 2-degree toe-in bilge keels for low draft and upright drying-out, flip-up bungee-tensioned rudder, molded-in scuppered toe rails, watertight foam-crush-zone bow anchor compartment, and a carbon-fiber-sparred gaff yawl rig balanced for full or reefed combinations. Invites comment from the group. Signed "Chris Ostlind."
