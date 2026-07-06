---
type: Concept
title: Running lights — why an all-around white light instead of red/green sidelights
description: Covers why Paradox and Little Cruiser carry a single masthead all-around white light instead of red/green running lights, and how builders wire and construct compact LED masthead units.
tags: [paradox, operations, safety, navigation-lights, colregs, glen-maxwell, alastair, little-cruiser, wiring, mast, led, susan-davis, david-leblanc, dc, derek-clark, kjell-karlsson, dave-bolduc]
timestamp: 2026-07-04T00:00:00Z
---

# Running lights

The [Paradox](/paradox.md) and [Little Cruiser](/matt-layden/little-cruiser.md)
plans call for a single **mast-head (all-around) light** rather than the
conventional red/green port-and-starboard **running lights** most sailboats
carry.

## The COLREGs case for a single masthead light

**International maritime law** only requires vessels under 17 ft to be able
to show a **white light** in time to avoid a collision — even a simple
flashlight would technically satisfy this. Paradox instead carries a proper
**all-around white light** (the same fixture doubling as an anchor light) to
meet the requirement.

This arrangement creates a **right-of-way advantage** that is not at first
apparent to anyone unfamiliar with the rules: a vessel **overtaking another
is always burdened** and must give way to the vessel being overtaken.
Because a lone white light on the horizon reads, at a distance, like the
**stern light of another vessel already underway**, an approaching vessel
will tend to assume it is the overtaking party and alter course to avoid
Paradox — working in the small boat's favor even though Paradox is not,
strictly, "underway with a stern light" in the traditional sense.

A legal subtlety worth noting: **inland right-of-way rules do not by
themselves satisfy international right-of-way rules, but international
rules do satisfy inland rules** — i.e. complying with the (stricter)
international standard is always sufficient.

For **river sailing** specifically, it may still be worth adding
conventional **port and starboard sidelights** as well — not because the
white light is legally insufficient, but because night-running high-speed
powerboat operators on rivers cannot be relied on to correctly interpret
right-of-way cues at all, being often "real stupid, real drunk or both." A
bright, long-range **spotlight** carried for shining in the face of oncoming
night traffic is a complementary practical tactic for the same reason — it
actively forces the issue rather than relying on the other vessel correctly
reading a masthead light.

## A compact LED tricolour/all-round masthead unit

One practical build combines both a **tricolour light** and a **white
all-around light** in a single unit **less than 2 in in diameter and 1.5 in
tall**:

- Built using **LEDs**, which use roughly **one-tenth the power** of an
  equivalent filament bulb for the same light output — a meaningful saving on
  a boat with limited battery capacity (see
  [weight, ballast, and displacement](/design/weight-and-ballast.md)).
- Only **two wires** run up the mast to power it: the tricolour and
  all-around LEDs are wired in **opposite polarity**, so reversing the
  battery connection's polarity switches which light function is lit — a
  neat way to drive two independent light functions over a single
  two-conductor run instead of the four-plus wires a conventional
  separate-fixture setup would need.
- A boat with no engine has no need for a separate steaming light.

## Routing and maintaining masthead-light wiring without cutting the mast open

Electrical wiring is one of the **most frequently replaced items** on any
sailboat, due to **corrosion**. Epoxying masthead-light wiring into the
interior of the mast would mean cutting the mast open every time it needs
replacing — so the wiring is better left **unencapsulated**:

- A **socket at the bottom of the mast** can be **extracted**, leaving a
  **20 mm hole** to fish wire through.
- At the top, the wire exits through a hole **just big enough for the wire
  itself**, then is **sealed in place with silicone sealer**.
- The wire itself is **not epoxied in**: it simply **hangs loose inside the
  mast** (padded to stop it slapping against the inside), so it can be pulled
  and replaced without cutting into the mast.
- Ordinary **5 amp flex** cable is adequate for the run.

This approach — leaving the wire loose rather than encapsulating it — is what
lets a compact two-wire LED masthead unit be installed and later serviced
without opening up the mast.

## Routing masthead-light wiring outside the mast, below the sheave

A stave-built mast leaves little room past the **masthead sheave and its
axle** for wiring routed fully inside, which raises a second routing
question distinct from mast-base servicing above: whether to run the wire
inside the mast all the way to the top, or exit it 100-150mm below the light
and run the last stretch up the outside.

