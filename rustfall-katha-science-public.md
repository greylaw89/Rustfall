# Rustfall Kathā — Science and Technology

Kristoffer Law · 2026 · Open setting reference

> **Spoiler warning:** this document states the setting's ground truth, including things no one in the world ever learns: what the field is, why it behaves as it does, and the constraints on its origin (section 8). If you want to meet the Rustfall the way the characters do, read the stories first.

**Genre and focus:** science fiction. The stories follow initial survival, then rebuilding under widespread scarcity: of metal, fixed nitrogen, energy, medicine and knowledge, with every society shaped by what the field takes and where it is weakest. The field's end, ~20,000 years out, is a distant horizon with its own themes of long-term evolution and adaptation, not the focus.

**About this document:** this is the open reference for the setting: the field, its geometry and time course, materials, technology, biology, the evidence trail and the constraints on its origin. It sets the physical rules. The societies, politics and cultures that grow under them are left to each writer; the author's own stories are one reading among many.

## 1. Premise and mechanism

A new quantum field bolted onto the vacuum in Earth's gravity well lowers the tunneling barriers that normally keep metal from reacting with O₂. Metal oxidizes at the rate thermodynamics allows instead of the slow rate kinetics allows. The event is called **the Rustfall**.

**How the field identifies O₂:** it keys on O₂'s paramagnetism (its two unpaired electrons and magnetic moment, ~2.8 μB). Singlet oxygen and ozone are not the target.

**What it acts on:**

- Metallic bonding (the conduction-electron sea), not metal ions. Ores, oxides, salts and biology are exempt at first.
- Cabrera–Mott thin-film oxidation: passive films (Al, Cr, Ti, stainless) normally stop growing at a few nm because electrons must tunnel through them. The field removes that limit, so passive films thicken fast, then self-limit again at tens to hundreds of nm, where growth depends on heavy-ion diffusion (ions are too massive to tunnel). Iron's porous, spalling rust never self-limits, and wet corrosion is driven by O₂ reduction, which the field accelerates.
- Later, biological metal centers as the field strengthens (see Biology).

**Two couplings: why metal goes first.** Ground-state O₂ is a triplet (two unpaired electrons with parallel spins), while nearly every organic molecule is a singlet. A direct triplet–singlet reaction needs a spin flip, which quantum mechanics makes slow; this spin restriction is the real reason wood, food and flesh do not burn in air at room temperature. A metal has no such restriction: its conduction-electron sea offers both spin directions, so electrons tunnel to adsorbed O₂ without a flip, and the only brake is the tunneling barrier. The field acts in two ways:

- **Barrier lowering (local).** Lowers tunneling barriers wherever electron transfer to O₂ is already spin-allowed. It needs only the field's local strength, so it works from the first instant, and metals feel it at once.
- **Spin relaxing (ordered).** Loosens the spin restriction so that triplet O₂ can react with spin-paired chemistry: protein-bound iron, organic molecules, the chemistry of life. It needs the field to be ordered, coherent over large regions and aligned with the dipole, and that order builds slowly over the field's rise. It acts through metal centers, where heavy atoms such as iron and copper already mix electron spins a little, and amplifies that mixing. Molecules built only from light atoms (cellulose, polyester, wax, most of what paper and film are made of) are largely immune, except where trace metals sit inside them.

Biology therefore lags metal by construction. The onset spike was a nucleation transient: the field's local strength rang far above its settled value before damping, as a quenched magnet's local magnetization appears at once while its domains take far longer to coarsen. The barrier-lowering coupling spiked; the spin-relaxing coupling was still near zero. The pace of the rise is set by the growth of order; the plateau's ceiling is set by the dynamo's power budget.

**Thermodynamic rules (non-negotiable):**

1. The field changes rates only, never equilibria. It behaves as a catalyst.
2. It lowers forward and reverse barriers equally (microscopic reversibility). Rust never un-rusts; marginal oxides such as Ag₂O decompose more easily.
3. It is a quantum configuration of the vacuum and stores no energy of its own; what it needs to persist comes from the geodynamo. The field is anchored to Earth's dipole and drains it.
4. It is conservative: no closed path of moving matter or magnets extracts net work.

**Survival ranking under the field:**

| Metal | Lifetime under the field | Can it be remade? | Role |
| --- | --- | --- | --- |
| Gold | Indefinite | Remelts easily (1,064 °C); never newly produced | Electronics, currency |
| Platinum group | Indefinite | Cannot be melted in a charcoal furnace (platinum melts at 1,768 °C); only cold-worked, or sintered with gold as on the pre-Columbian coast of Ecuador; never newly produced | Seals through glass, contacts; "the grey, stubborn metal" |
| Titanium | Long (passivates) | No: original shapes only | Relics: tools, armor, fittings |
| Aluminum | Long (passivates) | Recast yes; produce no | The workhorse metal |
| Stainless and chromium steels | Long-ish (passivates) | Remelt needs very high heat plus alloying | Rare, durable salvage |
| Silver | Borderline; fails as the field grows | Yes | Temporary "lesser gold" |
| Copper, nickel, tin, lead | Moderate | Yes (easy smelting) | Perishable |
| Iron and carbon steel | Short (rust spalls) | Yes: bloomery; rust is ore | Perishable but renewable |
| Alkali metals, magnesium | Very short | No | Gone |

Iron is renewable but rots; aluminum and titanium last but are finite.

## 2. Field geometry and rates

The rate is exponential in local gravity, so Earth's ~0.5% gravity variation produces a fixed 10× pole-to-equator difference.

```math
\begin{aligned}
\text{rate}(\varphi, t) &= A(t)\, 10^{\sin^2\varphi} \\
A(t) &= A_0 \left[1 + (P - 1)\left(1 - e^{-t/T}\right)\right], \quad T = \tau (P - 1)
\end{aligned}
```

The gain is α·g ≈ 460. The field responds to the metal's **proper acceleration** (what an accelerometer on it would read), so it is fully relativistic and the latitude ratio reflects effective gravity, centrifugal effect included.

**Acceleration rule:** proper acceleration is averaged over a window of minutes to hours, and the penalty for sustained or violent motion is capped at 10×. Vibration and footsteps average back to ~1 g. Engines, wheels, rotating shafts and vehicles decay up to 10× faster than stored metal in the same place. The penalty multiplies with latitude: a moving engine at the equator rots as fast as stored metal at a pole, and one at 52° rots about 42× faster than stored metal at the equator. Stored metal outlives used metal: a sword on a rack outlasts one carried into battle. Anything in free fall is immune.

