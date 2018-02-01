***********************
High Level Project Plan
***********************

Phase 1: Induction Phase
************************

Development of PSC and PMC
^^^^^^^^^^^^^^^^^^^^^^^^^^
A Project Steering Committee (PSC), comprised of at least one senior-level member from each partner organization and chaired by the Under Secretary of the Ministry of Forests and Soil Conservation will be meet bi-annually, proving guidance to the project. Other USAID programs (PAANI, Hariyo Ban, SERVIR) will be invited to observe these meetings and seek ways to integrate JaibikMap to leverage USAID funding. The Project Management Committee (PMC) of at least one member from each partner organization will meet monthly, oversee day-to-day project operations, and regularly report as per USAID guidelines. A Project Implementation Unit will be coordinated by IUCN PI, with one specialists guiding Junior Researchers. A National Data Review and Assessment/Inception Workshop will be organized. During this phase the PMC’s will draft a work plan (giving output deadlines), followed by formal MOUs.

Phase 2: Data acquisition, analysis and mapping
***********************************************

The details regarding data elements can be viewed at :doc:`/data_elements` page.

Mammalian species data
^^^^^^^^^^^^^^^^^^^^^^
Compiled data will include data on mammal species description, occurrences, distribution, status, habitat requirements and main threats. Institutional members  will be solicited to submit existing and emerging occurrence data after receiving information sheets on mammal species. As all 208 mammalian species were included in the IUCN national-level “2011 Mammal Red-List Species Assessment”, raw data housed at the Department of National Parks and Wildlife Conservation (DNPWC) will be translated into the GIS platform. All gaps in mammalian data will be identified and will become a priority for DNPWC.

Land use/ Habitat Data
^^^^^^^^^^^^^^^^^^^^^^
Compiled data will include current land use (e.g. forest, plains, wetlands, agricultural land, major settlements and roads). This information will be formally requested by DNPWC from a variety of Government of Nepal (GoN) Departments (e.g. Department of Forests, Department of Forest Research and Survey, Department of Statistics). The most complete national land cover database of Nepal prepared using public domain Landsat TM data of 2010 and replicable methodology will be accessed and incorporated from the USAID-funded SERVIR Himalaya project, along with the project’s maps for Protected Areas and Population Density.

Meteorological Data
^^^^^^^^^^^^^^^^^^^
Gathered from the Department of Hydrology and Meteorology (DHM) from the 282 meteorological stations established in Nepal, historical (from the past 70 years) and contemporary meteorological data will be purchased, compiled, cleaned and translated into the JaibikMap system. This data will also feed into the climate change modelling described below.

Phase 3: Analysis through modelling
***********************************

National-level Forest Climate Change Modelling Methodology
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
    1. Holdridge (1967) Life Zone (HLZ) Analysis provides a basis for defining local ecosystems in a globally comparable framework, building a useful. Using climate data gathered from DHM (precipitation, temperature, evapotranspiration), analysis will be conducted on the basis of existing and projected climate conditions using different climate change models (CCCM and DGF3) (Jha, 2006) in order to determine likely changes in vegetation patterns due to shifting “life zones”.
    
    2. Normalized Difference Vegetation Index (NDVI) is a simple graphical indicator that can be used to analyse remote sensing measurement to assess whether targeted satellite imagery of Nepal contains live green vegetation or not. Mainali et al (2015) have observed that both precipitation and temperature affect NDVI values in specific conservation areas of Nepal. NDVI data from 2000-2010 will be collected using multi- temporal Terra MODIS Vegetation Indices Product (MOD13Q1) and digitally encoded in GIS along with meteorological data gathered from DHM for the past 70 years.

Species distribution modelling for mechanistic
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The species distribution modelling will focus on key mammal species which are most vulnerable to habitat loss due to climate change as well as endemic plant species previously studied by Co-PI Dr. Jha. Working on each species individually, the climate (HLZ) and multi-temporal remote-sensing (NDVI) will be used to create a mechanistic habitat assessment model which incorporates climatic features and biotic features to evaluate the impacts of climate change on the species spatial distribution.

