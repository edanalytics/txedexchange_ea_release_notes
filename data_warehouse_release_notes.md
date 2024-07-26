# Data Warehouse Release Notes

## 2.1.0 - 07/23/2024

This release included
* adding the TEA version of id_system
* replacing `courseIdentificationSystemDescriptor` values with their `shortDescription`
* configuring descriptors and extensions from `studentAcademicRecord.diplomas` and `courseTranscripts` for Region 10's CCMR app
* updating warehouse to latest version of edu_wh (0.3.3), which includes warehouse models for diplomas, graduation plan, and [more](https://educationanalytics.monday.com/boards/3556827529/pulses/3611787577)

## 2.0.0 - 06/11/2024

This release included
* code to configure and load more assessment data:
  * DIBELS
  * iReady
  * CLI TX-KEA
  * improvements to automated extracts of files from sharefile
* updating warehouse to latest version of edx_portal_dw_data_health_check
* updating warehouse to latest version of edu_wh
* updating warehouse to latest version of edu_ext_podium (new models to support new/updated Leadership Analytics dashboards)
* new data validations developed by Crocus, reviewed by EA
* code to expand models for several extensions, particulary in student academic record domain