Builders have settled on three different answers. The most common is to
bring the wire out below the mast's solid top and run it up the outside from
there, since the plans' dimensions leave very little clearance past the
sheave and axle for wiring kept fully inside; a cleaner variant of the same
idea, floated in hindsight, is to run copper strips up the outside of the
mast near the top and bury them under a wrap of fiberglass cloth rather than
leaving bare wire exposed on the surface. A second builder likewise routes
the wiring **outside the mast at the top**, exiting near the topping-lift
hardware. A third keeps the wiring recessed **flush with the mast's
surface**, routed through a shallow groove rather than run proud on the
outside or fished through the interior.

At the **bottom** of the mast, one builder brings the wire out under deck
level and connects it to a plug fitted just under the forward port-side
deck — simple to connect and disconnect each time the mast is stepped or
unstepped for trailering, and proven reliable in service.[38]

## LED electrical theory, and how to wire several in series

The underlying electrical theory behind an LED masthead unit, for builders
wanting to design their own array rather than buy one ready-made:

- **LEDs are current-driven, not voltage-driven**, unlike a filament
  bulb. A filament bulb simply takes whatever voltage it is fed and
  regulates its own current draw; an LED instead needs its **current**
  actively controlled, and must be connected with the correct polarity.
- Every LED has two key ratings: its **forward voltage** and its
  **operating current**. On one builder's own nav light, the white LEDs had
  a forward voltage of **3.46V**, the red **1.84V**, and the green
  **2.2V** — with all three needing about **20mA**, the norm for most LEDs
  generally.
- Below the forward voltage, no current flows and the LED stays dark; at
  the forward voltage, it draws its rated current and shines brightly;
  above it, current rises further (still bright) until, past the rated
  voltage, the LED is destroyed by excess current.
- **The simplest current control is a resistor.** From a 12V supply
  (higher if the boat runs 13.6V or more with a charging system), a
  white LED needing 3.46V leaves 8.54V to drop across a resistor; at the
  desired 20mA (0.020A), Ohm's law (V=IR) gives roughly **427 ohms**
  (rounding up to the nearest convenient value), for a power consumption
  of about **240mW**.
- **Wiring LEDs in series multiplies the light for the same power
  budget.** Three of the same LEDs in series drop 10.38V between them,
  leaving only 1.62V for the resistor — still at 20mA, so the resistor
  drops to about **81 ohms**. Total power draw is unchanged at 240mW,
  but light output **triples**, since less of the fixed power budget is
  wasted as heat in the resistor. Maximizing the number of LEDs wired in
  series to get the most light for the least power draw is the guiding
  design philosophy — used both for a nav-light array and for strings of
  three white LEDs lighting the interior and lockers.

One builder's own array uses **six 60-degree white LEDs** arranged as **two
parallel rows of three in series** (matching the series-wiring principle
above), with a half-watt resistor ample for the 240mW circuit; LEDs and
resistors of this kind are available from general electronics suppliers
such as RS Components (`rswww.com`) in the UK.

## Building a sector'd LED masthead light: LED counts, wiring, and potting

A combined **tricolour (red/green/white) and all-round anchor light** in a
single low-profile housing is worth building rather than buying where a
compact **mast-fitting design** — the mast must stow inside the hull for
trailering — demands a thinner unit than any off-the-shelf fixture. Working
from each LED's datasheet **luminous intensity** (candela) rating against
the legal minimum visibility requirement gives the LED count needed per
sector:

- **Red sector:** 3 LEDs
- **Green sector:** 5 LEDs (green LEDs run dimmer than red at the same
  legal threshold, hence the extra LED)
- **White sector:** 4 LEDs
- **Anchor light:** 6 LEDs

Rather than fit opaque baffles between sectors, each LED's own
**viewing-angle** datasheet figure can set the sector boundaries directly —
accepting a soft, gradual color transition between sectors rather than a
hard cutoff, no worse than many commercial lamps.

The array splits into **five circuits**: three tricolour circuits (5
green + 56 ohm resistor; 3 white + 82 ohm resistor; 3 red + 1 white + 150
ohm resistor) wired in parallel for 720mW total, and two identical anchor
circuits (each 3 white + 82 ohm resistor) wired in parallel for 480mW
total. The tricolour and anchor circuit groups are then wired to each
other in **reverse parallel polarity**, so that reversing the battery
polarity at the mast base switches between the tricolour and the anchor
light — the same two-wire trick noted above, requiring only two
conductors to run up the mast for both light functions.

Construction used two purpose-made circular circuit boards about one inch
in diameter (one per light function), with LEDs positioned point-outward
in their correct sector locations, then the whole assembly **potted in
silicone rubber** with only the LED heads protruding. The housing itself
is a pair of turned plastic fittings and a short length of perspex tube
held together with a central screw, and does double duty retaining the
pin for the mast-head sheave. An alternative construction method — LEDs
mounted around the outside of a short cylinder with wiring run inside —
is a reasonable first idea but is more easily replaced by circuit-board
etching once that equipment is available. A light built this way has
proved **brighter than a 12W filament bulb**.