Phase 4: Model verification and validation
******************************************

    1. To verify the validity of the National Level Forest Change Analysis, three forest types that have narrow range distributions (TISC 2002) in Eastern, Central, and Western Nepal, the combined HLZ and NDVI model will be cast with predictions of the impacts of forest change on forest cover. Field assessments will be conducted, during which time the three studied narrow-range forest types will be visited and analysed based on the field reality and tree ring analysis in order to reconcile accuracy of climate change information and verify the model’s accuracy.
    2. In these forest-field sites, citizen scientists’ observations will be consulted to gather accounts of shifts in occurrence of key endemic species as well as mammalian species observed over the past 10 years. The study population will be community forest user groups’ (CFUG) members. CFUGs in Nepal are required to have equal representation of women, and representation of dalit or other marginalized groups.
    3. To better understand data-deficient phenological trends, a secondary field analysis will be conducted in the Himalayan region which can be compared with past records.
    4. Reconciling all gathered information, the models will be finalized and information will be translated into GIS and other forms required for the map system.

Co-PI Dr. PK Jha will compare his current USAID-funded research on the impacts of climate change on vegetation patterns in the Chitwan Annapurna Landscape with the National Level Forest Change Analysis. As little is currently known about the impacts of climate change on biodiversity in this area (which is covered by the USAID-funded Hariyo-ban project), insights may be gained through this comparison.

Phase 5: Tool (JaibikMap) development
*************************************

Requirement analysis and system architecture
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The details regarding system architecture and technology pipeline can be viewed at :doc:`/tech_stack` page.

Prior to data importation, a systematic review will be held by KLL to analyse what has been collected in order to identify required system and website components. Next, web programmers will develop the system architecture, including the system blueprint. The overall Open-street map base layer will be designed and amended as necessary, including all land-use and forest data overlays. The map design will then be reviewed by the PMC and amended as needed. Finally, the system administration will be developed, including data storage and integration of a mechanism for updating, system control, and backup.

System Construction
^^^^^^^^^^^^^^^^^^^

The details regarding visual elements of the tool can be viewed at :doc:`/visual_elements` page.

Finally, the web-based JaibikMap will be coded, including key interactive interface elements, such as 

            - Searchable species habitat/range
            - Slippy/zooming
            - Links with relevant materials from other online sources
            - Several layers (forest cover, land use, mammal range, etc.)
            - Downloadable data
            - Display of mammalian pictures taken by citizen scientists
            
Next, the Android Phone App will be developed, through which citizen scientists can upload pictures taken during opportunistic sightings of mammalian species. This information will feed back to a database which can be accessed by specific users (as to avoid the danger of informing poachers of mammal occurrence). Pictures can be viewed on the web-based platform linked with general information about the mammals.

Incorporation of MOL features
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The National Science Foundation-supported Map of life (MOL) team (PIs Jetz, Yale University; Guralnik, University of Florida) will assist with the integration, use and applications of key MOL features to be included in the JaibikMap. Some such features developed by MOL to be leveraged will include:

            - Regionalized web-application: allows Nepal-focal selection of species for assessment of regional data availability, consensus distribution mapping, and detailed distribution assessment. Biodiversity information (species distribution, lists, etc.) and reporting tools will allow for visualization, analysis and download.
            - Mapping species richness and endemism patterns: regionalized for Nepal, species richness, inventory completeness, and endemism can be visualized. This is especially useful for targeting survey efforts in data deficient areas as well as for identifying biodiversity hotspots for focusing conservation efforts.
            - Refinement of interactive range map (overlaid with reserves): revealing the “best possible” species’ range, helping conservationists determine how well protected a species is based on Nepal’s reserve system.
            - Species-environment overlay tools for map layers: for comparison of current and future scenarios and remote sensing data
            - Species occurrence data upload tool: standardized uploading from multiple data contributors for streamlined ingest from previously disparate groups
            - Prototype of a mobile application for Nepal biodiversity discovery and citizen science data recording that can work away from the cell network (offline)

These features jumpstart the project and allow the timeline/budget to be feasible. The sharing of technical expertise and developed products will occur through Skype meetings and direct/ongoing communication with the Kathmandu-based developers. Training will be provided by the MOL team on the use of the aforementioned tools, as well as during the modelling design and analysis. Capacity development will occur over the span of the project with all related CO-PIs focusing on data mobilization, analysis, and technology development.

