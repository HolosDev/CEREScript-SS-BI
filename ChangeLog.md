Changelog for CEREScript-SS-BI
====

## Unreleased changes

### Add
* Implement each `crs*` instruction function
* Handling Partial Variable Index

### Change
* Change design for backpack compatibility
* Study how to handle readVP/writeVP in CERESSpool
* Use ValueContainer instead of Value
* Implement parallel `updateValuesToVT`
* Use `getValues*` instead of using `foldr` in `cacheMaker`
* Move Move `get*Cache` and `set*Cache` functions to `CERES.BI.Data.*`
* Change default GHC version and Stackage for 8.8.*
* Change default GHC version and Stackage for 8.10.*


## 0.7.0.0 -- 2020-04-XX

### Added
* Add more storage in WorldState which have NKey as a primary key
* Implement `Maker s f a` type for SI initiation

### Changed
* Move `Cache` modifier to `CERES.BI.Data.Cache.Function`
* Overhaul structures for new `NKey` storage compatibility
* Overhaul import modules and refactoring with CEREScript-SS version up (v0.16.1.0)
* Use `random-adaptor` package instead of homemade adaptor module
* Rename `HistoricTable` to `HistoricalTable`
* Revise definition of SpoolInstance
* Revise definition of CERESSpool with `Maker s f a`

### Removed
* Remove module `CERES.BI.Data.Spool`


## 0.6.0.0 -- 2020-03-28

### Added
* Implement missing instruction functions template

### Changed
* Update dependency of old CEREScript-Core 0.11.0.0


## 0.5.0.0 -- 2020-03-26

### Changed
* Update dependency of old CEREScript-Core 0.10.0.0


## 0.4.0.0 -- 2020-03-12

### Added
* Implement new `set*` and `get*` for Cache
* Define RG type and move to `CERES.BI.Type`

### Changed
* Update dependency of old CEREScript-Core 0.9.0.0
* Change old function name `get*` and `set*` to `get*By` and `set*By`


## 0.3.1.0 -- 2020-03-08

### Fixed
* Fill non-exhaustive patters
* Fix wrong localVariables is given in `runSpoolInstance`

### Removed
* Remove unused definition


## 0.3.0.0 -- 2020-03-08

### Added
* Implement `runSpoolInstance`
* Implement `runCEREScript`
* Implement `runInstruction`

### Changed
* Add PRNG generator field to `WorldState` and `SpoolInstance`


## 0.2.0.0 -- 2020-03-08

### Added
* Implement `updateWorld`
* Implement `cacheCommitter`
* Implement `siisExecutor`
* Implement `updateWorldState`
* Filter and Unwrap RW from WorldCache and apply to WorldState
* Add type `LocalCache`
* Add InternalTime fields to `World`
* Add initialLocalVariables and initialLocalCache field to `CERESSpool`
* Add constants for interpreter control variables' ID
* Add more fields to `SpoolInstance`
  * LocalState
  * Original Spool ID
  * Rest CEREScript

### Changed
* Move SIIS definition to Data
* Redesign/Rename `LocalState`, `LocalVariables` and `LocalCache`

### Fixed
* Add missing `siisExecutorSub`


## 0.1.0.0 -- 2020-03-06

### Added
* Inherit codes from CEREScript-SS
* Implement basic tree-forest aggregation algorithm
* Implement basic cacheMaker

### Changed
* Change some data and type names from original
