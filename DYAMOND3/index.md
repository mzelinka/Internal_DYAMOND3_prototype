---
layout: default
title: DYAMOND3 prototype Homepage
---

# DYAMOND3
# Cess-Potter Uniform +4K Experiments
<img src="images/AR_CA60_zoom2880x1440_starField3.png" alt="SCREAM_CA60_zoom">

## Synopsis:
<p>
Anthropogenic global warming is a pressing societal concern for which accurate predictions of future climate are needed. Unfortunately, climate model projections of the future vary widely owing to uncertainty in future anthropogenic radiative forcing and from uncertainty in equilibrium climate sensitivity (ECS)  –  the steady-state change in temperature in response to a sustained doubling of atmospheric carbon dioxide.  Reducing uncertainty in ECS is an abiding goal of climate science, as many aspects of the global climate response to warming are tied to the overall response of global temperature. The root cause of uncertainty in ECS is uncertainty in radiative feedbacks that modulate the ability of the Earth to shed heat to space as it warms. Cloud feedback is the dominant component of this uncertainty because of the significant leverage that clouds have on the Earth’s energy budget, the wide diversity of cloud types in the atmosphere, and the fact that their radiative properties are controlled by both macroscale and microscale processes, most of which are crudely represented in global models. Given the resultant disagreement among global climate models in cloud feedback and ECS (which has persisted for decades and has recently grown), recent efforts have instead attempted to constrain climate sensitivity through synthesizing other lines of evidence (i.e., historical record, paleoclimate evidence, and process-level studies), with promising results. Nevertheless, numerical simulations of present and future climate at the global scale remain a unique and essential tool for climate science, not only for exploring and improving our understanding of Earth’s climate in a physically consistent framework, but also for providing information on future climate at space and time scales that are relevant to a growing spectrum of societal needs.<br>

In this context, the latest generation of high resolution (<5k km horizontal grid spacing) global storm-resolving models (GSRMs) serves as a potential game changer. This is because they explicitly simulate more small-scale processes, thereby requiring fewer subgrid-scale parameterizations than their coarse-resolution counterparts, with the anticipation that this will allow them to simulate climate more reliably. Indeed, GSRMs have been shown to simulate cloud and precipitation characteristics with much greater fidelity than coarse resolution models (Caldwell et al 2021), and explicitly simulate impactful weather events like tropical cyclones and mesoscale convective systems that cannot be resolved by coarse resolution models (Judt et al 2021; Feng et al 2018). Despite these improvements, they still struggle with simulating clouds that are formed from sub-kilometer-scale motions or that depend sensitively on representation of cloud microphysics, which remain unresolved. The DYAMOND (DYnamics of the Atmospheric general circulation Modeled On Non-hydrostatic Domains) Project was established to facilitate intercomparison of GSRM representations of the atmospheric circulation at timescales of weeks to decades and to explore the ability of such models to better represent the atmospheric general circulation relative to traditional global climate models. The <a href="https://www.esiwace.eu/the-project/past-phases/dyamond-initiative/services-dyamond-summer">first</a> and <a href="https://www.esiwace.eu/the-project/past-phases/dyamond-initiative/services-dyamond-winter">second</a> phases of DYAMOND were successful in uniting and invigorating a growing community of global storm-resolving modelers to simulate and examine 40-day simulation campaigns in northern-hemisphere summer and winter seasons (respectively).<br>

The next logical step is to examine climate warming simulations with GSRMs. As part of this 3rd Phase of DYAMOND, a pair of year-long “AMIP-style” prescribed SST/SIC simulations will be conducted. The first is the control climate experiment already described in Takasuka et al (2024). The second is identical to this control experiment, except with sea surface temperatures uniformly increased by 4K everywhere. This pair of simulations will be used to explore the response of climate to warming and follow from Cess-Potter experiments that have routinely been conducted over the past several decades with coarse resolution models as an efficient way to diagnose key processes governing climate sensitivity without the need for long coupled model integrations. <a href="https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1002/2014GL060347">Ringer et al. (2014)</a> and <a href="https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021JD035460">Qin et al. (2022)</a> have demonstrated that such idealized simulations can effectively capture the key feedback mechanisms seen in fully coupled simulations, including cloud feedbacks at global and regional scales. Moreover, Qin et al (2022) find that atmosphere-only +4K experiments of short duration (e.g., only a single year) are sufficient for capturing this signal. This motivates the proposed experimental design described below.<br>
</p>