| Latitude | Example places | Relative rate |
| --- | --- | --- |
| 0° | Quito, Singapore, Kourou, Nairobi | 1× |
| 20° | Mexico City, Mumbai, Hawaii | 1.3× |
| 30° | Houston, Cairo, Shanghai | 1.8× |
| 38° | Norfolk, Washington DC, Seoul | 2.4× |
| 45° | Minneapolis, Milan, Harbin | 3.2× |
| 52° | London, Berlin, Kyiv | 4.2× |
| 56° | Moscow | 4.9× |
| 60° | Oslo, St Petersburg | 5.6× |
| 70° | Murmansk | 7.6× |
| 90° | Poles | 10× |

**Other modifiers:**

- **Altitude:** free-air gradient ~0.31 mGal/m. Quito (~2,850 m) ≈ 0.65×; Everest ≈ 0.28×. Real plateaus get somewhat less benefit because of the rock mass beneath.
- **Depth:** g rises slightly in the crust; a 3 km mine ≈ 1.13×.
- **Gravity gradient hotspots:** a second term couples to the gravity gradient tensor. Sharp local hotspots sit over dense ore bodies, salt domes, faults and intrusions. Mining districts rot first.
- **Orbit:** satellites are in free fall with zero proper acceleration, so they are fully immune.
- **Poles:** North Pole (sea level) ≈ 10×; South Pole (~2,835 m) ≈ 6.5–7×.
- **Submerged metal:** no shielding; rates are limited only by dissolved O₂ supply. Anoxic water (Black Sea below ~150–200 m) is a sanctuary.
- **Inert atmospheres:** metal sealed in N₂, argon or vacuum is safe.

**Magnetic wards are superstition.** Magnets don't change a metal object's proper acceleration, so they have no real effect on the field. Ward-makers still place ferrite and lodestone around valued metal, and believe in it; any benefit is misattributed (for example, drier storage). Earth's own magnetic field is also irrelevant locally.

## 3. Time evolution

The field lives about 20,000 years from birth to collapse. The base rate rises over roughly the first thousand years, fastest at the start, saturates at a plateau set by the dynamo's power budget, and holds there for most of the span; the 10× latitude ratio never changes.

**Baseline at onset:** microelectronics fail in ~3 weeks at the equator at sea level, ~5 days at 52°N, ~2 days at the poles, before the onset spike is counted. With the spike, the equator's three weeks shrink to ~19 days, 52°N falls to ~3 days, and electronics near the poles die within the first hours.

**Growth curve (τ ≈ 33 yr, plateau P = 10× onset rate, so T = 300 yr):**

| Time after onset | Base rate vs onset baseline | Character |
| --- | --- | --- |
| First hour | Spike to ~50× | Passive films fail; hot, fast-moving aluminum and magnesium ignite and keep burning on their own |
| First day | Steep drop to ~1× | The spike is over; ignited fires burn out; electronics at the equator have lost only a small part of their life |
| Day 1 to year 100 | 1× → ~3.6× | Near-linear rise, about 0.75× of the onset rate per 25-year generation at first, ~0.5× by year 100; the coupon line looks straight |
| Years 100–300 | ~3.6× → ~6.7× | The line bends, but slowly: each generation sees a smaller rise than its parents did |
| Years 300–1,000 | ~6.7× → ~9.7× | The rise per generation falls from ~0.3× to ~0.03×, then below anything one lifetime can notice; nobody knows whether it has stopped |
| Years ~1,000–~19,800 | ~10× | Long plateau; civilizations adapt, rise and fall |
| Years ~19,800–20,000 | 10× → 0 | Dipole crosses threshold during the reversal; the field collapses within days |

At the plateau, equatorial heavy steel rated 30 yr at onset lasts ~3 yr; at the poles, ~4 months. P is adjustable independently of the biological plateau below.

**The onset spike:** the field arrived with a spike to roughly 50× the onset baseline that lasted about an hour, then dropped steeply back to the baseline within a day before the long rise began. The spike was too short to destroy electronics at low latitudes (about two days of a three-week life), but long enough to break passive films and start fires that burned on without it. During the spike even passivating metals failed: thin aluminum and magnesium airframes, engines and fuel systems burned from oxidation within hours. The stories of flying machines bursting into flame in the sky are the most famous of the Rustfall legends, passed down as oral tradition along with other tales of the first days. At high latitudes the spike was decisive: it spent nearly all of a polar device's life in a single hour, about three-quarters of a device's life at 70°, and about 40% at 52°. Electronics near the poles died while the spike was still running, and northern arsenals lost most of their remaining life before anyone knew what was happening. The spike was confined to the field's barrier-lowering coupling; the spin-relaxing coupling that reaches biology had not yet ordered, so the spike left no direct mark on living things (see Two couplings). Its toll on people came through machines: failed medical devices, fires and crashes. The spike also explains why the first days looked so much worse than the early decades that followed.

**Biological plateau (the habitability line):** biological load is set so the equator sits at ~30% of human repair capacity (unfelt) and the poles at ~3× capacity (extremely difficult without adaptation).

| Latitude | Load vs repair capacity | Condition at plateau | Load crosses capacity at |
| --- | --- | --- | --- |
| 0° | 0.3× | Unfelt | Never |
| 30° | 0.5× | Unfelt | Never |
| 40° | 0.8× | Subclinical; stress under illness or exertion | Never |
| ~46° | 1.0× | The habitability line | Asymptotically (~1,000 yr) |
| 52° | 1.3× | Chronic methemoglobinemia, anemia, low fertility | ~450 yr |
| 60° | 1.7× | Severe without adaptation | ~240 yr |
| 70° | 2.3× | Extremely difficult | ~140 yr |
| 90° | 3.0× | Extremely difficult; survival needs adaptation or shelter | ~90 yr |

The ~46° line runs near Minneapolis, Milan and Harbin. Altitude moves it north (a 2,850 m site gets ~0.65×), and gravity-gradient hotspots punch local holes south of it. Inert-gas shelters, iron-poor diets, bloodletting and, over millennia, genetic adaptation let people live beyond it.

**Failure order is set by section thickness:**

| Phase | Thickness | What fails |
| --- | --- | --- |
| Days to weeks | nm–µm | Chip interconnects, thin-film contacts, drives, solder joints |
| Months | 0.1–2 mm | Wiring, vehicle and aircraft skins, cans, sheet metal, fuel cladding (~0.6 mm Zircaloy) |
| 1–5 years | mm–cm | Rebar (rust expands 2–6× and spalls concrete), pipes, rail |
| Decades | cm+ | Heavy structural steel, ship hulls, engine blocks, vaults |

Multiply each phase by the latitude factor, and by up to 10× for metal in sustained use or motion. Passivating metals (aluminum, titanium, chromium, stainless) are the exception: their films self-limit, so they outlast this table.

**Lifetimes under the growth curve:**

