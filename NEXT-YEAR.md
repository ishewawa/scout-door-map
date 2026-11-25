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
* Overlay instead of switching (Brea's preference): a toggle shows other families' houses on top of her own map, the same way past seasons overlay now. Each family gets its own color, with a list to turn families on and off one at a time. Tapping their house shows the details read only; her own houses stay fully editable. Houses marked by two families get flagged so double knocks are easy to spot.
