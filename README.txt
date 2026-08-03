# Square iPad Simple Redirect Test

This package contains two simple HTML pages for testing whether an iPad can open the installed Square Point of Sale app from a browser/FormAssembly redirect.

## Files

1. `open-square-pos.html`
   - Shows a button to open Square POS.
   - Also attempts to open Square POS automatically after a short delay.

2. `open-square-pos-button-only.html`
   - Shows only the button.
   - Use this if iPad Safari blocks the auto-launch attempt.

## FormAssembly setup

Set the post-submit redirect URL to wherever you host one of these files, for example:

https://yourdomain.com/open-square-pos.html

## Important limitation

This does not use Square's POS API checkout flow.
It only tries to open the Square POS app.

It will not:
- prefill an amount
- open a specific item/category
- create a cart
- return payment success/failure to FormAssembly
- attach the Square payment to the form submission

Staff will need to select items and complete payment manually in Square POS.