### The goals of these simulations are to:
<p><ol>
    <li>diagnose responses (including climate sensitivity, radiative feedbacks, responses of the hydrological cycle and general circulation of the atmosphere, etc.) to warming</li>
    <li>determine which climate responses are robust across GSRMs and which differ in important ways</li>
    <li>decompose and evaluate model agreement in individual climate responses</li>
    <li>compare and contrast the responses that emerge at storm resolving scales with those produced in traditional GCMs</li>
    <li>establish a baseline response to uniform warming that can be compared to subsequent experiments with non-uniform warming to explore questions related to pattern effects in high resolution models</li>
</ol></p>

## Protocol:
<p>
<ol>
    <li>+4K simulations should be identical to the control simulation (specified in Takasuka et al 2024) in all ways except SST should be uniformly increased by 4K everywhere.</li>
    <ol type="a">
    <li>If a modeling group performs the simulations for a different time period, it will still be accepted even though it may complicate comparison to other models.</li>
    <li>If a modeling group can only afford to run a subset of a year, it is recommended that they avoid solstice months, given that Qin et al (2022) found systematically less agreement between atmosphere-only feedbacks derived from solstice months and the “true” feedbacks diagnosed in coupled simulations.</li>
    <li>Use same land initial conditions as the control.</li>
    </ol>
    <li>Participating models must have grid spacing of 5 km or less. While it is preferred that models not incorporate a parameterized representation of atmospheric deep convection, such models will not be excluded. The vertical domain should extend to well above the troposphere (25 km or higher), and at least 75 vertical levels is desired. Models should be able to represent the actual atmospheric general circulation, which requires a full representation of fine-scale physical processes (microphysics, radiation, small-scale turbulence) as well as realistic lower boundary conditions like topography.</li>
    <li>Modeling centers are encouraged to implement the CFMIP Observation Simulator Package (COSP; <a href="https://journals.ametsoc.org/view/journals/bams/92/8/2011bams2856_1.xml">Bodas-Salcedo et al. (2011)</a>; <a href="https://gmd.copernicus.org/articles/11/77/2018/">Swales et al. (2018))</a>, which produces cloud fields that are more directly comparable to satellite observations and that can be used to detail cloud radiative feedbacks.</li>
    <ol type="a">
    <li>Highest priority output are cloud fraction histograms produced by the ISCCP simulator and cloud fraction profiles provided by the CALIPSO simulator</li>
    <li>Modeling centers may choose to write the output needed to run COSP offline if online implementation is not possible.</li>
    </ol>
</ol>
</p>

## Model output and data policy
<p>
Unlike the first two phases of DYAMOND, data archiving and access - including provision of and access to input data - will be provided through NERSC. Because these Cess-Potter simulations are an order of magnitude longer than previous DYAMOND runs, and both the control and +4K runs are needed to investigate temperature-mediated changes in fields, the set of requested data must be trimmed down. Novel approaches to reducing data volume (such as coarsening output or using data compression) are welcome so long as anyone analyzing the data would be able to use the provided data.
</p>
<p>
Groups should strive to conform to the specified output (in Tables 1-X). Additional output is welcome if it is needed to understand a given model and some requested output may not be well defined for some models. Participants should document the data they provide and any relevant details for understanding or using this data. In recognition of the challenges in writing output from such large simulations, conformance to the output requirements is left up to the individual groups’ best judgment.
</p>
<p>
To address several of the primary goals listed above does not generally require high temporal or spatial resolution model output. For example, diagnosing and decomposing radiative feedbacks can be done using offline monthly-resolved radiative kernels at low spatial resolution corresponding to traditional GCMs. Given this, and the desire to facilitate collection of a large collection of model data to be hosted at a central location, we have identified high priority fields that are written at relatively low spatial (0.25 degree) resolution, keeping data volumes relatively small. These data are requested at both monthly and 3-hourly resolution (Tables 1-2), the latter to facilitate examining temperature-mediated changes in cloud organization, submonthly precipitation, convection, synoptic systems, tropical cyclones, etc. Several select 2D fields useful for storm tracking are additionally requested at 1-hourly resolution (Table 2). Finally, for modeling groups that have the capability, outputs from satellite simulators and higher spatio-temporal frequency fields useful for investigating the behavior of clouds in key climate regimes are requested (Table 3).
</p>
<p>Below, we define standard pressure levels as the 37 pressure levels from ERA5 reanalysis: 1000, 975, 950, 925, 900, 875, 850, 825, 800, 775, 750, 700, 650, 600, 550,
334 500, 450, 400, 350, 300, 250, 225, 200, 175, 150, 125, 100, 70, 50, 30, 20, 10, 7, 5, 3, 2, and 1hPa.
</p><br>

