# Changelog for polysemy-zoo

## 0.4.0.1 (2019-07-10)

- Fixed an erroneous lower bound in the tests

## 0.4.0.0 (2019-07-10)

### Breaking Changes

- The semantics of `absorbWriter` are now aligned with the `MTL` implementation

### New Effects and Interpreters

- Added `SetStore` effect
- Added `Floodgate` effect
- Added `Final` effect, together with submodules of interpreters using it
    (thanks to @KingoftheHomeless)
- Added `lookupOrThrowKV`, `existsKV` and `modifyKV` actions to `KVStore`
- Added Redis interpretations of `SetStore` and `KVStore`

## 0.3.0.0 (2019-06-17)

- Removed `Polysemy.MTL`
- The machinery for MTL absorption is now monomorphized in
    `Polysemy.ConstraintAbsorber`. See the documentation there and in submodules
    for more information.

## 0.2.0.0 (2019-06-14)

- Removed `Polysemy.RandomFu`, which is moving to its own package
- Add explicit cabal bounds for dependencies of `polysemy-zoo`

## 0.1.2.1 (2019-06-12)

- Update the tests to run against `polysemy-0.4.0.0`

## 0.1.2.0 (2019-06-01)

- Added `Polysemy.MTL` for inter-op with MTL (thanks to @adamConnerSax)
- Moved `Polysemy.Random` from `polysemy`
- Added `Polysemy.RandomFu` (thanks to @adamConnerSax)
- Added `fixedNat` and `fixedNat'` to `Polysemy.IdempotentLowering` for working
    with higher-order effects.

## 0.1.1.0 (2019-05-22)

- Added `Polysemy.IdempotentLowering`


## Unreleased changes
