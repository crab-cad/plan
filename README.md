## Goals for all crates

- Support no-std and document any limitations
  - if a crate cannot support no-std document why
- The following cargo commands will be used
  - `cargo doc --open`
  - `cargo test`
  - `cargo test --release`
  - Others TBD
    - `cargo publish`
    - `cargo clippy`
    - `cargo fmt`
    - `cargo bench`
- The following platforms will be supported
  - Linux
  - MacOS
  - Windows
  - Others TDB
    - `wasm`
    - `raspberry pi`
    - `arduino`

## Integration
- Use rita for geo-3d and csgrs triangulation
- Use geo-3d for csgrs polygon
- Use zerocopy or bytemuk for free conversion
- Transfer repos:
  - [ ] rita
  - [ ] geo-3d
  - [ ] csgrs

## [rita](https://github.com/glennDittmann/rita)
- [ ] Finish the ES 3d flip algorithm
- [ ] Non-planar 3d triangulation
- [ ] Remove need for cxx, by using/making an all rust alternitive to `geogram_predicates`
- [x] Add fuzzing
- [ ] Add benchemarks, check if using nalgbra is faster
- [x] Make logging and timing optional

## [csgrs](https://github.com/timschmidt/csgrs)
- [ ] Make all tests pass
- [ ] Make offset(dilate/erode) 3d
- [ ] Make BSP intersection fully 3d
- [ ] Allow for non-planar polygons
- [ ] Add benchmarks
- [ ] Add more tests


## [geo-3d](https://github.com/TimTheBig/geo-3d)
- [ ] Fix polygon methods
- [ ] Make all tests pass
- [ ] Make relate 3d
- [ ] Redo readme

## new crates
Note this is not a promise.
- `polygon-rand` to generate random valid polygons for fuzzing in the rest of the crates
- A unified 3d visulizer to see geo-3d algorithms, rita triangualtion, and csgrs shapes and usage; with bevy and egui
- `gcode-rs` a standard enum with serializer traits, for slicers to use and other crates to implement for different formats and firmwares