In turn, the MOL project will be able to test the scalability of its platform and facilitate critical biodiversity conservation in a region vulnerable to the impacts of climate change – a new step for the global project. By addressing the specific demands of regions such as Nepal, MOL will increase understanding of how to build capacity in data-deficient regions.

Dissemination and Capacity Development
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Specialized training on scientific methods
------------------------------------------

In order to develop the capacity of a variety of stakeholders to continue to use the JaibikMap for both inductive and deductively modeled predictions, a series of trainings will be led by the CO-PI Dr. PK Jah (in coordination with the Map of Life team), for 30-50 stakeholders, including: researchers and policymakers from the GoN’s Department of Hydrology and Meteorology and Department of National Parks and Wildlife, academics and graduate/post-graduate students from Tribhuvan University, IUCN Nepal and Kathmandu Living Lab staff, and IUCN members from other conservation organizations. Trainings will include sessions on

    - Holdridge Life Zone analysis: Parameterize climate data, link DHM and DNPWC
    - NDVI and remote sensing: applications for SDM and climate change
    - Engagement of Citizen Scientists: how-to for researchers and practitioners in facilitating local level engagement; potential pathways for this paradigm shift.
    - Species Distribution Model (SDM) building: overview of SDMs (regression, Ecological Niche Factor Analysis, ensemble forecasting, etc.)
    - Climate Change Modelling and present-future planning strategies: developing inductive and deductive hypotheses

Data capacity and technological development
-------------------------------------------

At the inception phase of the project, a National Data Review and Assessment workshop will be held, during which time the PMC will prepare formal presentations reporting their current repositories of relevant data to present to 30-50 key stakeholders from diverse nature conservation organizations. The event will be held in Kathmandu, during which time the representatives in attendance will be solicited for further cooperation data sharing. Women’s, minority, ethnic and disability organizations (among others) will be targeted to receive otherwise missing data inputs. This workshop will yield a report assessing current limitations in data retrieval in Nepal with guidelines for stakeholders (particularly the Government of Nepal) for filling existing research gaps, later addressed through the project. Knowledge gained will inform KLL and MOL team of how the JaibikMap can develop, guiding the end product design of the JaibikMap. Tentative features will be communicated to everyone in attendance.

A JaibikMap Training Workshop, held in Kathmandu, will be conducted at the culmination of the project period. This workshop will target 100-150 external stakeholders, including policymakers, academics, researchers, species conservation and development planning implementers and students, with an emphasis on recruiting women from each target group. Local media will also be invited. The workshop, which will include our USG-supported partners either in person (pending outside funding) or via Skype, will elucidate how the JaibikMap was developed (including review of data layers and forest/species climate change modeling), how to best use the JaibikMap interface and its myriad applications.

Junior researcher development: GIS and data analysis
----------------------------------------------------

The management structure of the project is designed in such a way that junior researchers, particularly those with GIS and remote sensing backgrounds, will be employed. Working directly with CO-PIs, these specialists, while having 1-2 years of relevant experience, will be given direct feedback and mentorship throughout the project within the Project Implementing Unit, culminating in both informal (on-going meetings, etc.) and formal (directed trainings in the aforementioned series) training. A mid-level GIS/Remote Sensing expert will work with Dr. Menaka Panta and the MOL team to integrate and back-stop/quality check all products (data layers, maps, etc.) for the hand-over to KLL for it’s integration into the web-based platform.

Developing citizen science through community engagement
-------------------------------------------------------

During the validation phase of the forest change and species distribution modelling, workshops will be held with Community Forests User Groups to cover several topics and develop these groups’ capacities as citizen scientists. Specifically, sessions will be held with 30-50 individuals with 3 CFUGs at the three field sites areas during which time the following themes will be covered:

    - Species conservation: theory and practice as to why it is important for the health of forests and habitats
    - Climate change adaptation: what can be expected and how it impacts communities, including adaptation strategies based on IUCN’s Ecosystem-based Adaptation’s Framework which has been honed over the life of a 5 year global project (focused in Nepal in the Panchase area) in collaboration with UNDP, UNEP, and GoN
    - Wildlife monitoring and reporting

Further, KLL will continue to organize free, weekly “OpenStreetMap Clinic” to share and exchange knowledge of open data mapping with the public and actively works to engage Nepalese youth in open data mapping projects through programmes with public schools.