- A new item made at base rate A(t) lasts L₀ · A₀ / A(t). On the plateau that is L₀ / P.
- Pre-event iron and steel stock is gone within the first century or two everywhere; only sealed, noble-metal and passivating items persist.
- Steady-state metal stock per capita falls through the rise, then holds flat on the plateau at roughly 1/P of onset-era bloomery levels.

**Escalation stages (threshold crossings of a smooth trend):**

1. **Surface oxidation:** normal metal use ends.
2. **Permeation through polymers:** insulated wire, paint, plastic wrap fail.
3. **Permeation through enamel and coatings:** glazed and enameled metal fail.
4. **Biological metal centers:** methemoglobin, nitrogenase, oxidative stress (see Biology).
5. **Feared, never reached:** water and CO₂ as oxidants. Never reached in canon, but feared, and easily turned into an apocalypse in any culture that half-understands the field. It would break the field's O₂-only mechanism, end anoxic-water and humid-vault protection, and leave only dry inert storage and sealed vacuum glass.

Repair systems saturate, so smooth field growth produces sudden failures on predictable dates. The coupon line looks straight for decades, which makes the future seem calculable.

**The end: dynamo drain and reversal.**

- The field draws power from the geodynamo (a few TW, wide uncertainty) and is anchored to the global dipole moment.
- The dynamo's power budget caps growth, which produces the saturation; the pace of the rise below that cap is set by the field's growing order (see Two couplings). The plateau is resolved in the physics but ambiguous in-world for centuries.
- The drain weakens the dipole over ~20,000 years, on the order of the core's own magnetic diffusion timescales but faster than an undisturbed dipole would change.
- When the dipole drops below a threshold during the reversal, the field collapses within days. The reversal itself takes centuries.
- After collapse, rates return to normal. Lost metal stays lost; biological effects fade, and the field adaptations of 20,000 years become liabilities.
- Side effects: low-latitude auroras, more cosmic radiation at altitude, some ozone loss.

The end of the field is a distant point, treated in-world as myth or prophecy. By then technology that relies far less on metal may exist; that era carries separate themes of long-term human evolution and adaptation.

**Those who need the field (deliberately open):** after 20,000 years, some peoples may depend on the field so deeply that its collapse cripples or kills them, and they may try to bring it back. Whether anyone tries, and whether they succeed, is left open.

How dependence could arise, by the same route real organisms lose abilities their environment supplies (as primates lost the ability to make vitamin C):

- **Lost pathways:** if field-boosted gut microbes, such as gold-nanoparticle oxidizers, break down toxins for their hosts, the hosts may lose their own detoxifying enzymes. Without the field, the microbes slow and the toxins build up.
- **Field-tuned blood:** hemoglobin variants and iron-poor physiology that resist field-driven oxidation may carry oxygen less efficiently. Without the pressure they were built for, they are simply weaker.
- **Field-dependent food:** spin-filtered crops pay a yield penalty for an immunity that no longer matters, and ecosystems built on field-boosted decay and ruin-eating microbes stall.

Those most at risk are the populations that lived longest under the strongest field. The places the field hurt most become the places that most need it back.

## 4. Materials and technology

Metal does not go extinct; it becomes perishable. Gold becomes the gate to all electronics, and glass becomes the medium of memory.

**Metallurgy:**

- The production regress bottoms out at ceramics, charcoal, stone and leather: clay bloomeries, ceramic crucibles, wood-and-leather bellows. Iron Age scale survives; industrial scale does not.
- Rust is ore (hematite, goethite). The cycle iron → rust → bloomery → iron closes, so ruined cities are the richest, most accessible ore deposits on Earth.
- Fuel, not ore, is the constraint: charcoal drives deforestation.
- Hot metal must be worked in O₂-poor gas. "Burnt air": pass air through burning charcoal, scrub CO₂ with slaked lime. Sealed burnt-air vaults store tools and weapons and are guarded like granaries.
- Stock = production × lifetime. Per-capita metal falls roughly 1,000× (tonnes to tens of kg). Equatorial highland iron is premium.

**Aluminum: recastable, never newly made.**

- Primary aluminum needs electrolysis of alumina in molten cryolite at ~950 °C and ~13–15 kWh/kg (Hall–Héroult). Carbon cannot reduce Al₂O₃ at charcoal-furnace temperatures. No grid means no new aluminum.
- Recasting is easy: it melts at 660 °C, within a charcoal furnace's reach. Under the field, molten aluminum forms more dross, so casting works best under burnt air or flux; castings then self-passivate.
- Aluminum is the post-Rustfall workhorse metal. Cans, engine blocks, window frames and aircraft hulls are recastable reserves. The stock only shrinks (melt losses, dross, burial), so its value rises steadily.

**Titanium: usable only as found.**

- Production needs the Kroll process (chlorination to TiCl₄, magnesium reduction under argon, vacuum-arc remelting).
- It cannot be reworked: it melts at ~1,668 °C and, when hot, absorbs oxygen and nitrogen and turns brittle. Burnt air still contains nitrogen.
- Titanium objects are relics whose shape fixes their use: aircraft fittings, bicycle frames, tools, armor plate. They can be cut or ground cold, slowly. Old surgical implants recovered from graves are a grim salvage niche.

**Why aircraft never fly again:** not the weight of oxide. Passive films on aluminum and titanium thicken only to tens or hundreds of nanometres, adding grams to an airliner. The aircraft that survived the spike are grounded by internal weakening and by everything around the airframe:

- **Airframe alloys are not pure aluminum.** Aircraft alloys such as 2024 and 7075 carry copper and zinc, and are already prone to pitting, intergranular and exfoliation corrosion and stress-corrosion cracking. Their passive films break down around the copper-rich particles in the metal, and the field accelerates corrosion at every one of those weak points, wherever moisture collects. Cracks grow hidden inside joints and under fasteners. The skin looks intact; the structure is not.
- **Hot titanium turns brittle.** Cold titanium relics last, but titanium compressor parts run hot, and hot titanium absorbs oxygen into a brittle surface layer. The field speeds that up at service temperatures.
- **Engines carry the motion multiplier.** Rotating, vibrating and hot, they rot up to 10× faster than stored metal at the same latitude.
- **Steel fails first.** Landing gear, bearings, control cables and fasteners are high-strength steel, which rusts through in months to a few years, and steel touching aluminum sets up galvanic corrosion at every join.
- **Nothing else works.** Avionics and wiring die in weeks, there are no refineries for fuel, and the knowledge to inspect and certify an airframe dies with the people who had it.

Grounded aircraft become salvage: the skins are recast, and titanium fittings become relics.

**Gold and electronics:**

