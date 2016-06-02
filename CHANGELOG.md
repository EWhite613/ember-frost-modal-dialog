# 2.1.1

* **Changed** dialog footer buttons from a fixed width of `150px` to have a minimum width of `150px`.

# 2.1.0
## Non breaking changes
- added perfect scroll in the root addon for dialog content.
- updated header+footer styles for scrolling
- using ember-prop-types 

# 2.0.0
## Changed
- BREAKING Using [ember-remodal](http://sethbrasile.github.io/ember-remodal/) addon to simplify modal dialog support. Additional modal-dialog template options required

## Removed
- BREAKING Removed liquid-fire modal code. 
  - Removed the need to configure the router.js file

## Upgrade notes
If you are upgrading your app to use this version, note the following - 
- Remove the modal declaration from your router.js file
- Remove `{{liquid-modal}}` template code if you do not have any other liquid-fire modals in your app
- Apply `remodal-bg` class to the parent container where you want a blur effect on the modal overlay.
- `frost-modal-dialog` root template must use block-slots with `target` and `body` slots. See README for more details.