A navigation-rules objection stands against fitting a tricolour light at
all on a boat this size: Paradox and Little Cruiser are only required to
show a single all-round white (anchor) light, and if a tricolour is fitted
and only the anchor light is switched on at night, an approaching vessel
may misread the lone white light as a **stern light**, concluding it is
overtaking and therefore burdened with giving way — when in fact, with the
tricolour switched on instead, a sailing vessel would have right of way and
could find itself closing far nearer than is comfortable before the other
vessel gives way. The point reinforces, from a different angle, [the
COLREGs case for a single masthead light](#the-colregs-case-for-a-single-masthead-light)
made earlier in this file.

## Running LEDs off a charging battery rather than a steady 12V supply

The forward-voltage/current figures above assume a steady 12V supply, as on
a boat with no charging source aboard. A boat that does charge its battery
under way should size the current-limiting resistor for the **higher
charging voltage** (e.g. 14.4V) rather than the resting 12V; run this way,
the LEDs will simply glow slightly dimmer once charging stops and the
battery settles back toward its resting voltage (around 12.6V fully
charged) — a difference too small to notice by eye. Where the swing between
charging and resting voltage is larger, a simple voltage regulator ahead of
the array can stabilize it, though this is unnecessary on most
installations. Every LED's datasheet gives a **maximum forward current**
rating that must never be exceeded, or the LED is destroyed; white LEDs are
commonly rated for 30mA and green for 25mA, leaving some headroom to work
with as supply voltage varies.

The legal basis for the single all-around white light bears restating:
**COLREGS** requires only that small boats show a white light sufficient to
avoid collision, and by convention a 360-degree masthead light satisfies
this — with most vessels obliged to give way to it. Under power, COLREGS
additionally calls for side
lights, a steaming light, and a stern light, though the steaming and stern
functions may be combined into a single all-around white; side lights,
however, may **not** be folded into a combined tricolor unit under those
rules — a technical limit on how far the two-wire tricolor/anchor-light
trick (above) can be pushed for a boat that is sometimes motored.

## The kerosene-vs-LED debate

A wider debate has played out over whether to power navigation lights with
LEDs or fall back on kerosene, prompted by a builder with a boat under 20 ft
and motorless (for whom USCG nav-light approval is not strictly required,
though desirable) wanting to run nav lights, a compass night light, and
possibly a cabin reading light off rechargeable dry cells and a solar
charger.

The case for **kerosene lamps** over LEDs rests on their being legal and
cheap to operate, and on the view that a lit nav light does not meaningfully
reduce the need for a proper lookout anyway, since a low, small boat is hard
for larger vessels to notice regardless of light brightness. Where LEDs are
wanted, it can be cheaper to buy plain incandescent fixtures and retrofit LED
lamps into them rather than buy pre-made LED fixtures outright (the hobbyist
LED-parts site `ledmuseum.home.att.net` is one source), and an **anchor
light** is generally rated more important than nav lights.

The fuller case runs **against kerosene** running lights as impractical and
unsafe aboard a small boat: expensive to run, and — per repeated firsthand
experience of being confronted by Coast Guard and police — **technically
illegal** as an anchor light unless hoisted above the masthead, contradicting
the Pardeys' own published advice on the point ("they're wrong"). By
contrast, LEDs are cheap as a complete system (small gauge wire, small
battery, small solar panel all being individually inexpensive), last roughly
**10,000 hours**, and do not soot up sails or the cabin the way a kerosene
lamp does. A builder not wanting to assemble their own array can simply buy
**USCG-approved Hella LED nav lights** from Defender Industries or West
Marine; dry-cell dinghy nav lights, by contrast, have a reputation for poor
results. As a design-specific point directly relevant to Paradox: since
Paradox has **no separate steaming light** requirement unless motoring, a
single **all-around white light at the masthead** already satisfies both the
running-light and anchor-light requirements together — the same COLREGs
point made above, reached independently more than once.

**Dave Bolduc's microcruising.com equipment-review page**
(`microcruising.com/review.htm#low`) is a specific LED supplier recommended
as prompt and reasonably priced. A separate, liability-focused observation:
the choice of navigation light mostly matters **after** a collision occurs,
when assigning blame becomes a question of proper warning versus a proper
lookout — and a shallow-draft boat's real practical advantage is being able
to **anchor in locations that exclude deeper-draft vessels** from the
collision risk altogether, sidestepping the whole question.

Other data points from the same discussion: a **Coleman dry-cell lantern
with two fluorescent bulbs** is claimed to run 10+ hours on one bulb (with
the option to run both), though its visibility range on a single bulb is
unclear, raising the question of whether a genuinely efficient light could
simply be run up the mast at night. Inexpensive (~$10) "garde moonlights" —
compact units integrating an LED, battery, and solar panel in a single
masthead-light-like fixture — are another option, though possibly not bright
enough in practice. Coast Guard enforcement of anchor-light rules in
practice appears to be inconsistent and generally lenient: one owner who ran
a **kerosene anchor light** almost nightly for several years in Florida was
only ever questioned twice, on the technicality that the light showed yellow
rather than white (and was partly blocked by the mast), never drawing a
ticket or even a formal warning — with the Coast Guard in that encounter
saying they were glad he carried some form of anchor light at all. Anchor
lights are also, by report, far less common in practice than the rules would
suggest: in one crowded anchorage of roughly 200 boats, only about 10 could
be seen carrying an anchor light of any kind.

## Off-the-shelf LED sources for a boat-tent light

One cheap option, comparable to lockers already wired with LEDs on a
central battery, is a set of two self-contained bicycle LED lamps (about
£15, each roughly 100 x 40 x 20 mm with 3 LEDs and a quick-release clamp,
claimed to run 100 hours on two AAA cells), a design well suited to a boat
tent — though, lacking the ambience of a paraffin hurricane lamp, not a full
substitute for one.[28] A similar off-the-shelf lamp (a Pifco model) prompted
an e-mail to the manufacturer asking them to make a purpose-built all-round
white LED lamp for sailors, which drew only an amused non-answer.[29] A
Swedish supplier, `mitron.se/SURE-E/a-lite.html`, sells a lamp closer to a
genuinely boat-designed unit, purpose-built-looking for boating at a cost of
nearly £44.[30][31]

A cheaper DIY alternative is a home-built all-round LED light for about $18
total ($8 of LEDs plus $10 for a Perko replacement fresnel globe, the LEDs
sourced from `whitelightled.com` and the globe from West Marine or Boaters
World), documented with photographs at
`microcruising.com/Graphics/led2-0004r.jpg` and `led5-0001r.jpg`.[32] A
similar light built without a lens, with LEDs mounted in a length of perspex
tube instead, gives fine all-round white output, but on a similarly-built
red-green-white version the color transition between sectors lacks a sharp
cutover.[33]

## Cold Cathode Fluorescent (CCFL) as an LED alternative

**Cold Cathode Fluorescent (CCFL)** tubes are a possible alternative to LEDs
for a masthead light: CCFLs run roughly three times more efficient than the best white LEDs
(about 80 lumens/watt versus 23 lumens/watt) and, like LEDs, are dimmable.
Their drawbacks are a low-temperature starting limit (will not start below
-4°F/-20°C, though this still beats standard fluorescent tubes), a ballast
that may generate radio-frequency interference, and a shorter working life
(roughly 25,000-50,000 hours against an LED's theoretical 100,000 hours). No
CCFL masthead light is recorded as ever having been built for a Paradox; the
archive's built and tested masthead-light solutions remain the LED designs
above.[34]

CCFL is "another neat idea worth trying," but white LEDs have by now become
cheap enough (around $1 apiece) that there is little reason to switch away
from a homemade eight-bulb LED masthead light such as the one aboard [Little
Cruiser](/matt-layden/little-cruiser.md) (documented at
`microcruising.com/review.htm#low`). Separately from the masthead question,
the Bolducs built a low-cost anchor light around a **$6 solar garden
light** bought at a dollar store — complete with its own small solar panel,
two NiCad cells, and an LED — mounted at deck level specifically so it would
be easier to spot in the dark than a masthead light, which can be mistaken
for a star; it was never meant to satisfy the legal anchor-light
requirement, only to help the crew relocate their own boat after dark.
Testing the same solar garden light through a full year
showed a real seasonal limit: it ran until 3 a.m. in summer but only about
two hours after dark once autumn cut the available daily charging
radiation, prompting a plan to power the fixture from a separate battery
instead, or to feed a larger solar panel into the same garden-light
housing.[35][36]

## Solar-panel cable entrance through the deck or window

For a Paradox with an installed solar panel, wiring the panel's cable into
the cabin can be run either through a hole drilled in a window, or through a
loop of wire left outside the hull rather than piercing anything at all —
the external-loop method used on at least one boat. No builder has recorded
routing a solar-panel cable through the deck itself.[37]

# Citations

[1] Archive message page_525 (buster38801 / David, `paradoxbuilders`, msgnum 526, 2002-06-28) — "Running Lights": asks why Paradox and Little Cruiser have a masthead light instead of red/green running lights.
[2] Archive message page_526 (Glen Maxwell / "ifida", `paradoxbuilders`, msgnum 527, 2002-06-28) — "Re: Running Lights": international law requires only a white light visible in time to avoid collision for vessels under 17 ft; Paradox uses an all-around white/anchor light to satisfy this; overtaking vessels are burdened and must give way, so a lone white light reads as a stern light and tends to make approaching vessels alter course; inland right-of-way rules don't satisfy international rules but international rules satisfy inland ones; suggests adding port/starboard lights too for river sailing given reckless high-speed night traffic.
[3] Archive message page_527 (malomac / "doc", `paradoxbuilders`, msgnum 528, 2002-06-28) — "(No subject)": after 44 years on the water, recommends also carrying a bright, long-range spotlight to shine at oncoming night traffic, reasoning that high-speed night operators are usually "real stupid, real drunk or both."
[4] Archive message page_528 (Alastair / "openboat", `paradoxbuilders`, msgnum 529, 2002-06-28) — "Re: Running Lights": his Paradox has (or will have) a combined tricolour/all-round white LED masthead unit under 2 in diameter and 1.5 in tall; LEDs use about a tenth the power of an equivalent filament bulb; only two wires run up the mast, with the two light functions wired in opposite polarity so reversing battery polarity switches between them; no steaming light fitted since he does not plan to run an engine.
[5] Archive message page_579 (roger chan, `paradoxbuilders`, msgnum 580, 2002-07-13) — "Re: Wire maintenance in Mast": asks whether epoxying the mast-head light wiring into the mast means having to cut the mast open to replace it (a frequently-needed repair on any boat due to corrosion), or whether there is a Paradox design feature that avoids this.
[6] Archive message page_580 (Alastair / "openboat", `paradoxbuilders`, msgnum 581, 2002-07-13) — "Re: Wire maintenance in Mast": "you have to sort this out for yourself"; his solution is an extractable socket at the mast base (leaving a 20 mm hole), a small silicone-sealed exit hole at the top (untested as of writing), and 5 amp flex wire hanging loose (padded to stop slapping) rather than epoxied in, so it can be replaced without cutting the mast.
[7] Archive message page_1016 (futabachan / Susan Davis, cross-posted `bolger`/`microcruising`/`paradoxbuilders`, msgnum 1032, 2003-06-18) — "LED array navigation lights?": under 20 ft, motorless (USCG approval not strictly required); wants to run nav lights, a compass night light, and maybe a cabin reading light off rechargeable dry cells and a solar charger; asks for a good LED array source, having ruled out self-contained dinghy nav lights as unreachable from the cockpit.
[8] Archive message page_1017 (whisper / David LeBlanc, `paradoxbuilders`, msgnum 1033, 2003-06-18) — "Re: LED array navigation lights?": complains about receiving four copies of the cross-posted message; prefers kerosene lamps as legal and cheap, arguing nav lights don't much reduce the need for a proper lookout; if LEDs are wanted, cheaper to retrofit LED lamps into incandescent fixtures than buy pre-made LED fixtures; points to ledmuseum.home.att.net; rates an anchor light as more important than nav lights.
[9] Archive message page_1018 (lwhited / Larry Whited, `paradoxbuilders`, msgnum 1034, 2003-06-18) — "Re: LED array navigation lights?": points to Dave Bolduc's microcruising.com equipment-review page (microcruising.com/review.htm#low) for a prompt, reasonably-priced LED supplier; has his own array but hasn't wired it up yet.
[10] Archive message page_1019 (kd7ixk / "DC", `paradoxbuilders`, msgnum 1035, 2003-06-19) — "Re: LED array navigation lights?": needles David LeBlanc's cross-posting complaint; kerosene running lights are impractical and expensive, and a kerosene anchor light is technically illegal unless hoisted above the masthead (contra the Pardeys' published advice, "they're wrong"), per his own repeated experience being confronted by Coast Guard and police; LEDs are cheap as a system (wire/battery/solar panel all inexpensive), last ~10,000 hours, and don't soot up sails or the cabin; recommends USCG-approved Hella LED nav lights from Defender or West Marine if not building an array; reports poor results from dry-cell dinghy lights specifically; asks what dry-cell type Susan has in mind; notes an all-around white masthead light alone satisfies both running-light and anchor-light rules unless motoring.
[11] Archive message page_1025 (fklitzke / Fred Klitzke, `paradoxbuilders`, msgnum 1041, 2003-06-20) — "Re: LED array navigation lights?": also been looking for a good, cheap nav/anchor-light solution; not sold on a full 12V/solar/LED system given the hassle and expense; noticed a Coleman dry-cell lantern with two fluorescent bulbs, claimed 10+ hours on one bulb, visibility on one bulb unknown; asks if an efficient light could simply be run up the mast at night.
[12] Archive message page_1030 (proaconstrictor, `paradoxbuilders`, msgnum 1046, 2003-06-21) — "Re: LED array navigation lights?": his own home waters have "kinder gentler, well ok, all but absent" Coast Guard presence, loosening practical compliance pressure; mentions ~$10 "garde moonlights" integrating LED, battery, and solar panel in a masthead-light-like unit; guesses they may not be bright enough.
[13] Archive message page_1033 (TOMCBRADY / "bigeddytom", `paradoxbuilders`, msgnum 1049, 2003-06-21) — "Re: LED array navigation lights?": ran a kerosene anchor light almost nightly for several years in Florida; the Coast Guard commented only twice, on its being yellow rather than white and partly mast-blocked, never issuing a ticket or warning, and saying they were glad some anchor light was shown; in one ~200-boat anchorage, only about 10 boats showed any anchor light at all. Signed "Tom on Sandpiper."
[14] Archive message page_1034 (lwhited / Larry Whited, `paradoxbuilders`, msgnum 1050, 2003-06-21) — "Re: LED array navigation lights?": light choice mostly matters after a collision, as a question of proper warning vs. proper lookout; a shallow-draft boat's real advantage is anchoring where deeper-draft boats can't come close in the first place.
[15] Archive message page_1787 (openboat / "Alastair", `paradoxbuilders`, msgnum 1810, 2004-01-08) — "LED navigation lights part 1": first of a planned two-part write-up (theory, then construction); explains LEDs are current- not voltage-driven and polarity-sensitive; gives forward-voltage/operating-current figures for his own nav light's white (3.46V), red (1.84V), and green (2.2V) LEDs, all at ~20mA; walks through the voltage/current behavior below, at, and above the forward voltage; works a resistor-sizing example (427 ohms/240mW for one white LED at 12V) and shows wiring three in series triples light output for the same 240mW by dropping the resistor to 81 ohms; describes his own design philosophy of maximizing series LEDs for output per watt, also used in strings of three white LEDs for interior/locker lighting. Signed "Al, Yeovil, England."
[16] Archive message page_1789 (ifida / "Glen Maxwell", `paradoxbuilders`, msgnum 1812, 2004-01-08) — "Re: LED navigation lights part 1": "Great post Al! Tailwinds, Glen." Quotes Alastair's write-up in full.
[17] Archive message page_1791 (dclark52001 / "Derek Clark", `paradoxbuilders`, msgnum 1814, 2004-01-09) — "Re: LED navigation lights part 1": asks Alastair whether his six 60-degree white LEDs are wired as two rows of three in parallel, whether a half-watt resistor is ample for 240mW, and what UK source he uses for LEDs.
[18] Archive message page_1792 (openboat / "Alastair", `paradoxbuilders`, msgnum 1815, 2004-01-09) — "Re: LED navigation lights part 1": answers Derek Clark by pointing to his companion "part 2" construction post; confirms he sources his LEDs and resistors from RS Components (`rswww.com`).
[19] Archive message page_1793 (openboat / "Alastair", `paradoxbuilders`, msgnum 1816, 2004-01-09) — "LED navigation lights part 2": full construction write-up — LED counts per sector (3 red, 5 green, 4 white, 6 anchor), using each LED's datasheet viewing angle rather than opaque baffles to set sector boundaries; five circuits (three tricolour circuits in parallel at 720mW, two anchor circuits in parallel at 480mW) wired to each other in reverse parallel polarity for two-wire mast operation; built on two one-inch circular circuit boards potted in silicone rubber, housed in turned plastic fittings and a perspex tube, doubling as the mast-head sheave pin retainer; an alternative cylinder-mount construction method considered and abandoned once he gained access to circuit-board etching equipment; finished light brighter than an existing 12W filament bulb. Signed "Al, Yeovil, England."
[20] Archive message page_1794 (ifida / "Glen Maxwell", `paradoxbuilders`, msgnum 1817, 2004-01-09) — "Re: LED navigation lights part 2": thanks Alastair for an informative post; raises a COLREGs objection to fitting a tricolour light — showing only the anchor light at night risks being misread as a stern light by an overtaking vessel, ceding right-of-way that a lit tricolour would otherwise preserve for a sailing vessel.
[21] Archive message page_1802 (openboat / "Alastair", `paradoxbuilders`, msgnum 1825, 2004-01-10) — "Re: LED navigation lights part 2": answering Glen Maxwell, agrees an all-round white alone is simpler, and is what he himself would use if motoring at night.
[22] Archive message page_1803 (kd7ixk / "DC", `paradoxbuilders`, msgnum 1826, 2004-01-10) — "Re: LED navigation lights part 2": praises Alastair's two-wire polarity-switching design; asks whether his forward-voltage/current figures assume a regulated 12V supply, and what a charging battery (14.4V) or a rested, fully-charged battery (12.6V) would do to the LEDs; restates the COLREGs basis for the single all-around white light (only a white light is required to avoid collision; an all-round masthead light satisfies it by convention, with most vessels obliged to give way); notes that under power COLREGS also requires side lights, a steaming light, and a stern light — the steaming and stern functions may be combined into an all-around white, but side lights may not be folded into a tricolor.
[23] Archive message page_1805 (openboat / "Alastair", `paradoxbuilders`, msgnum 1828, 2004-01-10) — "Re: LED navigation lights part 2": confirms his figures assume 12V, since "Little Jim" has no charging facility; a charging system running at 14.4V should have the resistor sized for that voltage instead, with only an imperceptible dimming once charging stops; the LED datasheet's maximum forward current must never be exceeded (his own white LEDs rated 30mA, green 25mA, giving some headroom for voltage swings); a simple voltage regulator (from RS Components) can stabilize a larger swing if needed.
[24] Archive message page_1819 (sdhender / "Steve", `paradoxbuilders`, msgnum 1842, 2004-01-13) — "Wiring for masthead light": with three of the mast's four main pieces already epoxied together, asks how other builders have routed masthead-light wiring — fully inside the mast to the top, or exiting the mast 100-150mm below the light to run outside from there — preferring to keep the wiring inside if reasonable. Signed "Steve, in the Heartland of the USA."
[25] Archive message page_1820 (openboat / "Alastair", `paradoxbuilders`, msgnum 1843, 2004-01-13) — "Re: Wiring for masthead light": full text and citation above (see "Routing masthead-light wiring outside the mast, below the sheave"); brought his own wires out below the mast's solid top and ran them up the outside, since the plans' dimensions leave very little room past the sheave and its axle for wiring routed fully inside; in hindsight, wishes he had instead run copper strips up the outside near the top before wrapping in fiberglass. Signed "Al, Yeovil, England."
[26] Archive message page_1821 (ifida / "Glen Maxwell", `paradoxbuilders`, msgnum 1844, 2004-01-14) — "Re: Wiring for masthead light": "I had to run mine out side of the mast at the top. You can see a picture of it in the files section under topping lift, first picture." Signed "Glen."
[27] Archive message page_1822 (dlb / "dlb" / David Beard, `paradoxbuilders`, msgnum 1845, 2004-01-14) — "Re: Wiring for masthead light": "I routed a small groove for the wires to lay in." Signed "David."
[28] Archive message page_2434 (openboat / "Alastair", `paradoxbuilders`, msgnum 2462, 2004-11-17) — "LED lighting (again)": when he built "Little Jim" he installed LEDs in all the lockers and remote corners wired to a central battery, and was delighted with the results; wondered why he had bothered on finding a set of 2 self-contained bicycle LED lamps for £15 (each ~100 x 40 x 20 mm, 3 LEDs, quick-release bike clamp, claimed 100 hours on 2 AAA cells); felt they could have been designed for a boat tent, though without the ambience of a paraffin hurricane lamp. Signed "Al, Yeovil, England." Cross-posted to `paradoxbuilders` and `microcruising`.
[29] Archive message page_2435 (dclark / "dclark52001" / Derek Clark, `paradoxbuilders`, msgnum 2463, 2004-11-18) — "Re: LED lighting (again)": bought a similar Pifco lamp set the year before and had the same thought; e-mailed Pifco asking them to make an all-round white LED lamp for sailors, but received only an amused reply he didn't think was serious — "if they do make them I'm claiming credit!"; jokes that if he hadn't asked Alastair about the furling-spindle copper pipe (see [Alastair](/people/alastair.md)) it might have failed sooner; signs off "busy setting up my new table saw to finish cutting the chine logs" (see [chine log vs. taped-seam construction](/construction/chine-log-vs-taped-seam.md#a-follow-up-choice-brazilian-mahogany-versus-sapele)).
[30] Archive message page_2437 (gilljam.karlsson / "kjellkkk" / Kjell Karlsson, `paradoxbuilders`, msgnum 2465, 2004-11-19) — "Re: LED lighting (again)": in reply to Derek Clark's Pifco story, points to a Swedish supplier, `www.mitron.se/SURE-E/a-lite.html`.
[31] Archive message page_2439 (openboat / "Alastair", `paradoxbuilders`, msgnum 2467, 2004-11-19) — "Re: LED lighting (again)": Kjell's mitron.se lamp "is clearly designed for boating," though it costs nearly £44.
[32] Archive message page_2438 (mbolduc / "boldav38" / Dave Bolduc, `paradoxbuilders`, msgnum 2466, 2004-11-19) — "Re: LED lighting (again)": a home-built all-round LED light can be made for about $18 ($8 LEDs, $10 Perko replacement fresnel globe); LEDs from `www.whitelightled.com`, globe from West Marine or Boaters World; photos at `microcruising.com/Graphics/led2-0004r.jpg` and `led5-0001r.jpg`.
[33] Archive message page_2440 (openboat / "Alastair", `paradoxbuilders`, msgnum 2468, 2004-11-19) — "Re: LED lighting (again)": built a similar light of his own without a lens, mounted in perspex tube instead; the all-round white version is fine, but on a similarly-built red-green-white version the color cutover between sectors isn't very sharp.
[34] Archive message page_2698 (fasttimes / Brent Geery, `paradoxbuilders`, msgnum 2728, 2005-05-28) — "Introduction": most builders seem to use LEDs for a mast light; asks if anyone has considered Cold Cathode Fluorescent (CCFL) instead, citing 80 lumens/watt versus 23 lumens/watt for the best white LEDs, dimmability, a -4°F/-20°C starting-temperature floor, possible ballast RF interference, and a 25,000-50,000 hour life versus LEDs' theoretical 100,000 hours; links `elwirecheap.com` ($12 CCFL kits) and `j-right.com` (CCFL/LCD backlighting info). Answered at [35].
[35] Archive message page_2703 (mbolduc / "boldav38" / Dave Bolduc, `paradoxbuilders`, msgnum 2733, 2005-05-28) — "Re: Introduction": answers Brent Geery's CCFL question — a neat idea worth trying, though white LEDs are now cheap enough (~$1 apiece) that the Bolducs see no reason to move on from their own homemade 8-bulb LED masthead light aboard Little Cruiser (`microcruising.com/review.htm#low`); separately reports working on a low-cost anchor light built from a $6 "solar" garden light (from BIG LOTS) with its own small solar panel, two NiCad batteries, and an LED, mounted at deck level so it is easier to spot in the dark than a masthead-height light, which can be mistaken for a star.
[36] Archive message page_2739 (logicaid / "Alan", `paradoxbuilders`, msgnum 2739, 2005-06-01) — "'Garden' lights": reports testing the same kind of solar garden light through a full year: still running at 3 a.m. in midsummer, but only about two hours after dark once autumn cut the available daily charging radiation; plans to power a similar 360-degree-diffuser garden light from a separate battery instead, and is experimenting with feeding a larger solar-AA-NiCad-charger panel into the same garden-light housing. Signed "Alan."
[37] Archive message page_2702 (gilljam.karlsson / "kjellkkk" / Kjell Karlsson, `paradoxbuilders`, msgnum 2732, 2005-05-28) — "2 pics 2 questions": asks how other builders with an installed solar panel route its cable into the cabin — through a hole drilled in a window, or some other method — having noticed Glen Maxwell uses an external loop instead. No reply recorded.
[38] Archive messages page_3178/page_3180 (william / "williamserjeant" / William Serjeant, `paradoxbuilders`, msgnum 3209, 2005-10-08, "Mast Questions"; and ifida / "Glen C. Maxwell", `paradoxbuilders`, msgnum 3211, 2005-10-08, "Re: Mast Questions") — Bill, gluing his mast's front piece into place, asks where the masthead light's wiring should exit the mast and how it should route down to the battery terminals given the mast is stepped and unstepped for trailering, noting Glen's own masthead photos show an external housing for the flex at the top. Glen answers: the top routing follows what Bill already worked out from photos of "Zoë"'s masthead; at the bottom, he brings the flex out under deck level and connects it to a plug fitted just under the forward port-side deck, which has proven easy to connect and disconnect. Signed "Bill" / "Glen."

