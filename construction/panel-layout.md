---
type: Concept
title: Panel layout and nesting on the plywood
description: How Paradox panels, bulkheads, and the transom nest on the plywood sheets, the tight fits and how to resolve them, and the Hull/VRML/CAD nesting-software workflow.
tags: [paradox, construction, layout, nesting, plywood, bulkhead, transom, cad, hull-program]
timestamp: 2026-07-04T00:00:00Z
---

# Panel layout and nesting

Before cutting, [Paradox](/paradox.md) parts are laid out ("lofted") on the
plywood sheets. Several parts nest onto a single sheet and the fit is **tight**,
so careful layout — "check your layout twice before you cut" — matters. See the
[plywood bill of materials](/design/hull-scantlings.md) for what comes from
which thickness.

## Tight spots builders hit

- **Bulkhead #2 vs. the forward side panel.** [Matt Layden](/matt-layden/biography.md)'s
  plans put the **butt joint for bulkhead #2 at 100 mm (stbd) off the ship's
  centerline**. Moving the joint **over 50 mm** off centerline instead gives a
  better cutting clearance. All parts for the side panel — both bulkhead-#2
  pieces and the transom — are meant to come out of that **one sheet** without
  buying an extra.
- **Transom vs. side panel.** These can appear to overlap on the sheet. Rough
  dimensions: the side panel is about **670 mm tall** and the transom about
  **510 mm**; the aft side-panel base dimension is **28 mm** and the forward
  base is **115 mm**. Recalculated against the forward panel, the overlap is
  only about **2.5 cm** at maximum slop.

## The missing transom-radius dimension, resolved

The plans give the dimension for the **lowest point** of the transom's curved
radius but not the corresponding figure for the **top of the radius**, where
the drawing shows only lines and arrows with no accompanying numbers. The
figure is **57 mm**, confirmed two independent ways: working back from the
deck-beam dimensions on plan sheet 10 gives 57 mm at the top-right dimension
arrows with no problems fitting the deck, and a separate digital model of the
plans converges on the same 57 mm. A general beam-crop technique applies to
this same transom-radius/bulkhead-curve family of dimensions: drawing 7 gives
bulkhead #2 the curve dimensions for the **master beam crop**, a curve common
to all four bulkheads; rather than cutting a separate crop template for each,
it is simpler to mark out bulkhead #2 once and use it as the crop for the
others — lay the already-cut bulkhead #2 onto the next sheet of ply alongside
the main dimensions already drawn (bulkheads 1, 4, and the transom), line up
the centerlines and deck marks, and scribe.

## Ways to resolve an overlap

1. **Tilt the side-panel base line** so it is no longer parallel to the edge of
   the ply — this frees enough room around the parts to clear the transom. This
   is the recommended fix.
2. **Swap the transom and the adjacent bulkhead section**, flipping the bulkhead
   about a horizontal axis, so you only lose the top corner of the bulkhead —
   which is removed anyway to make room for the **sheer clamp**.
3. **Buy an extra half/full sheet.** Buying another sheet of 1/2 in ply avoids
   making a two-piece bulkhead at station #2; a **half sheet** is also the fix
   if the **rudder cheeks** will not come out of the 18 mm sheet alongside the
   bow section. If nesting a paper pattern of the side panel first, the ply
   edge stops being important to the base line.
4. **Fit a spare part into the freed-up space and move the piece to a different
   sheet entirely.** The bulkhead-#2 fit issue recurs across builds —
   [Walden](/boats/walden.md) hit the same snag, not a one-off. One
   workaround: **move bulkhead #2 over 40 mm**, giving a **511 mm-wide
   starboard side** and a **591 mm-wide port side**. This in turn means the
   **transom will not fit** on the sheet as laid out; rather than tilting the
   baseline or swapping pieces, **fit one of the rudder blades into the
   freed-up space** and move the transom onto a **different sheet**
   entirely — a third way to resolve an overlap when there is spare capacity
   elsewhere in the cutting list.

