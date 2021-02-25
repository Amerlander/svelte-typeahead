# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0](https://github.com/Amerlander/svelte-typeahead-multiselect/releases/tag/v1.0.0) - 2021-02-25

**Notes**
- **To keep this component compatible with IE11 you'll now need to polyfill `findIndex`.**

**Features**

- add `selection` props to add `selected` class on items in the result set.
- previously `selected` class was used for the active/preselected item. This gets now `active` class (see below).

**Fixes**

- don't select disabled items on keyboard navigation or if they are the first item in the result set
- keept the result set open when `focusAfterSelect` is `true`
- css for `lbael`, `input` and `input:focus` in the `data-svelte-search`-subcomponent is now scoped to this component.
- Active item holds now an `active` class instead of `selected`.

## This fork is based on [svelte-typeahead 2.3.0](https://github.com/metonym/svelte-typeahead/releases/tag/v2.3.0).
### [svelte-typeahead 2.3.0](https://github.com/metonym/svelte-typeahead/releases/tag/v2.3.0) - 2021-02-21

**Features**

- add `disable`, `filter` props to disable and filter items from the result set

**Fixes**

- bind the input element reference correctly to fix focusing behavior
- don't pass the Typeahead id to Search

### [svelte-typeahead 2.2.0](https://github.com/metonym/svelte-typeahead/releases/tag/v2.2.0) - 2021-02-20

**Features**

- add `inputAfterSelect` prop to allow user to preserve or clear the input field after selecting a result; possible values are `"update" | "clear" | "keep"` (default is `"update"`)
- add searched value to dispatched "select" event detail (`e.detail.searched`)

### [svelte-typeahead 2.1.0](https://github.com/metonym/svelte-typeahead/releases/tag/v2.1.0) - 2021-02-20

**Features**

- include `original` item and `originalIndex` in dispatched "select" event

### [svelte-typeahead 2.0.0](https://github.com/metonym/svelte-typeahead/releases/tag/v2.0.0) - 2020-12-31

**Breaking Changes**

- upgrade `svelte-search` to version 1.0.0
- defer to default `label`, `placeholder` props from `search-svelte`
- use `SvelteComponentTyped` interface in TypeScript definitions

### [svelte-typeahead 1.0.0](https://github.com/metonym/svelte-typeahead/releases/tag/v1.0.0) - 2020-11-28

**Features**

- export reactive `results` array containing fuzzy results
- add `focusAfterSelect` to opt in to focusing input after selecting a result
- keydown default behavior is preventing if pressing "ArrowUp", "ArrowDown", or "Escape"

**Breaking changes**

- `focusAfterSelect` is `false` by default
- redesigned default styles
- if using TS, Svelte version >=3.30 is required

### [svelte-typeahead 0.2.0](https://github.com/metonym/svelte-typeahead/releases/tag/v0.2.0) - 2020-11-17

- Add TypeScript definitions

### [svelte-typeahead 0.1.1](https://github.com/metonym/svelte-typeahead/releases/tag/v0.1.1) - 2020-08-06

- Remove `filter` named export

### [svelte-typeahead 0.1.0](https://github.com/metonym/svelte-typeahead/releases/tag/v0.1.0) - 2020-04-15

- Initial release
