# Rally Release Notes

## 5.0 - 08/20/2025

This release introduces groups and interventions, enhanced print functionality for reports and dashboards within Rally, adds support for assessments that do not include an overall performance level (e.g., MAP Fluency), and provides functionality to distinguish well-being survey administrations by term (e.g., fall, winter, spring). Additional improvements were made to assessment display logic, along with multiple bug fixes across assessments and surveys.

Breaking changes: None in this release.

New Features:
- The Groups and interventions feature is designed to help educators better support students by organizing them into custom groups based on shared characteristics or goals. With this new functionality, you can create custom student groups for projects or academic needs, instantly assign students to groups using pre-populated lists, easily manage and co-manage groups with colleagues, assign targeted interventions and track notes within each group.
- Grade Display Fix in MAP Scores Resolved an issue where some students were incorrectly showing the wrong grade next to their MAP scores in Rally. Grades now 
display accurately based on the most current student data.
- Enabled Print Functionality for Reports and Dashboards: Users can now generate print-ready versions of reports, charts, tables, and text directly from the Rally Student View. This includes support for printing from the browser as well as exporting formatted outputs. A guide on how to use the print functionality can be found here.
- -Well-Being Survey Term Selector: A new drop-down menu allows users to identify when a well-being survey was administered within a school year—specifically indicating fall, winter, or spring—providing greater clarity for interpreting longitudinal survey data.

Improvements:
- Support for Assessments Without Overall Performance Levels: Rally now accommodates assessments that do not include an overall performance level, such as MAP Fluency. These assessments can now be viewed and interpreted within the platform without issue.

Bug Fixes:
- Assessment-Related Fixes: MAP Assessment Date Alignment: Resolved a discrepancy in the displayed date for NWEA MAP assessments across EA products (Stadium, Podium, and Rally).
- SAT Histogram Layout: Addressed a layout issue in which the SAT histogram component would overflow its container, impacting visual consistency.
- Survey-Related Fixes: Survey Domain Persistence: Corrected a defect where domain-level results in the well-being section would not persist correctly when toggling between the Personal, Interpersonal, and Learning at School surveys.

## 4.0.0 - 05/22/2025

This release strengthens Rally’s security and backend infrastructure with a Node 22 upgrade and continuous vulnerability scanning. It also delivers important user experience and performance improvements—most notably, virtualizing the grade list for large districts. Several critical bug fixes enhance accuracy and usability across assessments, attendance, and student views.

Breaking changes: None.

New Features:
- Security Vulnerability Scanning in CI: A new vulnerability scanning tool (Sandworm) has been integrated into Rally. This proactively identifies security risks and ensures faster remediation.

Improvements:
- Node Upgrade to v22 (LTS): Upgraded backend from Node v20 to v22 for better long-term support, improved TLS/HTTP2 handling, updated OpenSSL libraries, and native tooling to detect unsafe dependencies. This helps prevent vulnerabilities and reduces engineering overhead.
- Removed Legacy Portal Login Strategy: Streamlined authentication system by removing deprecated login flows, contributing to better maintainability and security.
- Landing Page Performance Virtualization: Virtualized the long grade list, significantly improving performance on initial load, filter clearing, and home page navigation.
- TanStack Router Upgrade: Upgraded to the latest stable version of TanStack Router. This update improves routing behavior and requires updates to all internal route and link logic.

Bug Fixes: 
- Attendance Calendar Layout: Calendar containers now correctly expand to fit months with over 5 rows of data.
- Assessment Widget Filtering: Clicking the Math Assessment widget on “At A Glance” views now correctly filters the assessments to subject = Math (previously only ELA worked).
- Student Metrics Navigation Bug: Fixed an issue where the wrong student ID was being used when navigating between students in the metrics view.
- Behavior Page Scroll Fix: Fixed unnecessary scrolling caused by the student filter exceeding the page height.
- Well-Being Table Alignment: Fixed vertical alignment issue in the “At School” column headers—text now aligns to the top, matching line-wrapped headers.
- Assessment Table Sorting (Non-MAP Assessments): Sorting by sub-score columns now works correctly on all assessments, not just MAP.

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
