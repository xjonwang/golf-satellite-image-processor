# golf-satellite-image-processor
***
This is a golf hole recognition program that demarcates various lies (e.g. fairway, rough, trees, etc.) on a satellite image, uses those demarcations to convert satellite golf holes to a visually enhanced rendering, and supports distance calculations between the tee box or hole to any point on the map.
***
## Problem Statement
Currently, there are no affordable APIs for satellite golf course mapping (e.g. the industry-leader, Golfbert, charges $399/month). This is prohibitive to developing satellite-based data entry for golf apps. Without satellite maps, data entry takes the form of a spreadsheet, which is inconvenient and time-consuming. This adds unnecessary friction for users and prevents wider adoption.
***
### Key Requirements
* Lies should be correctly identified. The full list of lies is: tee box, fairway, rough, super rough/fescue, trees, water, bunker, and green.
* Boundaries should be correct to 4 yards (e.g. the learned boundary between fariway and rough can be 4 yards right of where it actually is). For reference, a typical fairway is 40 yards wide. 
* Boundaries should look smooth, rounded, and realistic (i.e. no jagged protrusions).
* The final rendering should be standardized and aesthetically pleasing (e.g. making all fairways a lime green to mask dead/brown spots on fairways).
* Distance calculations should be accurate to a yard (e.g. if you click on a point in the fairway, the distance calculated from the tee box can be long/short by 1 yard).