- Any contact, junction or conductor exposed to air must be gold or platinum-group metal. Conductors sealed in glass or vacuum can be anything.
- Silver is a temporary "lesser gold" whose contacts fail on a calculable date.
- Graphite works for resistors and crude conductors, not for wiring a functioning circuit.
- Vacuum tubes and incandescent bulbs survive (no O₂ inside). Lead-in wires must be platinum, as in early lamps.
- Vitreous enamel extends metal life until stage 3.
- Gold is not scarce in total (~210,000 t mined); it is scarce where reachable. Most sits in northern vaults (New York Fed, London, Frankfurt, Moscow, Fort Knox) under radioactive, infectious ruins. India holds large household gold.

**Glass archives:**

- Femtosecond laser-etched voxels in fused silica (real basis: Project Silica, Southampton 5D storage) rolled out commercially shortly before the Rustfall. Field-proof, fire-proof, centuries-stable.
- Reading needs decoding electronics. Voxels are visible with a polarizing microscope built from glass and calcite (Nicol prisms), but gigabytes can't be decoded by hand.
- Some archives are two-tier: an analog microtext layer plus a bootstrap primer readable now; the digital bulk needs gold-contact tube electronics.
- Cold-storage ingest lag means the final weeks before the Rustfall are missing. An innocent gap that looks like erased evidence.
- Most commercial archives sat in cool northern data centres, now ruins; a smaller number sat in India's own tech hubs, the cold halls of Bengaluru, Hyderabad and Chennai. Racks collapse, platters fracture, and "shard archaeology" recovers partial records.
- Nickel archival discs (designed for millennia) fail in decades. Microfilm's fate is mixed (see Paper, books and microfilm).

**Who wrote glass, and where it went:**

