# Code to check seeding efficiency when using Patatrack pixel tracks 
- Forked from Wahid (https://github.com/waredjeb/ElectronPixelMatching)
- Updated code to work with CMSSW_13_0_X


## Setup instructions 

```
cmsrel CMSSW_13_0_0_pre4
cd CMSSW_13_0_0_pre4/src/
cmsenv
git cms-init
git cherry-pick 1cbb29c69bacfaefe0b6715d8d8c885b91400b5c
git cherry-pick 013581a7353f21e0d931beea7ed1398f1071c727
git cms-addpkg CUDADataFormats/TrackingRecHit
git cms-addpkg Geometry/CommonTopologies/
git cms-checkdeps -a -A
scram b -j 8
```

Then add this package to the src directory and compile again :

```
scram b -j 8
```
