# @floating-ui/core

## 1.6.1

### Patch Changes

- fix: avoid spreading rects to support `DOMRect` types

## 1.6.0

### Minor Changes

- fix: handle CSS `:top-layer` elements inside containing blocks. It's no longer
  necessary to implement the middleware workaround outlined in
  https://github.com/floating-ui/floating-ui/issues/1842#issuecomment-1872653245.

## 1.5.3

### Patch Changes

- 4c04669: chore: exports .d.mts types, solves #2472
- Updated dependencies [4c04669]
- Updated dependencies [afb7e5e]
  - @floating-ui/utils@0.2.0

## 1.5.2

### Patch Changes

- 23f32f5d: fix(types): avoid ts 4.2+ syntax

## 1.5.1

### Patch Changes

- 88bf9768: fix(offset): avoid doubling calculation on same placement reset when
  `arrow` changes alignment of floating element

## 1.5.0

### Minor Changes

- d7e07fba: feat(arrow): add `alignmentOffset` data

### Patch Changes

- fd3c19ac: fix(flip): skip if arrow has performed internal shifting

## 1.4.2

### Patch Changes

- 0ef68ffa: fix(arrow): perform a reset if internal shifting is performed

  This allows `shift()` to continue taking action when the arrow's internal
  shifting of the floating element is performed (preventing potential
  overflow/clipping of the floating element in certain scenarios), while still
  allowing the arrow to point toward the reference when it is small if possible.

- Updated dependencies [a6c72f50]
  - @floating-ui/utils@0.1.3
