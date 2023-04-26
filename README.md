# TFLtargets

## Project concept.   

[![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)

Factories for generating TFLs using {targets} and a titlefootnote file.  

The goal of this package is to generate `tar_target()` shells (i.e., `tarchetypes`) that can assist in the reproducible generation of TFLs. Here we are focused on the generation of the outputs themselves, and not any of the modeling steps that comes before. 

Traditionally, programmers would use a titlefootnote file to organize this work. We will also use the titlefootnote file as the backbone of generating targets.  

- [ ] Read in and validate titlefootnote files. 
  - [ ] Titlefootnote S3 object with validation. 
    - [ ] The validation function should be customizable in the future. 
- [ ] Similar to other packages such as `stantargets`, write [target factories](https://wlandau.github.io/targetopia/contributing.html) to generate TFLs. These factories should allow users to specify three components: input data, output generation function, and saving directories. These target factories can also be specified by section (i.e., efficacy data, secondary outcomes).   
- [ ] A `tarchetype` function to pack these outputs into RTF files.  

## Additional considerations. 

Some additional considerations include:  
1. The package [rtables](https://insightsengineering.github.io/rtables/main/) allows users to generate a table "shell" that can be piped to a data set. Using this and/or `gt`/`gt_summary` can simplify the process.  


