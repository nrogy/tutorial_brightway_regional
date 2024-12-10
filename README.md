# Welcome

Welcome to this tutorial, which is a remake of the [tutorial](https://github.com/brightway-lca/from-the-ground-up/tree/main/regionalization/background-regionalization) built by Chris Mutel. The aim of this remake is to look in the hood of the package [bw2regional](https://github.com/brightway-lca/brightway2-regional) that allows performing regionalised Life Cycle Assessment (LCA), i.e. "including a detailed description of the location where an inventory dataset occurs" [(Mutel and Hellweg, 2023)](https://doi.org/10.31223/X5537N                ). 

# Goals of this tutorial

The goals of this tutorial are:
1. To be able to regionalise background and foreground Life Cycle Inventory (LCI) databases in brightway 2.5
2. To be able to look in the hood of the package bw2regional to check the results
3. To perform regionalised Life Cycle Assessment

These objectives will be achieved through the comparison between the impacts of driving a car for 1km with petrol and 1km with ethanol from sugarcane. The Life Cycle Impact Assessment (LCIA) method used is the LC-Impact method [(Verones et al., 2020)](https://doi.org/10.1111/jiec.13018                       ) implemented in brightway through the [bw2-lcimpact](https://github.com/cmutel/bw2-lcimpact) package.

In this tutorial, we will play with one approach for Regionalized LCA, i.e. Two Spatial Scales, Areal Allocation, and with Site-Generic LCA, as defined by [Mutel and Hellweg (2023)](https://doi.org/10.31223/X5537N                         ). 

# Contents of this tutorial

This tutorial consists in 5 notebooks excluding this one :
* 0 - Modification of the different packages
* 1 - Set up databases
* 2 - Set up regionalised data
* 3 - Under the hood of Regionalised LCA calculations
* 4 - Regionalised LCA calculations

The foreground database is available in the excel "ethanol-inventory.xlsx"

In the folder "Maps" I added some maps, also called geopackages in the tutorial, allowing the regionalisation of the LCI and of the LCIA. The maps are compatible with Ecoinvent 3.8. I modified the names of some features from the maps to be able to run the code. These modifications are explained in the notebook "2 - Set up regionalised data".

The virtual environment I used to run this tutorial is also available : ``brightway_regional_2.yml``.

# Versions of the main packages of the tutorial

The versions of some of the main packages are:
* brightway25 = 1.0.6
* bw2_lcimpact = 0.4.2
* bw2analyzer = 0.11.7
* bw2calc = 2.0.dev18
* bw2data = 4.0.dev46
* bw2io = 0.9.dev29
* bw2parameters = 1.1.0
* bw2regional = 0.7.dev2
* constructive_geometries = 0.8.2
* numpy = 1.26.4
* pandas = 2.0.3
* python = 3.10.14
* rower = 0.3

# Things to do before runing the tutorial

Before runing the tutorial:
1. Read this [paper](https://doi.org/10.31223/X5537N                )
2. Create the ``brightway_regional_2`` virtual environment.
3. Add the LCI maps in a folder of your computer
4. Replace the LCIA maps of the ``bw2_lcimpact`` package by the LCIA maps of this tutorial. The address is : ``C:\Users\``yourname``\AppData\Local\anaconda3\envs\brightway_regional_2\Lib\site-packages\bw2_lcimpact\data``
5. Modify the code of the packages according to the notebook <b> 0 - Modification of the different packages<b>. You will need the adress of the LCI maps that you registered on your computer.

# Some last words

If you need help for running this tutorial, don't hesitate to contact me on github or by email nicolas.rogy@ifpen.fr
I hope that you will enjoy it as much as I enjoyed building this remake.
