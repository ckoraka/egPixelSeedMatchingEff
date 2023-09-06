# Code to check seeding efficiency when using Patatrack pixel tracks 
- Forked from Wahid (https://github.com/waredjeb/ElectronPixelMatching)
- Updated code to work with CMSSW_13_0_X


## Setup instructions 

```
cmsrel CMSSW_13_0_0
cd CMSSW_13_0_0
cmsenv
git cms-init
git cms-addpkg CUDADataFormats/TrackingRecHit
git cms-addpkg Geometry/CommonTopologies/
git cms-checkdeps -a -A
scram b -j 8
```

Then add this package to the src directory and compile again. Structure should be src/SeedFromTrack/SeedFromTrackAnalyzer/.

```
scram b -j 8
```
