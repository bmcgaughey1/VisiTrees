# VisiTrees
Tree species list and related assets to support visualization applications. Assets include: simple colors for species, crown and bole shape information, images for complete trees, and images for various tree parts (bark, crown, branch). The intent is to provide an open-source resource that can be used by anyone developing visualzations involving trees.

# Starting Point
The initial tree lists came from the Forest Inventory and Analysis (FIA) program and the [rSVS R package](https://github.com/Rayonier/rSVS) developed by Jim McCarter with Rayonier. FIA is responsible for the national forest inventory in the United States so their species list represents species that are measured during data collection to support the inventory. Jim's list started with the list from FIA (older version) and added additional species from the [USDA Plants Database](https://plants.usda.gov/home) maintained by the Natural Resources Conservation Service (NRCS) program. The two lists are very similar. Their differences are, most likely, not significant regarding visualization needs. One significant difference is that the rSVS list includes species group codes but the FIA list does not (for the most part). While such group codes seems useful, VisiTrees implements the same capability by providing species group level visualzation assets.

A subset of the FIA tree list that includes FIA species codes <1000 was extracted to serve as the starting point for VisiTrees. Columns were rearranged and some were deleted to create the MasterSpeciesList.

# Tree growth forms
An excellent publication by Dr. Kim D. Coder describes tree growth processes and presents the most common overall growth patterns and a set of crown shapes. Basic growth forms are:
* Abcurrent tree forms have an aerial terminal bud and leaves (palm-like).
* Adcurrent tree forms have basal buds and leaves (ground hugging yucca-like).
* Bicurrent tree forms have irregular forked branching usually with thick green stems (catus-like).
* Decurrent (deliquescent) tree forms have many dominant branches with a spreading crown form caused by lateral branches growing at similar rates as the main axis terminal (leader), or the terminal continues to die with lateral branches rebranching continuously (so no one central axis develops, but many spreading branches).
* Excurrent tree form has a single dominant axis (leader) and forms a conical shaped crown as the terminal elongates more annually than lateral branches (a distinct main axis and many short secondary branches.

<center>![Tree growth forms](./images/CrownArchitectures.png)</center>

Given these base growth forms, we can define a series of generalized crown shapes useful for developing tree models.

<center>![Tree crown shape names](./images/CrownShapes.png)</center>
<center>![Tree crown shapes](./images/CrownShapeImages.png)</center>

# References
Coder, Kim D. 2018. Tree anatomy: Defining trees & forms. Warnell School of Forestry & Natural Resources, University of Georgia, (Outreach Publication WSFNR-19-35)[https://bugwoodcloud.org/resource/files/15277.pdf]. Pp.20.