## Layout tips

- **Mark each side panel** — which is which, inside vs. outside — or you will end
  up cutting new ones.
- Keep the **grain of the ply running as Matt indicates**, especially on any
  added sheet.
- Nest with **paper patterns** of the parts to juggle a tight fit before
  committing to the ply.
- The plans' **layout diagram omits several parts** entirely, so builders should
  watch for them and plan to use offcuts:
  - **Vent trunk pieces** — 18 mm for the front piece, 9 mm for the sides.
  - The **breasthook**.
  - **Butt blocks** — 12 mm.

## Bulkhead side curves

The plans specify a small **offset (curve) in the side edge** of three of the
four bulkheads — **5 mm** for bulkhead #1, **7 mm** for bulkhead #2, and **5 mm**
again for bulkhead #3 — while **bulkhead #4 and the transom** show no offset at
all, meaning those two have straight sides. The curve likely adds useful
**stiffness** to the sides. In practice the plywood side panels bend to match
this curve and nail up cleanly without difficulty.

## Metric vs. imperial measuring

The Paradox plans' **millimetre values are metric conversions of inch sizes**,
since [Matt Layden](/matt-layden/biography.md) himself bought his own materials
in inches. US "nominal" lumber sizes run smaller than stated (a 2x4 board is
closer to 1-5/8 x 3-1/2 in) due to grading and building-code allowances, so a
builder working in metric is better off measuring actual lumber dimensions in
cm at the lumberyard rather than trusting the nominal inch label, aiming for
**±2 mm** accuracy. There is also a practical distinction between **sawn** and
**planed** dimensional lumber: sawn stock is close to its nominal size, while
planed stock is sawn to size and then has more removed. Solid wood dimensions
(unlike **plywood**, which must be held to size) can vary several millimetres
without making a significant difference to the finished construction. Using a
pocket calculator to work in fractional inches (1/2", 1/4", 1/8"...) already
treats them as a decimal/metric-like system, sidestepping conversion errors by
adding and subtracting directly rather than converting first.

Paradox plans reach Australian and UK builders **already converted to
metric** without any special request — apparently standard practice for the
design rather than a special order — so a builder can work entirely in
millimetres throughout without reconciling Imperial-measure US plans against
metric plywood by hand. A free online conversion utility
(`joshmadison.com/software/convert`) covers any remaining unit
conversions.[32a][33][34]

A separate but related Australian plywood problem surfaced in the same
exchange: **locally produced Australian plywood** runs a metric sheet size
of **2400 x 1200 mm**, while imported **Gaboon** (Okoume, a West African
hardwood, also called Samara) runs **2500 x 1220 mm** — closer to the
dimensions Matt Layden's sheet layout actually assumes. The mismatch bites
hardest at **bulkhead #3**, drawn **1214 mm wide**, which does not fit the
locally produced sheet size using the plans' own layout. A Tasmanian builder
working from a **1:5 scale model** in aircraft ply toward CNC files for a
local CAD cutting service made his own CNC DXF files available to the
Bolducs for distribution alongside the plans.[35][36][37]

A workaround for the local-plywood mismatch followed: build **bulkhead #3 in
two parts**, scarfing the bottom section on, since the shorter local sheet
cannot supply its full 1214 mm width in one piece; the left-hand side panel
on the plans' drawing 6 also will not lay out as dimensioned on a 2400 mm
sheet, though the right-hand panel yields enough spare material to make up
the shortfall, and the aft bottom panel comes out slightly narrow near the
chine runners as well. Beyond sourcing imported Gaboon (which sidesteps the
sizing problem but raises its own old-growth/rainforest sourcing concern),
two alternative local timbers were suggested: **Hoop Pine**, whose veneers
are considered better made than Gaboon's, and the cheaper, more toxic
**Proof Ply**, which glues and paints well but is treated with CCA or a
similarly hazardous preservative. A sustainable-timber workaround beyond
these two options was asked for but not answered on record.[38]

## Side-deck and cabin-end-panel layout: a plans tight fit

Since the deck's width is **greater than 4 ft**, the **two side decks and the
two cabin end panels** do not all come from a single 4 ft-wide sheet of ply
as the plans show — a related issue to layout of the [mast interior sealing
and anchor-light fit](/construction/mast-sealing-and-fit.md).

The geometry: the **side decks** span from the **gunwale to the carlines**,
while the **end pieces** span **between the carlines** — and the distance
**between the gunwales alone** is already more than 4 ft, before the end
pieces are even added in. Only **2 of the 6 end pieces** are actually
affected, small enough that a builder can get away with a **joint in one
piece at each end** rather than needing a wider sheet.

This is a genuine tight-fit plans issue, confirmed by re-measuring against
**sheet #3** of the plans: the **maximum width of the foredeck is 3 ft 11
in**, and adding a little more for the **deck crown**, a builder following
the plans exactly will probably go over 4 ft. The fix in practice is to
**scab in an extra piece on each side** to reach all the way out to the edge
of the gunwales, a small **jointed addition** at each side rather than a full
extra sheet. See [Little Jim](/boats/little-jim.md) for the boat-level record
of this resolution.

This is a fourth kind of layout-fit problem alongside the
[bulkhead #2](#tight-spots-builders-hit), [transom](#tight-spots-builders-hit),
and [bulkhead side curve](#bulkhead-side-curves) issues above — this time on
the **deck** sheets rather than the hull-panel sheets.

## Cabin-end C-formed pieces, cut from the same 9mm sheet as bulkhead 1

The plans' layout for the **9mm sheet carrying bulkhead 1** also nests a set
of small **C-formed pieces** that are easy to miss on a first read, since
they do not obviously belong with anything drawn on sheet 4 alone. These
pieces are part of the **cabin ends**: they laminate onto the deck at each
end of the cabin to give the bottom of the cabin **windows** something to
attach to, and appear again, in context, on **sheet 4**, above bulkhead 4 and
at the bottom of the front window.

In practice the 9mm sheet does not always leave enough room to cut all four
pieces exactly as drawn once the bin sides have already been removed from
the same sheet — one builder found the points where they interlock with the
neighboring part had to be sacrificed for lack of ply, and simply glued in a
small extra offcut to restore the missing point once the pieces were
laminated up. The companion 12mm sheet carrying similar pieces can present
the same shortfall; the fix there is to reorder the layout, as covered in a
build's own "drawing changes" notes rather than by re-deriving the geometry
from scratch.

## No nesting plan exists for a stretched hull

Whether anyone has worked out a plywood nesting plan for a **stretched**
Paradox specifically — rather than the stock-length layout documented
above — is a question that surfaced once on the list but drew no recorded
answer; see [stretched Paradox](/design/variants/stretched-paradox.md) for
the design's scaling rules more generally.

## Lofting weights ("spline weights" or "lead ducks")

Full-size lofting of the plans' curved lines calls for a flexible batten
bent to the curve and held down at intervals — a job traditionally done with
cast-lead **"spline weights,"** also called **lead ducks**. A usable
secondhand set (six ducks, about 6¼ in long and 3½ lb each, lead cast in a
thick plastic coating with a flat-ish base and a threaded front hole for a
hook the buyer supplies) can be found cheaply through online auction
listings — one builder paid about $21 for a set that others have bid up past
$60, more than the sets are worth once shipping (roughly $14 for six, being
solid lead) is added in. A builder without access to a secondhand set can
also **cast a set from scratch**; plans for doing so are published at
`splineweights.com/makeyourown.htm`. Old discarded wheel-balance lead or
fishing sinkers are a further scrap-lead source, also usable more generally
as cast trim ballast. [Matt Layden](/matt-layden/biography.md) himself uses
lead ducks of this same general type, visible in his own construction
photos.[39][40][41][42][43]

## Software for nesting and converting the offsets: Hull, VRML, and CAD

Separately from the stretched-length question above, **Gregg Carlson's
"Hull"** — a freeware naval-architecture program with a **nesting
function** — provides another way to work the Paradox's own offsets: the
Paradox's values have already been entered into the program, can be
enlarged, and can be output as a text file of offsets to play with the
nesting of developed panels.

**Hull's output files can be imported into AutoCAD**, following a
step-by-step online tutorial for converting a Hull file to AutoCAD. The
Paradox's own offsets have been posted to the group's Files section for
builders' benefit: following the AutoCAD tutorial, a program called
**"Crossroads"** converts the **VRML** file Hull produces into **DXF**
format, which imports into **IntelliCAD 2000** without problems — confirming
the conversion path works in practice, not just in principle. Both the
original Hull file and the converted 3D DXF file are posted to the Files
section; the DXF format is **easier for most builders to work with** than
the native Hull file.

The Paradox **`.Hul`** file needs Gregg Carlson's free "Hull Designer"
program to open, while the 3D **`.dxf`** file needs a 3D CAD program —
IntelliCAD 2000 is one that works. A **2D** dxf file is a further
possibility alongside the 3D one already posted, since the file converted so
far is for 3D programs only.

The **3D dxf file** in the Files section's CAD Drawing folder can also be
imported directly into other boat-design software, such as "Nautilus," to
compare against a Paradox modeled from the plans (see [blue-water
suitability](/design/blue-water-suitability.md#flat-panels-and-the-brute-hammer-of-a-breaking-wave)
for the flat-panel seaworthiness question that prompted this cross-check).

This nesting-software thread is distinct from, but complementary to, the
paper-pattern and hand-layout methods described above: Hull's nesting
function works from the Paradox's digitized offsets, while the paper-pattern
method works directly from the plans on the physical sheet of ply.

# Citations

[1] Archive message page_033 (Alastair, `paradoxbuilders`, 2001-07-22) — bulkhead #2 overlaps the stbd forward side panel and the transom overlaps the side panel; Don's articles say move the bulkhead joint 50 mm for cutting clearance.
[2] Archive message page_034 (Glen C. Maxwell, 2001-07-22) — bought another 1/2 in sheet rather than a two-piece bulkhead at station #2; suggests nesting a paper pattern so the ply edge no longer governs the base line.
[3] Archive messages page_035/page_036 (Don Elliott, 2001-07-22) — bulkhead-#2 butt at 100 mm (stbd) off centerline (Don used 50 mm); side panel ~670, transom ~510; couldn't get rudder cheeks from the 18 mm sheet so bought a half sheet; mark inside/outside; keep grain per plans; all side-panel parts should come from one sheet.
[4] Archive message page_038 (Alastair, 2001-07-23) — aft panel base 28 mm, forward panel base 115 mm; two solutions: rotate the side panel, or swap transom/bulkhead and lose only the top corner removed for the sheer clamp.
[5] Archive message page_039 (Don Elliott, 2001-07-23) — recalculated overlap ~2.5 cm on the forward panel at max slop; tilting the 115 base line gives enough room.
[6] Archive message page_171 (Chris Becker, `paradoxbuilders`, 2001-12-15) — "It's a Start!": moved bulkhead #2 over 40 mm (511 mm stbd / 591 mm port); transom didn't fit as laid out, so fit a rudder blade in its place and moved the transom to another sheet; layout omits the vent trunk pieces (18 mm front, 9 mm sides), breasthook, and butt blocks (12 mm) — watch for them and plan to use leftovers.
[7] Archive message page_733 (admin / Paul V., `paradoxbuilders`, msgnum 747, 2002-10-04) — "Bulkhead side curves": bulkhead 1 has a 5mm side offset, bulkhead 2 has 7mm, bulkhead 3 has 5mm; bulkheads 4 and the transom show no offset (straight sides); asks if anyone had trouble bending the side ply to this curve, and whether the side nails up nicely; assumes the curve adds stiffness.
[8] Archive message page_736 (Alastair, `paradoxbuilders`, msgnum 750, 2002-10-04) — "Re: Bulkhead side curves": "Not me. I just banged in the nails and it pulled it down, no problem."
[9] Archive message page_734 (admin / Paul V., `paradoxbuilders`, msgnum 748, 2002-10-04) — "Metric system? what metric system?": found a cm/inch tape measure after some searching; US "nominal" lumber sizes (e.g. 2x4) run smaller than stated due to grading/code allowances; plans to measure actual lumber dimensions in cm at the yard rather than trust nominal inch labels, aiming for ±2mm accuracy; did the same converting inches to mm building a canoe in Germany.
[10] Archive message page_737 (Alastair, `paradoxbuilders`, msgnum 751, 2002-10-04) — "Re: Metric system? what metric system?": sawn vs. planed lumber distinction; the plans' mm values are conversions of inch sizes since Matt bought materials in inches; solid wood (unlike plywood) can vary several mm without a significant difference to the final construction.
[11] Archive message page_739 (migchelsen / Barend Migchelsen, `paradoxbuilders`, msgnum 753, 2002-10-05) — "Re: Metric system? what metric system?": using a pocket calculator already treats fractional inches as a metric-like decimal system, eliminating conversion errors since you add/subtract directly.
[12] Archive message page_764 (Alastair, `paradoxbuilders`, msgnum 778, 2002-11-16) — "Progress, a question and a problem": deck width is greater than 4 ft; can't see how the two side decks and two cabin end panels come from one sheet of ply as drawn; asks what the rest of the list thinks.
[13] Archive message page_769 (Glen Maxwell, `paradoxbuilders`, msgnum 783, 2002-11-19/20) — "Re: Progress, a question and a problem": as recalled, no problem with the side decks, because the end pieces are not four feet wide at their widest.
[14] Archive message page_770 (Alastair, `paradoxbuilders`, msgnum 784, 2002-11-20) — "Re: Progress, a question and a problem": side decks span gunwale-to-carlines, end pieces span between the carlines; the distance between the gunwales alone is already more than 4 ft; asks whether Glen cut his panels exactly as shown in the plans; only 2 of the 6 end pieces are affected, so may get away with a joint in one piece at each end.
[15] Archive message page_771 (Glen Maxwell, `paradoxbuilders`, msgnum 785, 2002-11-21) — "Re: Progress, a question and a problem": measuring from sheet #3, the max width of the foredeck is 3'11"; add a little for the deck crown and a builder will probably go over 4 ft; recalls, thinking back, that he scabbed in a piece on each side of his own boat to reach the edge of the gunwales.
[16] Archive message page_1646 (alex29 / "Jack", `paradoxbuilders`, msgnum 1668, 2003-12-30) — "nesting": asks whether anyone has worked out a plywood nesting plan for a stretched-length version of the boat, and would be willing to share it, or whether one is already available — unanswered in the archive.
[17] Archive message page_1652 (ifida / Glen Maxwell, `paradoxbuilders`, msgnum 1674, 2003-12-30) — "Re: nesting": asks Jack Gardiner whether he has a copy of Gregg Carlson's "Hull" program; it has a nesting function, and Glen has already entered the Paradox's values into his own copy and can forward the file; with it a builder can enlarge the values and output a text file of offsets to play with the nesting of developed panels; the program is freeware.
[18] Archive message page_1655 (longyard / "William  Longyard", `paradoxbuilders`, msgnum 1677, 2003-12-30) — "Re: nesting": glad Glen mentioned the Hull program; notes Hull files can be imported into AutoCAD, pointing to an online tutorial ("Hulls to AutoCad in 3 Easy Steps"); suggests Glen put the Paradox offsets into the Files section for other builders' benefit.
[19] Archive message page_1656 (ifida / Glen Maxwell, `paradoxbuilders`, msgnum 1678, 2003-12-30) — "Re: nesting": "Will do."
[20] Archive message page_1657 (alex29 / "Jack", `paradoxbuilders`, msgnum 1679, 2003-12-30) — "Re: nesting": does not have the Hull program yet, but will get a copy.
[21] Archive message page_1659 (ifida / Glen Maxwell, `paradoxbuilders`, msgnum 1681, 2003-12-30) — "Re: nesting": following Longyard's link, downloaded "Crossroads," converted the Hull program's VRML file to DXF format, and imported it into "Intellicad 2000" with no problems; will post both the Hull file and the 3D DXF file to the Files section.
[22] Archive message page_1660 (longyard / "William  Longyard", `paradoxbuilders`, msgnum 1682, 2003-12-30) — "Re: nesting": thanks Glen for the conversion work; expects more people will find a DXF file easier to work with than the native Hull file.
[23] Archive message page_1661 (ifida / Glen Maxwell, `paradoxbuilders`, msgnum 1683, 2003-12-30) — "Re: nesting": confirms the files are uploaded to the Files section under CAD files; the Paradox.Hul file needs Gregg Carlson's free "Hull Designer" program (carlsondesign.com); the 3D Paradox.dxf file needs a 3D CAD program, IntelliCAD 2000 recommended.
[24] Archive message page_1662 (ifida / Glen Maxwell, `paradoxbuilders`, msgnum 1684, 2003-12-30) — "Re: nesting": had not thought of a 2D dxf file as Longyard suggested; the uploaded dxf is for 3D programs; will see about uploading a 2D version too.
[25] Archive message page_1762 (ifida / "Glen Maxwell", `paradoxbuilders`, msgnum 1785, 2004-01-04) — "Re: nesting": tells Bert Vercauteren the 3D dxf files are already in the Files section's CAD Drawing folder, and points him to Chapter 9 (Kjell Karlsson's translated Yrvind excerpt) for Sven Yrvind's own view on Paradox's seaworthiness; quotes Bert's stability-confirmation/flat-panel-safety message and his own prior "nesting" reply in full. Signed "Tailwinds, Glen."
[26] Archive message page_1768 (alex29 / tidybowlmann / "Jack" — Jack Gardiner, `paradoxbuilders`, msgnum 1791, 2004-01-05) — "Transom missing dimension": laying out the transom, can find the dimension for the lowest point of its radius but not the corresponding figure for the top of the radius, where the lines/arrows are drawn with no numbers; asks for any input. Confirmed via `X-Yahoo-Profile`/`u=` headers as the same Jack Gardiner tracked on [people/jack-gardiner.md](/people/jack-gardiner.md), not a distinct newcomer.
[27] Archive message page_1771 (openboat / "Alastair", `paradoxbuilders`, msgnum 1794, 2004-01-05) — "Re: Transom missing dimension": has "57?" pencilled onto his own plans at the top-right dimension arrows, worked back from the deck-beam info on sheet 10; had no problem fitting the deck, so takes 57 mm as correct; suggests leaving the top cut until the deck beam is attached if in doubt. Signed "Hoping for calm nights, Al, Yeovil, England."
[28] Archive message page_1772 (alex29 / tidybowlmann / "Jack Gardiner", `paradoxbuilders`, msgnum 1795, 2004-01-05) — "Re: Transom missing dimension": "Agreed, that seems right, 57 I know if i work at it I could figure it out, but its much easier to follow where one has tread before. Thanks." Signed "Jack."
[29] Archive message page_1773 (kayaker37 / "Paul", `paradoxbuilders`, msgnum 1796, 2004-01-05) — "Re: Transom missing dimension": "My model shows 57mm as well."
[30] Archive message page_1776 (roverticket / "Jeffery Please" / "Jeff UK", `paradoxbuilders`, msgnum 1799, 2004-01-06) — "Re: Transom missing dimension": drawing 7 gives bulkhead 2 the curve dimensions for the master beam crop, common to all bulkheads; rather than making a separate crop for each of the four, marks out bulkhead 2 and uses it as the crop — lays the cut bulkhead 2 onto the ply with the main dimensions drawn (bulkheads 1, 4, transom), lines up the centerlines and deck marks, and scribes. "Simple and quick." Signed "Jeff UK."
[31] Archive message page_1952 (b.genell / "bgenell" / Bengt Genell, `paradoxbuilders`, msgnum 1975, 2004-03-06) — "Sheet layout": received the plans and articles a couple of weeks earlier and studied them carefully, but on laying out the first sheet of ply could not identify the C-formed pieces drawn in the middle of the 9mm sheet with bulkhead 1; asks for an explanation. Signed from "a snowy Sweden."
[32] Archive message page_1953 (openboat / "Alastair", `paradoxbuilders`, msgnum 1976, 2004-03-06) — "Re: Sheet layout": the C-formed pieces are part of the cabin ends, laminated over the deck at each end of the cabin to attach the bottom of the windows to (see also sheet 4, above bulkhead 4 and at the bottom of the front window); found it was not possible to cut all four pieces from the 3rd 9mm sheet exactly as drawn, since there wasn't enough ply left once the bin sides had been removed — lost the interlocking points as a result, then glued in the extra bit when laminating them up; also could not cut the equivalent pieces from the first 12mm sheet as drawn, and reordered the layout instead, recorded under "drawing changes" in the files section. Signed "Hoping for calm nights, Al, Yeovil, England."
[32a] Archive message page_2215 (shersey / "shersey.rm" / Shane Hersey, `paradoxbuilders`, msgnum 2242, 2004-08-31) — "Re: new builder in Oz": asks a new Australian builder how he is managing to fit Imperial-measure US plans against Australian metric plywood sizes; mentions having his own set of Paradox plans and living in Canberra.
[33] Archive message page_2216 (bilbil / "bilbilau" / Bill Anderson, `paradoxbuilders`, msgnum 2243, 2004-08-31) — "Re: new builder in Oz": his plans are already in metric, hadn't specified metric versus imperial, thought that was standard for Paradox; gives a free online unit-conversion program (`joshmadison.com/software/convert`); remarks the Australian fleet is growing.
[34] Archive message page_2218 (dclark / "dclark52001" / Derek Clark, `paradoxbuilders`, msgnum 2245, 2004-08-31) — "Re: new builder in Oz": relieved after checking — has already cut all his bulkheads working entirely in millimetres, and confirms his own plans are metric too; separately asks whether anyone knows how many completed Paradoxes exist worldwide and how many are under construction in England — see [references/paradox-uk-website.md](/references/paradox-uk-website.md#a-uk-and-worldwide-build-count) for the answer.
[35] Archive message page_2223 (shersey / "shersey.rm" / Shane Hersey, `paradoxbuilders`, msgnum 2250, 2004-08-31) — "Re: new builder in Oz": apologizes for assuming the plans weren't metric ("if all else fails read the instructions"); asks OzBill whether he is opting for exterior-grade or marine plywood.
[36] Archive message page_2224 (johndhall / "jdmhall" / John Hall, `paradoxbuilders`, msgnum 2251, 2004-09-01) — "Re: Digest Number 575": Launceston, Tasmania; Australian locally produced plywood runs 2400 x 1200 mm, while imported Gaboon (Okoume) runs 2500 x 1220 mm, a closer fit to Matt Layden's own sheet layout; this leaves bulkhead #3, drawn at 1214 mm wide, a tight fit against the local sheet size; has not yet started the full-size build but has a 1:5 scale model in aircraft ply well advanced, and is finishing CNC files to cut full-size parts via a local CAD cutting service; offers to make the CNC DXF files available to Dave and Mindy Bolduc for distribution alongside the plans.
[37] Archive message page_2226 (shersey / "shersey.rm" / Shane Hersey, `paradoxbuilders`, msgnum 2253, 2004-09-02) — "Re: Digest Number 575": asks whether John Hall has a workaround for the plywood-size mismatch besides using imported ply; identifies Gaboon as Okoume (Aucoumea klaineana), aka Samara, a West African hardwood possibly harvested from old-growth or rainforest sources, and says he would prefer a local, sustainably sourced ply species if one exists.
[38] Archive message page_2232 (johndhall / "jdmhall" / John Hall, `paradoxbuilders`, msgnum 2259, 2004-09-05) — "Re: Digest Number 577": answers Shane — using local ply means reworking bulkhead #3 in two parts with a scarf on the bottom section; the left-hand side panel on drawing 6 also will not lay out as dimensioned, though the right-hand panel has enough spare material to make up the shortfall on a 2400 mm sheet; the aft bottom panel is also slightly shy on width near the chine runners; Gaboon avoids all these problems but raises the sourcing concern Shane flagged; has been considering Hoop Pine (decent multiple veneers, better made than Gaboon in his opinion) or, as a cheaper but more toxic alternative, Proof Ply (glues and paints well but loaded with CCA or similar). Signed "John, 41.5 South 147.1 East."
[39] Archive message page_3885 (mbolduc / "boldav38" / Dave Bolduc, `paradoxbuilders`, msgnum 3917, 2006-08-26) — "Spline weights for lofting on Ebay": points out an eBay listing (item #110025009760) for a set of six lead-duck spline weights, 6¼ in long, about 3½ lb each, lead in a thick plastic coating with a flat-ish base and a threaded front hole for a hook; paid $21.06 for his own set, has seen others go as high as $60; also notes plans for casting a set from scratch at `splineweights.com/makeyourown.htm`. Signed "David."
[40] Archive message page_3886 (DBoboc9556, `paradoxbuilders`, msgnum 3918, 2006-08-25) — "Re: Spline weights for lofting on Ebay": jokes that publicizing the listing will now drive the winning bid up to $60. Signed "Dave B."
[41] Archive message page_3887 (mbolduc / "boldav38" / Dave Bolduc, `paradoxbuilders`, msgnum 3919, 2006-08-26) — "Re: Spline weights for lofting on Ebay": doubts many people actually want lead ducks; advises bidding what one thinks is fair and waiting for a later auction if it doesn't hit, since the seller has more sets.
[42] Archive message page_3888 (azskybum / Curtis, `paradoxbuilders`, msgnum 3920, 2006-08-26) — "Re: Spline weights for lofting on Ebay": had bid on the sets himself; notes the ones that sold for $60 probably didn't need the splines screwed in, and that solid-lead ducks are pricey to ship. Signed "Curtis." Same established below-threshold correspondent (Phoenix, Arizona) tracked at [references/paradox-uk-website.md](/references/paradox-uk-website.md#a-uk-and-worldwide-build-count).
[43] Archive message page_3889 (mbolduc / "boldav38" / Dave Bolduc, `paradoxbuilders`, msgnum 3921, 2006-08-26) — "Re: Spline weights for lofting on Ebay": shipping ran $14.26 NJ to NC; these particular sets have sold from $20 to $61; picking up old discarded tire-balance weights or fishing sinkers lets a builder cast a set for almost nothing — used this method himself to cast small pigs of trim ballast for Swamp Thing; the splineweights.com ducks are probably a little nicer than the eBay ones but cost much more; points to a photo of Matt Layden's own construction progress (`physics.bgsu.edu/~layden/FunStuff/Boats/Matt_Boat/05-02-12.htm`) showing Matt using ducks that look much like the splineweights.com ones.
