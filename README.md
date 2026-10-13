# AEV-V2G-Grid-Resilience

## Overview

This repository provides the input datasets used in the study entitled:

**Operator-Oriented Co-optimization of Autonomous Electric Vehicle Fleet Operation and Grid Loss-of-Load Mitigation in Coupled Transportation–Distribution Networks**

The study investigates the coordinated operation of autonomous electric vehicle (AEV) fleets and vehicle-to-grid (V2G) services for passenger transportation and distribution-network loss-of-load mitigation under extreme weather disturbances.

The case study considers a coupled system comprising a 24-node transportation network and a 14-bus distribution network in New York City.

## Datasets

All datasets are provided in MATLAB `.mat` format.

| File | Description |
|---|---|
| `01_Passenger_OD_Demand.mat` | Passenger origin–destination (OD) travel demand across 24 transportation nodes and 48 half-hour intervals. |
| `02_Road_Network_Distances.mat` | Road-network topology and distances between transportation nodes. |
| `03_Original_Arc_Speeds.mat` | Original time-varying road-segment speeds, including harmonic mean, P15, and P85 speeds. |
| `04_Day_Ahead_Electricity_Prices.mat` | Day-ahead electricity prices over 48 half-hour intervals. |
| `05_Normalized_Native_Load_Profile.mat` | Normalized native electricity-load profile over 48 half-hour intervals. |
| `06_Native_Load_Bus_Base_Values.mat` | Base active and reactive power demands for the 14-bus distribution network. |
| `07_Charging_Station_Deployment.mat` | Charging-pile allocation and rated charging power across the 24 transportation nodes. |

## Data Specifications

- **Transportation network:** 24 nodes and 94 directed road links.
- **Distribution network:** 14 buses.
- **Time resolution:** 30 minutes for transportation and electricity-price inputs.
- **Passenger demand:** 89,961 travel requests across 48 intervals.
- **Charging infrastructure:** 450 charging piles rated at 40 kW each.
- **Traffic speed:** km/h.
- **Road distance:** km.
- **Electricity price:** USD/kWh.
- **Active and reactive power:** MW and MVAr.

## Data Usage

The datasets can be loaded directly in MATLAB. For example:

```matlab
load('01_Passenger_OD_Demand.mat');
load('02_Road_Network_Distances.mat');
load('03_Original_Arc_Speeds.mat');
load('04_Day_Ahead_Electricity_Prices.mat');
load('05_Normalized_Native_Load_Profile.mat');
load('06_Native_Load_Bus_Base_Values.mat');
load('07_Charging_Station_Deployment.mat');
```

The datasets support research on transportation–power network coordination, electric vehicle fleet optimization, V2G operation, and distribution-network resilience.

## Citation

If you use these datasets in your research, please cite the associated manuscript:

*Operator-Oriented Co-optimization of Autonomous Electric Vehicle Fleet Operation and Grid Loss-of-Load Mitigation in Coupled Transportation–Distribution Networks.*

## Contact

For questions regarding the datasets, please open an issue in this repository.