### Tier 1. High priority
<p>Table 1. 3D Output on standard pressure levels and 0.25˚ horizontal resolution.
<style>
table {
  font-family: arial, sans-serif;
  border-collapse: collapse;
  width: 100%;
}

td, th {
  border: 1px solid #dddddd;
  text-align: left;
  padding: 8px;
}

tr:nth-child(even) {
  background-color: #dddddd;
}
</style>
<table>
    <tr>
        <th>   </th>
        <th>Variable Long Name</th>
        <th>Units</th>
        <th>Temporal Resolution</th>
    </tr>
    <tr>
        <td>1</td>
        <td>Cloud fraction</td>
        <td>fraction</td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>2</td>
        <td>Mass fraction of cloud water</td>
        <td>g kg<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>3</td>
        <td>Mass fraction of rain water</td>
        <td>g kg<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>4</td>
        <td>Mass fraction of graupel water</td>
        <td>g kg<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>5</td>
        <td>Mass fraction of snow water</td>
        <td>g kg<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>6</td>
        <td>Mass fraction of cloud ice</td>
        <td>g kg<sup>−1</sup></td>
        <td>mon |  3hr</td>
    <tr>
        <td>7</td>
        <td>Relative humidity</td>
        <td>%</td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>8</td>
        <td>Specific humidity</td>
        <td>g kg<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>9</td>
        <td>Temperature</td>
        <td>K</td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>10</td>
        <td>Zonal wind velocity</td>
        <td>m s<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>11</td>
        <td>Meridional wind velocity</td>
        <td>m s<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>12</td>
        <td>Vertical velocity</td>
        <td>Pa s<sup>−1</sup></td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td>13</td>
        <td>Geopotential height</td>
        <td>m</td>
        <td>mon |  3hr</td>
    </tr>
</table>
</p><br>

<p>Table 2. 2D output at 0.25˚ horizontal resolution.
<table>
<tbody>
    <tr>
        <td> 1</td>
        <td>Vertically integrated cloud ice,</td>
        <td>kg m-2</td>
        <td>mon |  3hr</td>
    </tr>
    <tr>
        <td> 2</td>
        <td>Total cloud cover</td>
        <td>%         </td>
        <td>mon |  3hr        </td>
    </tr>
    <tr>
        <td> 3</td>
        <td>Vertically integrated cloud water (liquid + ice)   </td>
        <td>kg m-2    </td>
        <td>mon |  3hr        </td>
    </tr>
    <tr>
        <td> 4</td>
        <td>Surface upward latent heat flux </td>
        <td>W m-2     </td>
        <td>mon |  3hr        </td>
    </tr>
    <tr><td> 5</td><td>Surface upward sensible heat flux   </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td> 6</td><td>Surface (2 m) relative humidity </td><td>%         </td><td>mon |  3hr        </td></tr>
