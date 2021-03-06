# Carbonic anhydrase II : caboxybenzenesulfonamide (CAII:CBS)

This script produces the input file for measuring the binding affinity of CBS to CAII

## Reference

* Sarah E. Boyce, Joel Tellinghuisen, and John D. Chodera.
  Avoiding accuracy-limiting pitfalls in the study of protein-ligand interactions with isothermal titration calorimetry.
  http://dx.doi.org/10.1101/023796

## Deck configuration

For the `caii` experiment:
* `Water` (`Trough 100ml`) - ddH2O
* `Buffer` (`Trough 100ml`) - CAII dialysate
* `SourcePlate` (`5x3 Vial Holder`) - well A1 holds CBS solution
* `ProteinSourcePlate` (`ITC Plate`) - well A1 holds CAII solution
* `DestinationPlate` (`ITC Plate`) - empty ITC 96-well deepwell plate

## Manifest

* `bCAII.py` - bovine CAII:CBS experiment
* `hCAII.py` - human CAII:CBS experiment
* `bCAII-SIM.py` - bovine CAII:CBS experiment with standard and SIM titrations

* `*-LiHa.gwl` - a Tecan EVO LiHa worklist to pipette buffer and protein
* `*-aLiHa.gwl` - a Tecan EVO aLiHa worklist to pipette ligand
* `*.xlsx` - a spreadsheet for the PEAQ that defines the cell and syringe sources for each titration series
* `*.csv` - translation of XLSX

## Experimental

* `experiment-caii-and-phipa-pilot.py` - pilot experiment for combined CAII and PHIPA experiments
