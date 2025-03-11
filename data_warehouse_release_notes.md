# Data Warehouse Release Notes

## 3.1.0 - 03/31/2025

This release included
* Removing validation rules that have been discontinued by TEA
* Updating validation rules to reflect changes listed in the TEA changelog
* Optimizing validation rules efficiency by refactoring code with DRY principles and improving join performance.
* Adding updated validation promotion logic to 16 prioritized L3 Summer rules marked 3.1 in column J of [this](https://docs.google.com/spreadsheets/d/1IV29MxGqdzez80GLu2kxkhMJ-afsP7km0VdVgzeYKXQ/edit?gid=1290404059#gid=1290404059) spreadsheet.

## 2.2.0 - 10/15/2024

This release included
* additional validation rules implemented
* updates to existing validation rules for 2025
* addition of campus IDs to validation rules
* assessment automation and configuration updates
* pulling in updated DHC package
* upgrades to other under-the-hood packages

as well as additional updates to support Ed-Fi Data Standard v5.0 changes/additions via sub-packages `edu_edfi_source` and `edu_wh` such as
* change the source of `dim_parent` to `stg_ef3__contacts` and `fct_student_parent_association` to `stg_ef3__student_contact_associations` due to the rename from parent to contact in Ed-Fi data standard v5.0
* add `section_type` descriptor column to `dim_section`
* add `preferred_first_name`, `preferred_last_name`, and `gender_identity` columns to dim_staff
* add `preferred_first_name`, `preferred_last_name`, and `gender_identity` columns to dim_parent
* fix surrogate key creation for `stg_ef3__grading_periods` to properly hanlde lowering of alphanumeric column (`grading_period_name`) that is part of natural key

## 2.1.0 - 07/23/2024

This release included
* adding the TEA version of id_system
* replacing `courseIdentificationSystemDescriptor` values with their `shortDescription`
* configuring descriptors and extensions from `studentAcademicRecord.diplomas` and `courseTranscripts` for Region 10's CCMR app
* updating warehouse to latest version of edu_wh (0.3.3), which includes warehouse models for diplomas, graduation plan, and [more](https://github.com/edanalytics/edu_wh/blob/main/CHANGELOG.md#edu_wh-v033)

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
