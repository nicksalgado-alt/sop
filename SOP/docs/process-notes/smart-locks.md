# Smart Locks

Seed notes for smart lock estimating.

Use this as a working note, not a final SOP.

## Things That Commonly Matter

- battery handling or replacement
- cosmetic inspection standard
- firmware reset or device testing
- missing accessories
- packaging complexity
- damage caused by mounting hardware or door use

## Questions Claude Should Consider

- Does the product need functional testing beyond visual inspection?
- Is there a common refurbishment path for cosmetic wear?
- What percentage of units are expected to be damaged versus sellable used?
- Are there category-specific shipping or storage concerns?

## Lockly-Specific Notes

- Product line: Secure Pro ($310), Vision Elite ($430), Secure Plus ($230), Affirm ($180), Styla ($700), **Visage** (facial recognition, ~$350+)
- Weighted avg MSRP: ~$289
- Estimated 180K units/year sold (1.5% of smart lock market)
- Return rate: ~10%
- Key refurb steps: battery test/replace, firmware reset (clear owner data), keypad/fingerprint test, motor cycle test, BLE/WiFi connectivity check, cosmetic refurb
- Hard fail modes: motor failure, board damage, water intrusion, battery leak
- Parts harvest value: batteries, mounting hardware, keypads, strike plates

## Lockly Visage Repack SOP (from video — PGK728WR)

- **Video-observed repack time**: 2:37 (training pace), production steady-state estimate: 1:30–1:45
- **Process**: Unbox → lay out all components → verify accessories against printed tray diagram → repack accessories into blue tray → assemble foam + tray + lock bodies + strike plate into retail box → add documentation → close retail box → place into shipping carton
- **Component count**: 12 distinct items (exterior body, interior assembly, strike plate box, WiFi sensor kit, touchscreen cover, USB cable, 3+ hardware bags, activation card, installation locator kit, manual, support card)
- **Critical check**: Accessory completeness against the blue tray printed layout — this is the go/no-go for NTF repack
- **No functional testing** in repack SOP — NTF path only (sellable condition)
- **Activation Card** has unique QR code per unit — must stay matched to device
- **See detailed SOP**: [lockly-visage-repack-sop.md](lockly-visage-repack-sop.md)

## Update Guidance

When a smart-lock estimate is reviewed, add the useful lesson here if it is broadly reusable.