<tr><td> 7</td><td>Surface (2 m) specific humidity </td><td>g kg-1    </td><td>mon |  3hr        </td></tr>
<tr><td> 8</td><td>Precipitation    </td><td>kg m-2 s-1</td><td>mon |  3hr |  1 hr</td></tr>
<tr><td> 9</td><td>Column water vapor              </td><td>kg m-2    </td><td>mon |  3hr        </td></tr>
<tr><td>10</td><td>Surface air pressure            </td><td>Pa        </td><td>mon |  3hr        </td></tr>
<tr><td>11</td><td>Sea level pressure              </td><td>Pa        </td><td>mon |  3hr        </td></tr>
<tr><td>12</td><td>Surface downwelling longwave radiation             </td><td>W m-2     </td><td>mon | 3hr         </td></tr>
<tr><td>13</td><td>Surface downwelling longwave radiation under clear-sky conditions </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>14</td><td>Surface upwelling longwave radiation</td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>15</td><td>TOA upwelling longwave radiation</td><td>W m-2     </td><td>mon |  3hr |  1 hr</td></tr>
<tr><td>16</td><td>TOA upwelling longwave radiation under clear-sky conditions       </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>17</td><td>Surface downwelling shortwave radiation            </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>18</td><td>Surface downwelling shortwave radiation under clear-sky conditions</td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>19</td><td>TOA downwelling shortwave radiation </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>20</td><td>Surface upwelling shortwave radiation              </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td >21</td><td>Surface upwelling shortwave radiation under clear-sky conditions  </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td >22</td><td>TOA upwelling shortwave radiation   </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td >23</td><td>TOA upwelling shortwave radiation under clear-sky conditions      </td><td>W m-2     </td><td>mon |  3hr        </td></tr>
<tr><td >24</td><td>Surface (10 m) wind velocity    </td><td>m s-1     </td><td>mon |  3hr |  1 hr</td></tr>
<tr><td >25</td><td>Surface (2 m) air temperature   </td><td>K         </td><td>mon |  3hr        </td></tr>
<tr><td >26</td><td>Surface skin temperature        </td><td>K         </td><td>mon |  3hr        </td></tr>
<tr><td >27</td><td>Surface (10 m) zonal wind velocity  </td><td>m s-1     </td><td>mon |  3hr        </td></tr>
<tr><td>28</td><td>Surface (10 m) meridional wind velocity            </td><td>m s-1     </td><td>mon |  3hr        </td></tr>
<tr><td>29</td><td>Integrated vapor transport (zonal)  </td><td>kg m-1 s-1</td><td>mon |  3hr |  1 hr</td></tr>
<tr><td>30</td><td>Integrated vapor transport (meridional)            </td><td>kg m-1 s-1</td><td>mon |  3hr |  1 hr</td></tr>
<tr><td>31</td><td>300 hPa geopotential height     </td><td>m         </td><td>mon |  3hr |  1 hr</td></tr>
<tr><td>32</td><td>500 hPa geopotential height     </td><td>m         </td><td>mon |  3hr |  1 hr</td></tr>
<tr><td>33</td><td>Zonal momentum flux at the surface  </td><td>N m-2     </td><td>mon |  3hr        </td></tr>
<tr><td>34</td><td>Meridional momentum flux at the surface            </td><td>N m-2     </td><td>mon |  3hr        </td></tr>
</tbody>
</table>
</p>
<p>Table 3. Output (15 min interval) on select pressure levels (200, 500, 700, and 850 hPa).
<table>
    <tr>
        <th>Atmosphere</th>
        <th>Variable Long Name</th>
        <th>Units</th>
    </tr>
    <tr>
        <td>u</td>
        <td>Zonal wind on model level</td>
        <td>m s−1</td>
    </tr>
</table>
</p>

## Timeline & Next Steps
<p>
The project timeline is given in Table 6, this includes a couple of action items that need to take place before the simulations can be started. One is the exact specification of the output data (especially ocean), the other is the provision of the initial data. It is expected that all information and data is available by the 1st of March 2020.
</p>
<p>Table 6. Project winter DYAMOND atmosphere only and coupled atmosphere-ocean timeline.
<table>
    <tr>
        <th>Date</th>
        <th>Action to be completed</th>
    </tr>
    <tr>
        <td>15.07.2019 </td>
        <td>Initial protocol to be circulated</td>
    </tr>
</table>
</p>

## Perspective
Project DYAMOND is working toward an intercomparison of global storm O(3 km) resolving model representations of the atmospheric circulation on the decadal time scale. It will explore the ability of such models to better represent the atmospheric general circulation, and its sensitivity to surface temperature, as compared to traditional approaches, which use a statistical representation using statistical representations of major modes of convective heat transport. One pressing question is whether changes in clouds, precipitation and cloud controlling factors is similar to what has been gleaned from cruder (traditional) models of the atmospheric circulation. The coupled simulations specifically target the atmosphere-ocean interactions on the meso-scale and the impact on the general circulation, when convection and ocean eddies are resolved.

## Open Questions
<p><ol>
    <li>Requests about COSP-type output?</li>
    <li>Question2</li>
</ol></p>

#### Acknowledgements
[E3SM](https://e3sm.org/)
[SCREAM](link)
[NERSC](https://www.nersc.gov/)
[LLNL](https://www.llnl.gov/)
[PCMDI](https://pcmdi.llnl.gov/index.html)
[DOE (RGMA, EESM)](link)

###### Document version: 21 November 2023
[termsOfUse]: TermsOfUse/