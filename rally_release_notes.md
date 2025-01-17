# Rally Release Notes

## 3.0.0 - 01/28/2025

This release focused on the expansion of supported assessments:
- Added i-Ready metadata to allow those assessments to persist to Rally's FE
- Added ACT to Stadium (also represented in the data warehouse workstream)

## 2.0.0 - 06/11/2024

This release focused on the expansion of supported assessments, plus a minor UI update:
- Added CLI CIRCLE and TX-KEA metadata to allow those assessments to persist to Rally's FE
- Updated the Classroom page ring charts and assessment charts to only use permitted aria-labels

## 1.2.0 - 04/07/2024

This release focused on some minor design enhancements that did not make it into v1.0.
- Added a performance level backgrounds toggle to the performance over time chart
- Enhanced the student page to make navigating back to the classroom page more clear
- Updated the loading text for the student attendance page
- Improved the student navigation panel for consistency, and to include school name(s)
- Improved the classroom navigation panel to include teacher name(s)
- Updated the "no data" message on the student performance over time chart
- Made student names clickable in grade/classroom assessment table view, as well as in the grade/classroom well-being table so users can drill down to view a student
- Made student names clickable in the grade/classroom chronic absenteeism and passing percentage charts so users can drill down to view a student
- Improved the landing page by adding a school filter to make navigation easier for district admins with many schools
- Improved closing tool tips for the chronic absenteeism and passing percentage charts
- Re-styled the FAQ page

## 1.0.0 - 01/31/2024

This release represented a substantial redesign of Rally with updated navigation, and the addition of new data.
- Navigation - updated for ease of use and future flexibility, informed by user research
- Classroom page
  - Added student course and grade data
  - Added student discipline and behavior data
  - Added program data
  - Updated assessment charts and table views
- Student page
  - Added student course and grade data
  - Added student discipline and behavior data
  - Added program data
  - Updated assessment charts, table views and performance over time chart
  - Added student attendance data
- Consolidated and simplified admin features
- Expansion of accepted assessments - CLI early childhood screeners (CIRCLE, TX-KEA)

##  Initial Release - 09/06/2023 

The Rally Analytics Platform provides actionable well-being and academic data for teachers to better understand their students’ paths to success.

The features added to the existing Rally application for this release include:

- Adding metadata to source Staar Interim assessment data as well as NWEA Map assessment data for TX.
- Updating dbt code to combine multiple Stadium implementations into the Rally warehouse.
- Changing login flow to be OIDC compliant, allowing users to log in via the EdGraph app launcher.
- Increasing color constrast throughout the app to make Rally more accessible. 
