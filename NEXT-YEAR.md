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

## Houses that bought from more than one seller

Seen in 2026: a house already had another scout's wreath on the porch when we delivered ours.
* If the other seller uses the app, Brea's card for that house says "Also bought from the Smith Family" and whether theirs is delivered yet, so a wreath already on the porch isn't a surprise.
* When selling, the overlay shows houses that already bought from someone else this season, so Brea knows before knocking.

## Rollout plan

1. Our pack first. Family accounts ready before fall sales. Demo at a pack meeting. Track families, houses, sales, double deliveries.
2. Word of mouth: den leaders, nearby packs, gymnastics and sports families. One page "how to start" with a QR code.
3. Wreath supplier, once we have numbers. Offer a free mention or logo/link only. No data access, no quick signatures; get any agreement reviewed.
* Cost: Firebase free tier won't cover hundreds or thousands of live syncing families plus photos. Reduce syncing when idle; plan for a small fee or sponsorship.

## Installing on any phone (iPhone too)

* Install helper inside the app: Android gets a one tap Install button; iPhone gets a short picture guide (Safari, Share button, Add to Home Screen).
* Works in the browser without installing, so nobody is blocked.
* Test everything on a real iPhone: location, camera, photos, Venmo link, navigation (opens Apple or Google Maps). Flash/torch likely doesn't work in iPhone Safari; fall back to brightening the photo.
* Later, if needed: real App Store and Google Play listings by wrapping the same app (Apple developer account about $99 a year, Google about $25 once, plus review).

## Door cards with a QR order form (Brea's idea, Nov 25 2026)

Leave a business card at every house that isn't home. The card has our phone number and a QR code that opens an order form. Orders flow into the app.
* Card: "Sorry we missed you!", item photos/prices or a short list, phone number, QR code. No kids' full names or home address.
* Order form (web page, phone friendly): name, address, phone, items and quantities, optional donation, pay now with Venmo link (amount filled in) or pay on delivery.
* Orders land in an "Inbox" in the app first. Brea approves each one, the app matches the address to the house on the map, and it becomes a normal order (status Yes, bought).
* Customer sees a confirmation with our phone number, so anyone who never gets their order knows who to call.
* Safety: the form can only add to the inbox, never read or change the map. Basic spam protection. Orders close on a set date.
* Optional later: mark houses where a card was left ("Card left") so we know who got one, and see which cards turned into orders.
* Also solves missing deliveries: every customer, in person or by card, ends up with our number.
* Card design (Brea): wreath photo, "Cub Scout [name] stopped by", no product list, QR code to our family's order page. One card design per scout; each scout's QR carries their name so the order is credited to them automatically (customer can still change it).
* Order page shows our products with photos and prices, address goes to that house's box on our map, Venmo link with amount filled in, or "Pay on delivery."
* Donations on the order page: give any amount, with or without buying anything. Quick picks ($5, $10, $20, $50) plus "Other amount." A donation only order still lands in the inbox, goes on their house (status Donation), and is credited to the scout on the card. Venmo link includes the donation in the total; "Pay on delivery" or "Pay when we stop by" for donation only.
* Card wording (Brea's final):
  It's Wreath Season!
  Sorry we missed you!
  Help support Ryler in Cub Scouts this year by ordering or donating. We appreciate you!
  [QR code] Scan to order or donate
  (Same card for each scout with their name swapped in.)
