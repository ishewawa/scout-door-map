# Hold list for next season

Ideas saved during the 2026 delivery season. Not built yet.

## Payment reminder texts (Brandon's idea, Nov 24 2026)

For customers who haven't paid and have a phone number on file, add a way to text each one with a single tap. The texts go out one at a time but take one tap each.

Draft message:

> Hi! Your wreaths from [scout] are in and we'd love to bring them by. Our records show the order isn't paid yet ($[amount]). You can pay on Venmo at @ausakis: [venmo link with amount and note]. If you'd rather pay with cash or check, just reply to this text and let us know.

Notes for building it:
* Use the phone's own Messages app (an sms: link with the message filled in), so it comes from our real number and they can reply. No paid texting service.
* A "Text unpaid" list in delivery mode. It shows each unpaid house with a phone number and one Text button per person, and marks who has already been texted and when.
* Fill in the amount owed and the Venmo link (same link the Venmo QR uses).
* Let us edit the message wording once in Settings.

## Accounts for other families (pack beta)

Let other families sign up and run their own map.

* Each family gets its own separate space in Firebase. One family can never see another's data.
* Sign up screen with email and password, plus password reset.
* Firebase rules lock each family to their own space.
* Invite your own helpers (spouse, grandparents) into your family's map.
* Move our current data into our family's space without changing anything.

### Master account (Brea)

Brea's account can see every family's map.

* Firebase rules give one admin email read access to all family spaces. Decide whether it can also edit.
* In the app: a family switcher only Brea sees, plus a pack overview with totals per family and the whole pack.
* Families should be told up front at sign up that the pack admin can see their map and customer info.
* Look only (decided). No editing other families' maps.
* Overlay instead of switching (Brea's preference): a toggle shows other families' houses on top of her own map, the same way past seasons overlay now. Other sellers' houses use the normal status colors, drawn faded with a dashed outline so they never look like Brea's own. Tap a house to see the family name. A search lets Brea highlight one family in a bright color. Tapping their house shows the details read only; her own houses stay fully editable. Houses marked by two families get flagged so double knocks are easy to spot.
* The overlay is invisible to everyone but Brea's account.
* First sign in after creating an account: one scroll and accept terms page. It includes a short, plain line that the Door Map admin can access all map data, including customer info, to run and support the app. The overlay itself isn't described.
* The overlay updates live: houses other families mark while selling or delivering show up within seconds.
* Live location stays inside each family. Phones in the same family see each other, like Brea and Brandon now. No pack leader accounts, and no admin view of other families' locations.
* The overlay shows every status other families mark (Not home, No, Come back, sold, and so on), with the time. Brea can still knock and mark her own status on the same house; her marks are separate from theirs. Open question: whether a house a family already sold to should look different, to avoid a second pitch to the same customer.

## Ready to go setup for new families

New accounts start fully set up so nobody has to configure anything:
* Statuses: Yes bought, Donation, No, Not home, Come back, Took my number, with the same colors as Brea's map.
* Products and prices: copied from Brea's current list (wreaths, garlands, etc.), updated each season.
* Current season already created and active.
* Core statuses are locked so the overlay reads the same across every family. Families can add their own extra statuses.
* Products are fully editable per family (Brea's decision): add, remove, rename and reprice items, since other packs may sell different things door to door. Brea's list is only the starting point.

## Open to any group, not just scouts

Kids in gymnastics, sports teams, schools and churches sell wreaths door to door too. Make the app work for any fundraising group:
* At sign up, ask what kind of group (Scouts, sports team, gymnastics, school, church, other) and the group's name.
* Neutral wording everywhere: "Seller" instead of "Scout" in the picker, "group" instead of "pack". Scout families can still see scout wording.
* Consider a name that isn't scout only (Door Map already works).
* One overlay covers every seller on the app, whatever their group (Brea's decision). No grouping or filtering by organization needed.

## Sign up details

* Sign up asks for: email, password, family name (shown on the map, like "The Smith Family"), group type and group name. The email is never shown as a name.
* Family name and group can be changed later in Settings.
* Families never see the overlay or any color assigned to them; nothing about the overlay appears on their side.