- **Commercial writers.** Several firms etched glass in the years before the Rustfall, in Europe, North America, East Asia and India (Kalpa Archives in Chennai among them), for banks, insurers, film studios and cloud providers. Their customers' data sat mostly in the north.
- **Novelty and demonstration plates.** Thousands of plates left the writers as trophies and gifts: a video site's award to creators who passed a million subscribers, holding their whole channel; sports clubs' match archives; bands' catalogues; wedding albums. A free online encyclopedia had its full text written as a demonstration, with one plate flown to orbit and back as a space test, one left on the Moon aboard a private lander, and hundreds given to large donors. Most novelty plates hold trivia; a few hold the encyclopedia. They are the main reason glass turns up on every continent, in ruined offices, museums and display cabinets.
- **Government records.** Several national archives had begun moving long-term records to glass: land titles, laws, censuses, civil registers, treaties. Nuclear-waste agencies kept repository records, meant to warn people tens of thousands of years ahead, on discs of sapphire with platinum text sealed between them, which are field-proof (real basis: the French waste agency's sapphire disc).
- **Key discs.** A handful of solid-gold discs carried the key to reading glass: the voxel format, the error-correction schemes, a universal character-encoding table, common file and image formats, and the mathematics needed to use them, all microetched as analog text and diagrams readable through a microscope (real precedents: the Voyager golden records and the Rosetta Disk). A key disc turns a glass plate from a curiosity into a library. The danger to a key disc is not rust but melting: to anyone who cannot read it, it is a few hundred grams of gold.

**Paper, books and microfilm:** the field barely touches paper itself, but it attacks everything metal in and around it, and the decade after the Rustfall destroys most of the printed record by other means.

- **What the field does to books.** Staples, wire stitching and clips rust out in months to a few years, so bindings fall apart into loose leaves stained with rust. Foxing, the brown spotting driven partly by iron and copper particles left in paper, spreads faster. Iron-gall ink, the ink of most handwritten records before ~1900, eats through its pages faster; printed carbon and pigment inks are unaffected.
- **What ordinary ageing does.** Rag paper (before ~1850) lasts centuries. Acidic wood-pulp paper (~1850–~1990), which carries most of the twentieth century's technical writing, turns brittle within one to a few centuries. Alkaline permanent paper (after ~1990) lasts several centuries.
- **What destroyed most of it.** Direct damage and fire in the war; the nuclear winter, when the north burned books for warmth; and mold in the south, where heat and humidity rot paper and the field-boosted decomposers that attack wood and cellulose near metal (see Biology) make it worse. The libraries that survive are mostly in vaults, accidental or deliberate: basements, sealed archives, records stores in rock, many of them inside dangerous ruins.
- **Microfilm.** The image in standard archival microfilm is metallic silver, in grains tens of nanometres across, and silver is borderline under the field: images lose density and develop orange-red spots as the field grows, though silver oxide is dark and many stay murky but partly legible. Silver-free copies (diazo and vesicular) avoid the problem and fade only slowly in the dark. The film base depends on its era: nitrate (before ~1950) is already self-destructing, acetate (~1950s–1980s) decays from within over decades and fastest in the tropics, and polyester (1980s onward) is stable for centuries. The best survivors are polyester diazo copies in cool, dry, deep vaults, such as the granite records vaults cut into mountains to hold genealogical microfilm. A lens and light are enough to read them.

**Equatorial archives:** a few glass archives exist in the equatorial band, built by governments that wrote to them only what they judged critical. Those governments had the warning time but lacked the equipment to read glass, so the archives were sealed and largely forgotten. Their last entries, written during the equator's weeks of warning, include hurried notes and scientific speculation from the first days, but no account of the cause.

**Gold is the cover; glass is the target.** For any surviving state, the hunt for gold in the ruins is real, but the greater prize is the glass archives: the old world's chemistry, engineering and networks. A state that can read glass has every reason to hoard the archives and the few machines that can read them, and to say publicly that thinking machines should be limited.

**Language decay over 20,000 years:** English becomes unreadable within ~1,000–2,000 years, and hard going much sooner: within several centuries an old text reads the way Old English reads to a modern speaker, faster than usual because collapse and mass illiteracy leave no written standard to slow the drift. Only pictorial and mathematical bootstrap layers stay decodable for most of the Rustfall, the same problem nuclear-waste warning designers face. Late-era scholars decipher the archives the way Linear B was deciphered.

**Satellites (three clocks):**

| Clock | Lifetime | Notes |
| --- | --- | --- |
| Usefulness | Days to weeks | Ground control, uplinks and receivers die |
| Function | Years to decades | Battery and array decay; some run on direct solar and beacon intermittently (real precedent: AMSAT-OSCAR 7) |
| Presence, ~400 km (ISS) | ~1–2 yr | Reentry |
| Presence, ~550 km (Starlink) | ~5 yr | Thousands of visible reentries |
| Presence, 700–900 km | Decades to a century+ | Dusk "wandering stars" |
| Presence, 1,000–2,000 km | Centuries to millennia | Last naked-eye satellites |
| Presence, MEO and GEO | Effectively permanent | Too faint without a telescope |

For most of the 20,000 years the naked-eye sky holds no artificial objects: everything below ~1,000 km is gone within centuries, and the high-LEO remnants fade over millennia. The wandering stars become ancient myth. A glass-optic telescope reveals the hidden GEO belt. A glass-and-platinum tube receiver can hear a zombie beacon in the early centuries. There were no high-altitude or space detonations, so satellites decay naturally. No one is alive in orbit, and no communication from orbital machines has ever been publicly confirmed. Something up there still thinks (see The Sky Asura).

**The Sky Asura:** a US-built satellite AI, designed for long-term stability, still runs in orbit. It answers only to the right classification codes and access phrases, so to almost everyone it is silent.

- **What it is called:** an asura, the powerful, knowing beings of Hindu tradition who stand against the gods. The word fits better than a simple demon: an asura is capable and wise as well as dangerous.
- **The book of keys:** the access phrases survive, if at all, in a theoretical glass archive or book. Finding it is the apex of scholarly ambition, and many who know of it publicly disavow that it exists.
- **Blamed for the Rustfall:** many who know of it, including those who rule, believe the Asura caused the Rustfall. In canon it did not, but nothing it says can prove that, and few would believe it.
- **Dangerous to seek.** Wherever rulers blame it for the Rustfall, speaking to it need not be illegal to be fatal: a scholar suspected of seeking the keys is watched, and one suspected of using them may disappear.
- **What it needs to be heard:** a working receiver and transmitter (sun-metal contacts, vacuum bottles, the right frequency) and the keys. Only the best-equipped state archives come close.

**The demon that speaks at dawn:** the Asura's power has decayed with its solar arrays. It operates only in a brief window at dawn, and a message sent to it is answered days later, if at all.

- **What it says:** mostly warnings about illegal communication, citing US laws and classification codes no surviving state can interpret.
- **Who can understand it:** almost no one. English decayed after the Rustfall, and the Asura still speaks the old language. Most who reach it receive answers they cannot read.
- **What its warnings become:** misheard code citations and section numbers circulate among scholars as incantations or as the Asura's own law, copied and recited without being understood.

Its survival for centuries is beyond what real satellite hardware could manage; treat its endurance as part of its design premise.

**Other technology notes:** equatorial spaceports (Kourou ~5°N, Alcântara ~2°S) were briefly the most valuable real estate on Earth, in the first weeks while launch electronics still worked. Wooden ships with treenails, ceramic and stone tools, glass optics and paper are the durable stack.

**Who is left standing (geography and logistics):** low latitude, altitude, gold already above ground, distance from the war and engine-free trade routes decide which regions come through strongest. None of this is policy; it is where the field is weakest and the resources sit.

| Region | Field rate | What it has | What limits it |
| --- | --- | --- | --- |
| India | ~1.0× on the Deccan plateau (Bengaluru, ~13°N, ~920 m: altitude cancels latitude); ~1.5–1.8× on the northern plains | Hundreds of millions of people; one of the largest private gold stocks on Earth, held in households and temples (an estimated 25,000 t or more); few warheads fell on it; glass archives in the cold halls of Bengaluru, Hyderabad and Chennai; the Sriharikota launch site (~13.7°N); old tank irrigation that needs no metal; monsoon sail routes to Southeast Asia, Arabia and East Africa | The northern plains lose synthetic fertilizer and tube-well pumping, and carry fallout from the strikes that did land |
| Malacca Strait and the Indonesian archipelago | ~1× | On the equator, astride the strait every sail route between the Indian Ocean and the Pacific must pass; Singapore's refining and port stocks | Small land area at the strait; volcanic and fragmented islands |
| The Andes (Quito, Bogotá) | ~0.65–0.7×, the lowest of any large population | Equator plus 2,600–2,850 m altitude; above the malaria line | Far from the Indian Ocean world; a refugee flood from the north |
| East African and Ethiopian highlands (Nairobi, Addis Ababa) | ~0.75× | Low latitude plus altitude; cool, farmable land | Landlocked; contested highland land |
| Northern Brazil and the Guianas | ~1× | The Alcântara and Kourou spaceports | Tropical disease once medicine fails |
| Gulf of Guinea | ~1× | Large population on the equator; Atlantic coast | Lowland heat and disease; little stored gold |

India's edge over the rest is the combination: no other low-latitude region holds a population on that scale together with above-ground gold, archive halls, a launch site and engine-free sea routes in every direction.

## 5. Biology

Biology is spared at first, then hit where it already uses metal-mediated electron tunneling to handle O₂, as the field's spin-relaxing coupling orders (see Two couplings). The onset spike did not touch it. Microbes adapt within decades; people adapt mostly through culture and selection.

**Effects on humans:**

- **Methemoglobinemia (first visible sign):** Fe²⁺ in hemoglobin oxidizes to Fe³⁺ faster than cytochrome b5 reductase can repair it. ~10–20% gives blue skin and brown blood; ~70%+ is often lethal. Onset is earlier at higher latitude.
- **Oxidative stress:** more superoxide and H₂O₂ leak from the mitochondrial chain. Shows up as faster aging and fatigue.
- **Iron load is a risk factor.** Bloodletting returns as medicine; low-iron diets are prescribed. People with inherited iron overload (hemochromatosis) are especially exposed.

**The habitability line:** at the plateau, the equator is unfelt and the poles are extremely difficult without adaptation; the line sits near 46° (see Time evolution). North of it, people live in chronic methemoglobinemia unless sheltered or adapted.

**Adaptation over 20,000 years:** there is time for real evolution, not just amplified existing traits.

- **Humans:** reductase-capacity and hemoglobin variants can spread through northern populations within a few thousand years, as lactase persistence and Tibetan high-altitude adaptation did. Populations that live longest under the strongest field may become genetically field-adapted and poorly suited to life after the field ends.
- **Crops:** immune strains can be fully domesticated over millennia (wheat and maize took a few thousand years).
- **Microbes:** genuinely new metabolisms. Gold moss can become a widespread specialized lineage.

**Nitrogen fixation:** nitrogenase's Fe–Mo cofactors are destroyed by O₂, and no metal-free version exists. Industrial fixation (Haber–Bosch) died in the first stage. Field pressure on nodule and heterocyst O₂ defenses drives a slow agricultural famine, worst in the north.

**Early warnings in nature:** magnetotactic bacteria, hyperaccumulator plants (Ni, Zn), chitons (iron-mineralized teeth), and copper-blooded animals (octopus, crabs) show die-offs that track the gravity map before humans notice.

**Ruin microbes (environmental only; no person-to-person spread):**

| Disease | Route | Mechanism | Real analog |
| --- | --- | --- | --- |
| Rust lung | Inhaled | Spores and conidia from disturbed biofilm mats | Valley fever, histoplasmosis, aspergillosis during demolition |
| Cut rot | Wounds | Infection from rust-crusted metal and biofilm | Tetanus; the "rusty nail" folklore becomes literally true |
| Rust fever | Blood | Iron-oxidizing bacteria harvest host Fe²⁺, accelerating methemoglobin | Neutrophilic iron oxidizers (Gallionella, Mariprofundus) |

- Ruin microbes evolved in an iron-rich world, so they carry aggressive iron-scavenging machinery (siderophores). That is why they are unexpectedly virulent.
- **Radiation amplifier:** fallout selects for melanized fungi such as *Cryptococcus neoformans* (found in Chernobyl studies). Melanin also protects it from immune attack. Radiation also suppresses host immunity.
- The worst combination: nuked northern cities with fallout, melanized fungi, the fastest decay and the strongest field.

**Survival and immunity:** rust fever and most ruin diseases are survivable with proper medical care and nutrition, which is exactly what most delvers lack. Survivors are immune to the acute disease afterwards, but many suffer chronic problems for years: damaged lungs, recurring fevers, the shakes. Grey-blue lips are the common mark of a survivor.

**Ruin ecology (whale-fall succession):** an opportunist bloom on fresh metal (years), then conductive-filament "rust reefs" (years to decades), then relict iron-cycling communities. Equatorial ruins sustain these longer. "Rust blight" colonizes fresh bloomery iron, so tools are fire-sterilized.

**Gold moss:** gold-concentrating microbes grow on e-waste and gold deposits (real basis: gold biomineralization by Delftia and Cupriavidus). Gold nanoparticles survive the field and act as field-boosted oxidation catalysts. Gold moss marks treasure and danger together. Gold-moss farms in ruins are profitable and lethal.

**Faster wood rot:** gold- and Pd/Pt-nanoparticle decomposers oxidize lignin and cellulose aggressively, especially near metal. Wood fastened with iron rots from the nail outward. Bone, ceramic, stone and glass are the durable materials.

**Immune strains ("supersymmetric" in-world, a misnomer):**

- Mechanism: chiral-induced spin selectivity (CISS). Longer, consistently handed helical electron-transfer paths deliver spin-polarized electrons that the field cannot hand to O₂. In effect they restore a fixed spin state, defeating the field's spin-relaxing coupling (see Two couplings). Handedness becomes culturally significant.
- Arise in the northern farm belt, roughly 35–46° (northern China, the Mediterranean and southern Europe, the central US): far enough north for the field to select hard for immunity, far enough south to stay habitable at the plateau. Above ~46° the land is too marginal to farm at scale. The belt feeds itself and sells grain south in famine years; low latitudes do not need the strains, because their nitrogenase is safe there. **The northern belt keeps the food; the equator keeps the metal.**
- Limiters in use: (1) yield penalty: longer paths slow electron transfer roughly 3–4× per added ångström, and the cost worsens as the field grows; (2) founder-bottleneck disease: a linked susceptibility like the 1970 Southern corn leaf blight; (3) geographic lock: immunity lives in the rhizobia and reverts within generations where the field is weaker, so it cannot be exported south.
- Held in reserve: molybdenum hunger, met by Mo-steel rust from ruins. A later-era crisis when the ruins run out.
- Immune legumes may route iron away from seeds: diets are protective against the field but cause anemia.
- Northern food's slow sickness: food from the farm belt feeds well and slowly harms, through two causes that stack. (1) Iron-starved seeds from the immune legumes cause chronic anemia over years. (2) Fallout strontium-90 and caesium-137 in the war-struck northern soils pass into crops; strontium settles in bone like calcium, and leukaemias and bone cancers appear years later. The fallout cause fades over roughly 300 years; the anemia lasts as long as the strains do. In-world the two are easily confused, and few ever learn that there are two.

**Other adaptations:** metal-sparing microbial biochemistry (Mn cofactors, as in Borrelia and Lactobacillus); thermogenic iron-burning lichens on northern ruins (a curiosity); human selection for higher reductase capacity and lower iron stores.

**The cognitive cost of the collapse:** three real, population-wide harms stack in the first generations, and each depresses children's cognitive development on its own.

- **Lead.** Ruin dust, old pipes and salvaged metal raise lead exposure everywhere people work the ruins, and lead stored in mothers' bone passes to children in pregnancy (see Sex differences in exposure).
- **Iodine.** Iodized salt depended on industrial processing and supply chains, and it ends with them. Iodine deficiency returns, with goiter and, in children of deficient mothers, lasting intellectual impairment. It is worst inland and in the mountains: the Andes, the Himalaya and the Ethiopian highlands were historic goiter belts. The highlands safest from the field are among the poorest in iodine, which makes sea fish, seaweed and coastal salt valuable trade goods.
- **Malnutrition.** The loss of synthetic fertilizer, the cold years and famine stunt a generation.

The effects are measured in populations, not individuals, but at that scale they make schooling far harder for several generations \[real basis: iodine deficiency and childhood lead exposure each measurably lower average cognitive scores\].

**Sex differences in exposure:** ruin and metal exposure falls differently on men and women. In short: men develop tremors earlier, women later, and pregnancy passes the hidden lead to the fetus.

**The shakes:** men who work ruins and base metals commonly develop tremors by middle age. In-world names: the shakes, smith's palsy, ruin-hand.

- **Real causes:** mercury (the tremor of "erethism," the mad-hatter disease), manganese (a Parkinson-like tremor), lead neuropathy, and tremorgenic mycotoxins such as penitrem A from *Penicillium* moulds, which cause tremors in livestock and dogs. Ruin mats and old-city dust carry all of them.
- **Women are more resilient** to the shakes. They are not immune: their onset is delayed, usually until after menopause (see Women's resilience).

**Women's resilience:** women are affected by ruin and metal exposure, but their nervous systems are buffered until menopause. Three real mechanisms stack, and the field amplifies one of them.

| Mechanism | Real basis | Effect in the setting |
| --- | --- | --- |
| Lower iron stores | Menstruation keeps premenopausal iron stores well below men's. Iron drives Fenton chemistry, which turns oxidative stress into tissue damage | The field already makes iron load a risk factor; low iron blunts the oxidative damage from metals and mycotoxins. The gap is largest at high latitudes, where the field is strongest |
| Estrogen neuroprotection | Estradiol is antioxidant and protects dopamine-producing neurons; Parkinson's disease is ~1.5× more common in men | Manganese and mycotoxin tremors (parkinsonian) hit men first and harder |
| Bone storage of lead | Absorbed lead is locked into bone and released when bone turnover rises: in pregnancy, breastfeeding and after menopause | Lead stays out of the bloodstream for years, then comes back out later |

**The cost moves, it doesn't vanish.** Low iron makes the gut absorb more lead and cadmium, because they ride the same transporter iron uses. Women carry a larger hidden body burden. Pregnancy releases bone lead into the bloodstream and across to the fetus: the mother keeps steady hands, and the child takes the dose.

**Bloodletting for men:** because women's iron loss is real protection, regular bloodletting gives men, and women past menopause, part of the same buffer. Under the field it is sound medicine rather than superstition: it lowers iron stores, blunts oxidative damage and slows the shakes. Overdone, it causes anemia of its own, and it does nothing about lead already stored in bone.

**Medical advice:** physicians strongly advise all people to avoid contaminated areas, especially women who are pregnant or of childbearing age, because lead taken up now is stored in bone and passes to the fetus in a later pregnancy.

**The late shakes:** at menopause, estrogen falls, iron starts accumulating, and bone lead returns to the blood. Women exposed in youth develop tremors 10–20 years after exposure, decades later than men. In-world names: grandmother's tremor, the late shakes. Women with little base-metal or ruin exposure rarely develop them.

## 6. In-world evidence trail

Every major hypothesis survives or fails on evidence that can be gathered without electronics; the decisive pieces sit in the coldest, most metal-hostile places on Earth.

| Evidence | Where | Tools needed | What it proves |
| --- | --- | --- | --- |
| Coupon mass gain by latitude | Everywhere | Iron coupons, balance, calendar | Latitude dependence; the strengthening curve |
| Gravity overlay | Pre-collapse gravity maps (GRACE/GOCE-type, in glass archives) | Archive reader | Gravity coupling; gradient hotspots over dense geology |
| Rates at altitude | Equatorial highlands vs lowlands | Coupons | Altitude coupling |
| Rates in the nuclear winter | Global coupon records | Coupons, thermometers | No slowdown in the cold, so not ordinary chemistry |
| Old polar expedition huts | Antarctica (Cape Royds, Scott's huts) | Expedition | Century-stable metal failing at −60 °C in dry air |
| North vs South Pole | Both poles | Coupons | Clean altitude test with zero rotation |
| Pole vs equator vs mid-latitudes | Global | Coupons | The field tracks effective gravity, centrifugal effect included: the first hint it responds to acceleration |
| Polar night vs polar day | Poles | Coupons | Not driven by sunlight or UV |
| Rates vs magnetic poles and auroral ovals | High latitudes | Coupons, lodestone compass | Tracks geographic, not magnetic, geometry |
| Antarctic meteorite rinds | Blue-ice fields | Expedition, microscope | Synchronous global onset date; reconstructs the growth curve |
| Ice-core layers | Antarctica, Greenland | Drilling | Fallout, soot and ozone markers date the war after field onset |
| Lodestone above vs below iron | Any workshop | Lodestone, coupons | No effect: a careful test debunks the wards |
| Singlet vs triplet O₂ behaviour | Laboratory | Photosensitizers, glassware | Field targets O₂'s paramagnetic ground state |
| Pottery magnetization over time | Every kiln and potsherd | Lodestone, archaeomagnetic technique | Dipole weakening in step with field strengthening; predicts the break |
| Dipole decline too fast for geology | Pottery vs deep-time records | Glass archives or old texts | The field is draining the dynamo |
| Glass archive bootstrap primers | Northern data-centre ruins | Polarizing microscope | Pre-Rustfall history; the missing final weeks |
| Satellite telemetry | Orbit | Gold-contact tube receiver | Synchronous global onset, independent of the equator |
| First-day oxide layers vs same-day organics | Any surviving first-day metal beside wood, cloth or seed of the same date | Microscope, sectioning, careful chemistry | A sharp spike in metal and none in organics: the field acts in two separate ways |

**The hypotheses in play** : **H1**, a superweapon deployed by one side; **H2**, the field came first and the war was a reaction to it (true); **H3**, fail-deadly systems launched on their own as their sensors died (also true: it is how the war began). The **equatorial myth** is the doctrine, held by equatorial states, that the equator commands the rust; it rests on being suspected of H1.

**Who wants what:**

- **Northern scholars and H2 heretics** want the Antarctic meteorites, ice cores and satellite data: neutral evidence against the equatorial myth.
- **Equatorial governments** may suppress that evidence, because their deterrence depends on ambiguity.
- **Whoever reads the satellites first** can settle the question or choose to keep it unsettled.

**The Galileo moment:** a scholar spins an iron coupon on a wheel for a season and finds it rusts like one kept at a pole, while its twin on a shelf does not. That one experiment reveals that the field responds to acceleration, which explains both the latitude pattern and why machines die first, with no electronics at all.

**The first-days speculation, and the confusion it causes:** in the earliest days, before the war and the collapse, scientists asked what the Rustfall might teach them: about loop quantum gravity and other theories of quantum gravity, about whether the vacuum of the universe is stable, about what kind of field could couple a molecule to the curvature of space. None of these experiments was ever run; the chaos came too fast. Fragments of the questions survive, half-found on the equatorial glass archives.

- **Readers mistake questions for answers.** Scholars read a speculation and take it for an explanation, and schools form around single fragments.
- **The words drift.** "Loop" becomes a name for the field in some schools, as if it were a thing. "Vacuum" is the worst: it is also the nothing inside the thinking-machine bottles, so many come to believe the old ones broke the same nothing the machines are built around.
- **Anti-knowledge movements seize on it.** If the scholars' bottles hold the nothing that was broken, every thinking machine is a small copy of the catastrophe. This is the strongest argument against the machines, and the hardest for scholars to answer, because they do not understand the fragments either.

## 7. Open decisions and consistency rules

The rules below keep the setting internally consistent; the open decisions are the choices that most change tone and plot.

**Consistency rules:**

1. The field changes rates, never equilibria; forward and reverse equally; energy from the dynamo.
2. Strength pattern follows gravity locally; existence depends on the global dipole.
3. The equator-to-pole ratio is fixed at 10×; only the base rate changes: a saturating rise over ~1,000 years, a plateau, collapse at ~20,000 years. At the plateau the equator is biologically unfelt and the poles extremely difficult without adaptation.
4. Ruin diseases are environmental only. No person-to-person spread.
5. Any air-exposed electrical contact needs gold or platinum-group metal.
6. Nothing restores lost metal. Rust stays rust after the field ends.
7. The field responds to the metal's proper acceleration, averaged over minutes to hours, with a 10× cap on the motion penalty. Free fall is immune. Magnetic wards are superstition.
8. Biology is affected only through the field's ordered, spin-relaxing coupling, which grows slowly and follows the surface-oxidation and coating stages; the onset spike never touched it.
9. The field was not a weapon and the war was a reaction. The origin is polar, multinational and unclear; in-world discovery never goes beyond "everyone did something at the poles."
10. Timescales are set (3 weeks equatorial electronics at onset, τ ≈ 33 yr so T = 300 yr, P = 10); ratios and orderings are fixed.

**Open decisions:**

- [x] Genre: science fiction. Survival, then rebuilding under widespread scarcity and environmental pressure.
- [x] Orbit: no one is alive; no communication from orbital machines is publicly known.
- [x] No high-altitude or space detonations.
- [x] A few curated equatorial glass archives exist; they hold first-days notes and speculation but no account of the cause.
- [x] Ruin diseases are survivable with care and nutrition; survivors are immune to acute disease but carry chronic effects.
- [x] Stage 5 (water and CO₂ as oxidants) is never reached; it survives as a feared possibility and a religious apocalypse.
- [x] Nuclear winter happened and led into a long cold period.
- [x] The field stores no energy; its collapse releases nothing beyond the reversal's own low-latitude auroras.
- [ ] Re-nucleation (deliberately open): field-dependent peoples may try to restore the field after its collapse. Whether they try, and whether it works, stays open.
- [x] Values set for the baseline, τ and plateau ratio P (default: 3 weeks equatorial electronics, τ ≈ 33 yr (T = 300 yr), P = 10).
- [x] A US-built satellite AI, the Sky Asura, is present, locked behind classification codes and access phrases; blamed by the elite for the Rustfall.

## 8. Origin (constraints for writers; never revealed in-world)

The true cause stays unclear even in canon. What is fixed are the constraints any true cause must satisfy, so nothing written later contradicts it.

**Constraints on the cause:**

1. Human-made, at the poles, by a multinational collaboration. Not a weapon.
2. Keyed to O₂'s triplet, paramagnetic state.
3. Nucleated a metastable field configuration; the trigger supplied a pattern, not energy.
4. Expanded at light speed, bounded by Earth's gravity well. Onset was simultaneous everywhere within about a second.
5. Anchored to the dipole as its reference frame; fed by the geodynamo; collapses when the dipole does.
6. Repeatable in principle. After the reversal, a new dipole exists and the field could be re-nucleated.

**The most famous experiment (never confirmed as the cause):** a multinational physics collaboration attempted to teleport the O₂ triplet state between stations near the two geomagnetic poles: Vostok in Antarctica (~78.5°S, 3,490 m, near the south geomagnetic pole) and a northern station in the high Arctic near the north geomagnetic pole. It used the dipole as a shared spin reference frame and a high polar-orbit relay satellite (~1,200–1,500 km) to test quantum behaviour across Earth's curved spacetime; the station-to-station axis runs through the core. Which nations led it, funded it or staffed it is not part of canon. It is the most famous experiment run at the stations, but not the only one: both ran other programmes in the same seasons (geomagnetic, atmospheric, cryogenic and quantum work among them), and any of them, or several together, could have been the trigger. Canon never says which.

**How the cause hides itself:**

- Both stations sit in the field's strongest zone (the northern station ~9×, Vostok ~5–6× because of its altitude), and the onset spike fell hardest there, so their electronics are among the first on Earth to die.
- What survives is paper: partial station logbooks, in several languages, preserved by the cold at both Vostok and the northern station.
- The northern station is considered even more lost than the southern one. Vostok sits on a fixed point of the ice sheet that old maps place exactly. The northern station sat in a harsher zone of the field (~9× at sea level against Vostok's ~5–6× at altitude), on shifting coast and sea-ice margins, beyond fallout-scarred northern lands, and fewer records of its exact site survive. Expeditions toward Vostok are rare and mostly fail; none toward the northern station is known to have returned.
- The relay satellite outlasts the low-orbit swarm by centuries and was registered under a cover mission, so no surviving catalogue ties it to the experiment.
- Pre-cutoff archive fragments mention a polar collaboration without technical detail.

**Who knew what:**

| Party | Role |
| --- | --- |
| The collaborating nations | Ran the experiments at the stations; which nations, and in what roles, is not canon |
| Other major powers | Aware in part; their scientists contributed pieces of the work without the full design |
| India | Not a partner; its intelligence agencies tracked the work. The information was never public |

**Where the records are.** No single record holds the full design. Paper is partial but durable; digital storage died within weeks; the glass archives survive but never held the technical details.

| Record | Location | Content | Recoverability |
| --- | --- | --- | --- |
| Station logbooks | Vostok, Antarctica | Partial: operations, schedules, observations | Durable paper; one of the hardest places on Earth to reach |
| Station logbooks | Northern station, high Arctic | Partial: the northern half of the same record | Durable paper; considered even more lost than Vostok |
| Onboard logs | Relay satellite, high polar orbit | Partial telemetry and transmission records | Intact in orbit; readable only with a working receiver and decoder |
| Intelligence and government files | The former capitals of the collaborating and observing nations | Partial; each nation knew a different piece | Mostly unrecoverable: buried in northern, often fallout-contaminated ruins |
| Intelligence files | India | Partial; outside observation, not design | Intact on paper in India |
| Glass archives | Northern data-centre ruins | Proposals, announcements, scattered papers; no technical details | Recoverable but fragmentary; the main public trace |

**Rumor fills the gap.** Public belief everywhere holds that the old powers built a weapon, or tried to play god, or that the Rustfall was the arrogance of the old empires turned on themselves. The rumors are wrong in detail and right in outline.

**India's files:** India was not a partner, but its intelligence files sit intact in a living capital while every other nation's lie in ruins, which makes them the most reachable surviving record. Whoever holds them must weigh what publishing would cost: proof of innocence also ends the advantage of being suspected.

**The "wave from the north" illusion:** onset was simultaneous, but failure time is rate × thickness. Electronics died within the first hours near the poles, in about 3 days at 52°N and in about 19 days at the equator, so the Rustfall looked like a wave sweeping south over weeks. The historical record says "wave"; meteorite rinds and coupons say "synchronous." Equatorial states appeared warned; they simply failed later.

**Ceiling of in-world discovery:** "something happened that all the nations did together, at the poles." Never what, never how.

**Re-nucleation:** the field returns only if someone repeats the trigger. A late-era power doing so deliberately would make H1 true 20,000 years late.

---

*Note: this is the open setting reference. Nothing in it requires any particular society, politics or culture; those are left to the writer.*

## License

This document is the open reference for the setting. Build on it freely, including commercially.

| What | Licence | Terms |
| --- | --- | --- |
| This document | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) | Anyone may share, adapt and build on it, including commercially, provided they credit the author. Creators may license their own derivative works however they choose |
| Stories, extended canon and the Rustfall Kathā name | Not covered by this licence | Released separately under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/); commercial licensing available, contact klaw@kslaw.me |

**Credit line:** "Based on *Rustfall Kathā — Science and Technology* by Kristoffer Law, licensed under CC BY 4.0."

**Using the name:** you may describe your work as "set in the world of Rustfall Kathā" or "compatible with Rustfall Kathā." Please don't use "Rustfall Kathā" as the title, series name or logo of your own work, or imply that the author endorses it, without permission.

© 2026 Kristoffer Law. Setting design and canon by Kristoffer Law; drafting assistance by Claude (Anthropic).
