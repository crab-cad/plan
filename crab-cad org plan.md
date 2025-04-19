## Integration
- Use rita for geo-3d and csgrs triangulation
- Use geo-3d for csgrs polygon
## rita
- Non-planar 3d triangulation
- Remove need for cxx
- Add fuzzing and benches
## csgrs
- Make all tests pass
- Make offset 3d
## geo-3d
- Fix polygon methods
- Make all tests pass
## new crates
- `polygon-rand` to generate random valid polygons for fuzzing in the rest of the crates