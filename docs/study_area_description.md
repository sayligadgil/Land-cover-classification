# Study Area Description

## Location
- **Area Name**: Hyderabad Metropolitan Mix (Urban-Suburban Gradient)
- **State/Country**: Telangana, India
- **Center Coordinates**: 
  - Latitude: 17.4200° N
  - Longitude: 78.4700° E
- **Bounding Box** (Approximate 25km × 25km):
  - North: 17.5325° N
  - South: 17.3075° N
  - East: 78.5825° E
  - West: 78.3575° E

## Area Characteristics
- **Size**: Approximately 25 km × 25 km (625 sq km)
- **Terrain**: Generally flat with minor undulations (Deccan Plateau)
- **Climate**: Semi-arid tropical (BSh), hot and dry most of the year
- **Dominant land use**: Urban center with suburban sprawl and peripheral open lands
- **Elevation**: ~500-600m above sea level

## Expected Land Cover Classes

### Primary Classes (5 classes - recommended for first project):
1. **Dense Urban/Built-up**: 
   - High-density residential, commercial complexes, industrial areas
   - Examples: Banjara Hills, Jubilee Hills, Secunderabad core
   - Expected spectral signature: High reflectance in visible bands, low in NIR

2. **Suburban/Low-density Urban**:
   - Residential areas with tree cover, planned layouts
   - Mixed built-up with vegetation
   - Expected spectral signature: Moderate reflectance across all bands

3. **Water Bodies**:
   - Hussain Sagar Lake (primary), smaller tanks and reservoirs
   - Clear spectral signature - high absorption across all bands
   - Easiest class to identify (validation benchmark)

4. **Vegetation/Green Cover**:
   - Public parks (Lumbini Park, NTR Gardens), street trees, institutional green spaces
   - Any agricultural patches in periphery
   - Expected spectral signature: High NIR reflectance, low red (high NDVI)

5. **Bare Soil/Open Land**:
   - Construction sites, fallow land, exposed rocky outcrops
   - Parking lots, unpaved areas
   - Expected spectral signature: Moderate to high reflectance in all bands, low NDVI

### Optional Advanced Class (if initial results are good):
6. **Transportation/Roads**: Major highways, flyovers (challenging due to spectral similarity with built-up)

## Why This Area?

### Scientific Interest:
- Represents rapidly growing Tier-1 Indian city with planned and unplanned urban expansion
- Contains distinct urban heat island effects (Hussain Sagar vs built-up areas)
- Mix of planned development and organic growth patterns
- Water bodies embedded within urban matrix (unique for Indian cities)

### Practical Advantages:
- **Local knowledge**: Familiar landmarks enable ground-truthing and validation
- **Accessibility**: Can verify classification results through field observation if needed
- **Clear boundaries**: Hussain Sagar provides unambiguous water class for accuracy baseline
- **Diverse but manageable**: 5 distinct classes with clear spectral differences
- **High impact**: Urban classification directly applicable to:
  - Smart city planning initiatives
  - Urban heat island mitigation studies  
  - Green cover monitoring
  - Infrastructure development planning

### Learning Outcomes:
- Experience with mixed urban-natural environments (real-world scenario)
- Practice distinguishing similar urban classes (dense vs sparse built-up)
- Work with clear validation targets (water bodies)
- Portfolio piece relevant to urban analytics jobs

## Validation Strategy

### Ground Truth Collection:
1. **Personal knowledge**: Landmarks and areas I recognize directly
2. **Google Earth high-res imagery**: Compare classification with recent imagery
3. **OpenStreetMap data**: Road networks, building footprints available
4. **Field verification (optional)**: Can visit specific sites if classification accuracy is questionable

### Validation Approach:
- Collect 30-50 random validation points per class (separate from training data)
- Use Google Earth time-matched imagery for validation
- Calculate per-class accuracy (expect >90% for water, >80% for urban/vegetation)
- Document any misclassification patterns (e.g., shadows classified as water)

## Satellite Imagery Requirements

### Temporal Selection:
- **Preferred season**: October - February (post-monsoon, dry season)
  - Reason: Clear skies, minimal cloud cover, vegetation still visible
  - Water bodies at normal levels (not flooded or depleted)
- **Avoid**: June - September (monsoon clouds), March - May (extreme haze/dust)

### Image Criteria:
- **Sensor**: Landsat 8 or 9 OLI (Operational Land Imager)
- **Preferred bands**: 2-7 (Visible, NIR, SWIR)
- **Maximum cloud cover**: 10% over study area
- **Spatial resolution**: 30m (adequate for urban features at this scale)
- **Date range**: 2023-2025 (recent imagery for current land cover)

### Expected Availability:
- Landsat revisit time: 16 days
- High probability of cloud-free imagery in Nov-Jan window
- Backup: Sentinel-2 (10m resolution) if Landsat has persistent clouds

## Success Metrics for This Project

### Accuracy Targets:
- **Overall Accuracy**: >85% (good for first project)
- **Water class**: >95% (should be near-perfect)
- **Urban classes**: >80% (acceptable given spectral similarity)
- **Vegetation class**: >85%
- **Kappa coefficient**: >0.80

### Deliverables:
- Classification map with 5 classes at 30m resolution
- Accuracy assessment report with confusion matrix
- Visual comparison: Classified map vs Google Earth
- Analysis: Where did misclassifications occur and why?

## Future Extensions (Post-Project)

If time permits or for future projects:
1. **Temporal analysis**: Compare 2020 vs 2024 imagery to detect urban expansion
2. **Urban heat island mapping**: Use thermal bands to correlate with land cover
3. **Green cover change**: Track vegetation loss/gain over 5 years
4. **Deep learning upgrade**: Apply U-Net or CNN for higher accuracy
5. **Sub-pixel classification**: Mix of vegetation within urban pixels

## References and Resources

### Local Context:
- Telangana State GIS: https://tgplanning.telangana.gov.in/
- Hyderabad Metropolitan Development Authority (HMDA) plans
- Greater Hyderabad Municipal Corporation (GHMC) data

### Technical References:
- USGS Landsat Collection 2 User Guide
- "Urban Land Cover Classification using Landsat" - GIS Geography
- ISRO Bhuvan portal for validation data

## Notes
- Study area selected: May 17, 2026
- Project timeline: 6 weeks (May 17 - June 27, 2026)
- Part of portfolio for GATE DA preparation and M.Tech applications
- Target: Complete before summer 2026 internship applications

---

**Document Version**: 1.0  
**Last Updated**: May 17, 2026  
**Author**: Sayli Gadgil  
**Project**: Land Cover Classification using Machine Learning