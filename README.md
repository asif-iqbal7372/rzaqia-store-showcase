# Rzaqia Store

![Rzaqia Store](images/gig.png)

I own a small departmental store. I also build Flutter apps. This is not a demo
project made for a portfolio; it is the app my shop actually uses, which is why
the products, prices and order numbers in these screenshots are real.

## Why I built it

Before this app, customers phoned the shop all day to ask whether we have
something and what it costs. Orders went into a notebook. Nothing could be
searched afterwards, and the stock knowledge sat in one person's head.

What gets sold to small shops here is either a monthly subscription for a
system with fifty features a shop like mine will never open, or nothing at all.
So I built the narrow thing I needed.

## The customer side

Language switch between English, Urdu and Roman Urdu. Urdu is right-to-left, so
the layout has to flip properly, not just the words. Search matches all three
languages: "sugar", "چینی" and "cheeni" return the same product. Product pages
use photos of the actual packs that are on our shelves. Then cart, delivery
charge, and a cash-on-delivery order in a few taps.

## The shop side

Same app, different screen. Incoming orders land in a list, the owner opens one
and moves it from pending to processing to delivered, and can see the day's
total. No laptop, no admin website to keep open. The phone in his pocket is the
dashboard.

Prices and stock come from a small editable content source that I update
myself, so changing a price does not need a new build.

## Screens

| Search in any language | Owner's order list |
|---|---|
| ![Search](images/01_search.png) | ![Orders](images/02_admin.png) |

| Cart and checkout | Product page |
|---|---|
| ![Cart](images/03_cart.png) | ![Product](images/04_product.png) |

## Stack

Flutter and Dart for the app. Firebase for auth, live data and the order flow.
The three-language layer including the RTL handling is something I wrote
myself rather than pulling a package in.

## About the code

This repo has the write-up and the screenshots, no app source. The reason is
ordinary: it runs a live business, so the full code stays in a private repo. If
you want to look at the code before hiring me, ask, and I will walk you through
it on a screen share.

## Still on my list

Two things are visible in the screenshots above, so I would rather mention them
than let you find them. The tagline in the home header overflows on smaller
screens, and the add-to-cart button on the product page clips its own label
(see the last screenshot). Both are layout fixes and go into the next build.
There is no offline mode yet either.
