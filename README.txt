SPICE SHOP — Website + Online Ordering (Curbside Pickup)
=========================================================

WHAT THIS IS
------------
Your existing Spice Shop site (same dark/gold design, Playfair + Inter,
marquee, all sections) with a full online-ordering flow built in. The
"Order Online", "Explore the Menu", and "View Full Menu" buttons — and
clicking any signature dish — open a themed ordering experience:
menu by category, add-to-cart, quantity steppers, customer details,
HST totals, and an order confirmation.

Ordering is CURBSIDE PICKUP only (no delivery).


FILES
-----
index.html            The complete website. This is the whole thing.
previews/             Screenshots of the order page and cart.
README.txt            This file.


HOW TO VIEW
-----------
Double-click index.html to open it in any web browser.
(Food photos and fonts load from the internet, so stay online.)


HOW TO PUT IT LIVE
------------------
Option A — Netlify: go to app.netlify.com/drop and drag the
           "spice-shop" folder onto the page. Live in seconds.
Option B — Vercel / GitHub: push the folder to a repo and connect it
           to Vercel, same as your usual deploy flow.


HOW TO EDIT THE MENU
--------------------
Everything is in two spots near the bottom of index.html, inside the
<script> block:

1. MENU array — each item has:
     id     unique key (also links to a photo, see below)
     name   display name
     price  number (e.g. 18.99)
     veg    true = green veg dot, false = red non-veg dot
     spice  0 to 3 (chili dots)
     desc   description text

2. IMG map — maps an item id to a photo URL. Items without an entry
   show a gold monogram tile instead. Replace these Unsplash
   placeholder URLs with the owners' real plate photos when ready.


IMPORTANT — WHAT'S NOT DONE YET
-------------------------------
Placing an order currently shows an on-screen confirmation only.
It does NOT yet save the order or notify the kitchen, because there
is no backend connected.

Next step: a backend (e.g. Supabase) to store each order and alert
the kitchen by text/email, then later payment.
