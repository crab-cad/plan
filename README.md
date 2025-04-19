## Integration
- Use rita for geo-3d and csgrs triangulation
- Use geo-3d for csgrs polygon

## [rita](https://github.com/glennDittmann/rita)
- Non-planar 3d triangulation
- Remove need for cxx
- Add fuzzing and benches
- Make logging and timing optional

## [csgrs](https://github.com/timschmidt/csgrs)
- Make all tests pass
- Make offset 3d
- Add benchmarks

## [geo-3d](https://github.com/TimTheBig/geo-3d)
- Fix polygon methods
- Make all tests pass

## new crates
Note this is not a promise.
- `polygon-rand` to generate random valid polygons for fuzzing in the rest of the crates
- `gcode-rs` a standard enum with serializer traits, for slicers to use and other crates to implement for different formats and firmwares
