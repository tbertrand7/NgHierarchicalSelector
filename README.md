Angular tree-selector directive
=======================================

Hierarchical (or tree) selector for AngularJS. It can either have the whole data structure (a tree) passed to it or set to asynchronously load each level via a callback. It also allows auto-complete searching of the tree, optional multiple selection and keyboard navigation.

### Features
- Select data from a hierarchical/tree structure
- Asynchronously or not
- Includes auto-complete/type-ahead (configurable to hit your service)
- Keyboard navigation

### Check it out
http://lukemurray.github.io/NgNierarchicalSelector/

### Release notes
v0.2
  - Async support for loading items in the tree. See load-child-items attribute

v0.1.1
  - Prevent keyboard navigation from scrolling the page

### TODO
v0.3
- bugs
  - multi-select, lots of tags multi line
- Tests
  - yep, should be writing these
- Docs
  - configuration
  - customisation
- general
  - set up some repeatable way to do a release
  - add to bower
  - set up CI for the project
- async
  - show loading indicator if it takes awhile (hasn't loaded before they expand)
- input control
  - drop-down button for tree selection (configurable)  
- tree
  - option for parent select selects all children

v0.4
- autocomplete typing
  - allow typing at the end of the selected items
  - auto complete list for typing
  - no typing at the end if item selected and not multi select
  - support async for auto complete
- input control
  - remove selected items by keyboard

v0.5
- tree
  - disabled items
  - option for no check boxes in multi select?
  - keyboard, left on a chile node should make the parent the active node
- popup
  - better positioning of popup when at bottom/edges etc.

# Requirements
- AngularJS 1.3

## CSS
.expando - Change the expand marker style
.expando-opened - Change the colapse marker style

## ng-required directive

# Contributing
Do it.

## Building
Gulp is used to build the project.
- `gulp build` will build is for local development
- `gulp release-patch` will bump the version and build a release version
- `gulp release-minor` will bump the version and build a release version
- `gulp watch` with run 'build' and watch for changes

## Testing
