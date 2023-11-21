---
layout: default
title: DYAMOND3 prototype Homepage
---

# DYAMOND3 - Cess-Potter Uniform +4K Experiments
<img src="images/AR_CA60_zoom2880x1440_starField.png" alt="SCREAM_CA60_zoom">

## Synopsis:
<p>
Project DYAMOND (DYnamics of the Atmospheric general circulation Modeled On Non-hydrostatic Domains) describes a framework for the intercomparison of an emerging class of atmospheric circulation models that, through their resolution of the major modes of atmospheric heat transport, endeavor to represent the most important scales of the full three-dimensional fluid dynamics of the atmospheric circulation. The <a href="https://www.esiwace.eu/the-project/past-phases/dyamond-initiative/services-dyamond-summer">first</a> and <a href="https://www.esiwace.eu/the-project/past-phases/dyamond-initiative/services-dyamond-winter">second</a> phases of DYAMOND were successful in establishing X,Y,Z. 
</p>
<p>
As part of this 3rd Phase of DYAMOND, year-long simulations will be conducted with sea surface temperatures uniformly increased by 4K. These simulations will be compared with year-long control simulations covering the same time period to explore the response of climate to warming, including climate sensitivity, radiative feedbacks, and hydrological cycle responses. These follow from Cess-Potter experiments that have routinely been conducted over the past several decades with coarse resolution models as an efficient way to diagnose key processes governing climate sensitivity without the need for long coupled model integrations. <a href="https://agupubs.onlinelibrary.wiley.com/doi/abs/10.1002/2014GL060347">Ringer et al. (2014)</a> and <a href="https://agupubs.onlinelibrary.wiley.com/doi/10.1029/2021JD035460">Qin et al. (2022)</a> have demonstrated that such idealized simulations can effectively capture the key feedback mechanisms seen in fully coupled simulations, including cloud feedbacks at global and regional scales. Moreover, Qin et al (2022) find that atmosphere-only +4K experiments of short duration (e.g., only a single year) are sufficient for capturing this signal. This motivates the proposed experimental design described below.
</p>

### The goals of these simulations are to:
<p><ol>
    <li>goal1</li>
    <li>goal2</li>
    <li>goal3</li>
    <li>goal4</li>
</ol></p>

## Protocol:
<p>
<ol>
    <li>Simulations will be initialized on 20 January 2020 (or slightly before) so as to encompass the EUREC4A tropical field study (as well as parts of the MOSAiC arctic expedition) which will start on the 20 January 2020 and will last until 1st March 2020. The initialization will be from a common (ECMWF) analysis, and run for forty days and forty nights with specified sea-surface temperatures (7 day running mean) for the atmosphere only experiments. Groups are left free to initialize soil moisture according to their sense of best practice.</li>
    <li>The same period will be simulated by coupled atmosphere-ocean models by groups capable of running coupled systems at storm resolving scales. Groups are free on how to initialize the ocean (nudged run-up to the initial date, or ocean analysis at initial date).</li>
    <li>To participate the host model must be run at a grid spacing of 5 km or less for the atmosphere and a comparable resolution for the model ocean (if possible) and not incorporate a parameterized representation of atmospheric deep convection. The vertical domain should extend to well above the troposphere (25 km or higher), and the convening participants are targeting model versions with about 75 levels or more for the atmosphere and a sufficient number of levels for the ocean to approximate observed SSTs and that allows to study atmosphere-ocean coupling on the meso-scale.</li>
    <li>Models are expected to be of a form capable of representing the actual atmospheric general circulation, and thereby incorporate a full representation of finescale physical processes (microphysics, radiation, small-scale turbulence) as well as a realistic lower boundary conditions like topography.</li>
    <li>Analysis will be split into a ten day spin-up period and a thirty day analysis period, with two and three dimensional output as discussed below (see also Tables 1,2,3 and Tables 4,5 for the ocean models).</li>
</ol>
</p>

## Model output and data policy
<p>
Unlike the first two phases of DYAMOND, data archiving and access, including provision of and access to input data, will be provided through NERSC. All simulation output will be made publicly available as quickly as is technically possible. 
</p>
<p>
Based on the first DYAMOND simulations, the total output per model varied between 21 TB (UM) and 147 TB (GEOS), depending on horizontal and vertical resolution, output frequency, number of variables and compression. The total data amount, including sensitivity experiments and experiments at coarser resolutions amounted to about 1 PB. Resources have been applied for within the framework of the ESiWACE project, the project will also set up a coordination page to share this protocol and establish points of contact. Variable lists will be slightly adjusted, based on experience from the initial phase of DYAMOND and complemented through an output variable list for the ocean models.
</p>
<p>
Groups may have additional output that they may wish to provide, and depending on their microphysical representation different variables may be appropriate, or certain integral quantities may not be well defined (i.e., CAPE or CIN). A output list is specified for the atmosphere models in the Tables 1-3 for guidance. Groups should try to conform to the specified output, and document what and how they provide output, but in recognition of the challenges in writing output from such large simulations conformance to the output requirements is left up to the individual groups best judgement, which worked well in the first DYAMOND experiment.
</p>
<p style="color:Red;"><i>
The following tables are placeholders for us to populate. I think we were planning to have certain fields be output at high temporal resolution while others would be less frequent, so as to not be archiving hundreds of TBs:
</i></p>
<p>Table 1. 3D Output(3 h interval). On model levels below 20km.
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
        <th>Atmosphere</th>
        <th>Variable Long Name</th>
        <th>Units</th>
    </tr>
    <tr>
        <td>u</td>
        <td>Zonal wind on model level</td>
        <td>m s−1</td>
    </tr>
    <tr>
        <td>v</td>
        <td>Meridional wind on model level</td>
        <td>m s−1</td>
    </tr>
    <tr>
        <td>w</td>
        <td>Vertical wind on model level</td>
        <td>m s−1</td>
    </tr>
    <tr>
        <td>T</td>
        <td>Temperature on model level</td>
        <td>K</td>
    </tr>
    <tr>
        <td>P</td>
        <td>Pressure on model level</td>
        <td>Pa</td>
    </tr>
    <tr>
        <td>q<sub>v</sub></td>
        <td>specific humidity on model level</td>
        <td>g kg−1</td>
    </tr>
    <tr>
        <td>q<sub>c</sub></td>
        <td>specific cloud water on model level</td>
        <td>g kg−1</td>
    </tr>
    <tr>
        <td>q<sub>i</sub></td>
        <td>specific cloud ice on model level</td>
        <td>g kg−1</td>
    </tr>
</table>
</p>
<p>Table 2. 2D Output (15 min interval).
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
</p>

#### Acknowledgements
[E3SM]()
[SCREAM]()
[NERSC]()
[LLNL]()
[PCMDI]()
[DOE (RGMA, EESM)]()

###### Document version: 21 November 2023
[termsOfUse]: TermsOfUse/