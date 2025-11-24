# Leadership Analytics Release Notes

## 11/04/2025

The November 2025 release includes updates to parent contact information in dashboards, and model refactoring for the attendance dashboard.

New Features: 
NA

Improvements:
- The Attendance dashboard models were refactored in order to maintain the models and increase model performance.
- Physical address and display of home and cellphone numbers for parents of students has been added to the Chronic Absenteeism dashboard

## 10/07/2025

The October 2025 release includes improvements to the assessment filtering experience, the addition of student transcript information to the student profile, and the resolution of a “duplicate student issue” in courses.

New Features: 
- A table displaying students' course transcripts has been added to Student Profile to provide more insight into a student's academic history. The table will display underneath the current student grade list. 
- The Assessment Over Time chart has been modified to enable users to track progress more effectively across seasons and years.
- The filters on the Assessment page have been sub-divided to improve the filtering experience. The filters now include:
  - “Select Assessment” (or Family of Assessment)
  - “Select Subject”
  - “Select Test Grade”

Improvements:
NA

## 5.0.0 - 08/20/2025

This release introduces several enhancements aimed at improving usability and providing more detail across the Leadership Analytics platform. Improvements were also made to the Assessment dashboard to enable multi-season selection and update the order of assessment seasons to chronological order (Fall, Winter, Spring). Additionally, LA added discipline rate metrics and the number of incidents to the Behavior Dashboard, enhanced the Course Grade Dashboards with course and teacher information, implemented grade level ordering for clearer data organization, and loosened the required numeric grade filter to improve flexibility in grade reporting. Finally, LA improved the Section Profile dashboard to match the unique section definition across dashboards. A set of minor user feedback based improvements across dashboards. Please see the "Improvements" and "Bug Fixes" sections for a more detailed list.

Breaking changes:

- All dashboards:
  - Added grade to the list of student groups that can have flexibility with the backing variable in order to enable ordering. This will cause a break if the dashboards are update before edu_ext_podium
  - Added gender and race to the list of student groups that can have flexibility with the backing variable at a partner level
- Behavior Dashboard:
  - Added count of incidents to dashboard which relies on an edu and edu_ext_podium update. This will cause a break if the dashboards are updated before edu and edu_ext_podium

New Features:

- The Enrollment dashboard now has an "enrollment type" filter. This allows users to select one or more enrollment types.

Improvements:

- All Dashboards:
 - School year will now be displayed as academic year (e.g., 2024-25). This is configurable by implementation.
 - Grade levels now can be ordered across all dashboards
 - Student tables now use a new interactive table format with improved filtering, sorting, and ordering capabilities.
- Behavior Dashboard:
 - Added a metric to display discipline rate (number of students with a discipline action out of the total number of students overall).
 - Added the number of incidents to the Behavior dashboard, this includes: Number of incidents in school table, student table, and as a district metric
 - Over time chart now just displays number of discipline actions per day for clarity
 - Distribution of behavior and actions charts now displays Top 15 most frequent items for clarity
 - In Student Table, replaced Yes/No with number of In-School Suspensions and Out-of-School Suspensions for each student

- Section Profile & Course:
  - Improved resilience of the Section Profile dashboard by matching Section definition with Ed-Fi definition ( Section ID, Local Course Code, Session Name)

- Course Grade Dashboards:
  - Course Grades Snapshot no longer requires a numeric grade. Users can now select either a range of numeric grades or letter grades.
  - Users can now filter to specific courses by course information, local course information, or teachers.
  - Also added the new section definition to the filter in the Course Grades dashboards

- Enrollment Dashboard:
  - Add enrolled grade to the Student Table alongside the most recent enrolled grade

- Assessment:
  - Student Detail: Fixed a bug that caused the Select Student filter to be NULL

- Average Daily Attendance:
  - Add percentages to the tooltip of the Attendance Category Over Time chart to allow users to better understand the breakdown of the attendance categories at a point in time and over time.

- Assessment Dashboard:
  - Enablement of multi-season selection for educators to analyze the trends across multiple seasons of tests, for example, ACT and SAT. Order of Assessment Seasons in the dashboards was updated to follow the chronological order of Fall, Winter, Spring.

- Dashboard Descriptions:
  - Descriptions now include a date for the last time the description itself was updated

Infrastructural changes:

- Introduced a feature to the CLI Tool that allows implementations to swap the language used for student groups/programs

Bug Fixes:

- A bug that duplicated courses in the BI model originated in Stadium. This was fixed, but we are still tracking duplicates caused by co-teaching. We will aim to address that issue in the October release.

## 4.0.9 - 05/22/2025

This release incorporates a number of minor visual enhancements to the LA dashboard. Please review the “Improvements” section for a more detailed list.

Breaking changes: None in this release

New Features (if any): None in this release

Improvements:

- Search in filter values will now search across all values.
- Assessment dashboard tables will now reflect custom assessment labels
- Rename “School Year” to “Assessment Year” in Student Profile Assessment chart
- Assessment dashboards can now display assessments that have overall performance levels, but no scale score
- A variety of small visual enhancements:
  - Severity of attendance categories and/or category of chronic absenteeism indicated by stoplight color scheme.
  - Improved consistency of color palette across student group charts
  - Clarified language of most recent date across dashboards (With the exception of Section Profile)
  - Uppercase titles on all section separators.
  - Added separator in Profile dashboard below School table
- Updates to Chronic Absenteeism and Attendance dashboards:
  - Added Absence Percentages to Student and School (ADA only) tables
  - Changed metric name in School table from “Number of Students” to “Total Number of Students”
  - Updated chart descriptions for Attendance and Chronic Absenteeism to clarify data availability by selected date
- Updates to Behavior dashboard:
  - Clarification of subtitle of number of students in the district metrics
  - Changed filter name from “Discipline Type” to “Discipline Action”
  - Updated “Discipline Rate” metric name to “Actions per Student”
  - Enhancements to the custom assessment label logic to allow for labels to be set at the assessment or assessment family level

Bug Fixes:

- Profile dashboard: Fix bug that restricted discipline data from surfacing in dashboard consistently
  
## 3.1 - 03/27/2025
This release includes a variety of front-end adjustments to enhance and standardize the user experience.
- Assessment: Student Detail redesign to clarify selected year assessments vs assessment history.
- Remove separators between tables in Section Profile and Assessment: Student Detail
- Add "Search" to all school and student tables
- Update Most Recent Date language to be more descriptive and consistent
- Standardize order of student group charts for yes/no variables.
- Sort attendance rate charts so that the best attendance group is at the top of the chart
- Add timeline navigator to time series charts

## 3.0 - 01/28/2025

This release includes updating the Exchange SDK to V2.3.1.

## 2.2.0 - 09/24/2024

This release introduces a new cross-year assessment feature to the Assessment: Student Detail.

- The Assessment: Student Detail dashboard now allows the user to look at a student's historical assessment results. The tables and filters have an Enrollment School Year and Asssessment School Year. The user can select the Enrollment School Year to see the historic (enrollment year and previous) test results for those students. They can filter to a specific Assessment School Year if they only want to see assessment results from one year. 

## 2.1.0 - 07/23/2024

This release includes minor features across all relevant dashboards.
- Added a student filter to all dashboards with a student table to allow users to select any group of students.
- Increased the row limit to the maximum for the student tables to allow users to see as many students as possible.
- Revised the district metric section to improve visibility of titles.
- Updated Enrollment Status filter values on Attendance and Behavior dashboards
  
## 2.0.0 - 06/11/2024

This release introduces three new dashboards and a significant re-work of three existing dashboards. 

- Section Profile: This is a new dashboard that offers a comprehensive overview of the academic performance and demographic characteristics of the students in each section and/or educator's classes.Users can explore detailed information about the students in each section or educator's classes, including student grades, daily attendance, overall discipline actions, and demographic data aggregated by section.

- Student Profile: This is a new dashboard that offers a comprehensive overview of individual students, providing valuable insights into their behaviors, academic performance, demographic characteristics, and other student attributes.
  
- Course Grades Snapshot: This dashboard is replacing the D/F Counts dashboard. This allows users more freedom to chose a grade cutoff and see all of the students to have at least one grade that meet that criteria instead of just D/Fs.

- Profile Grades Change: The Percentage of Students at least one Non-Passing Grade chart is now based on transcript data instead of the most recent grading period in the grades resource. It shows the percentage of students who have at least one non-passing grade on any of their courses on their transcript in the chosen year. Denominator is the unique number of students with a course grade on transcript. This is calculated at the district, school, and grade level.
  
- Assessment: Changes to the assessment dashboard include improving chart selection and color schemes to allow users to make more meaning from the dashboard. 
  
- Asessment Student Detail: This is a new dashboard that provides information about assessment results at the student-level. The dashboard allows users several ways to filter the data, like filtering to one or more assessments and test seasons at the same time, selecting a performance level or student characteristics. 

## 1.2.0 - 04/07/2024
- Profile Dashboard: Change to allow district metrics to flow to Profile dashboard without staff data populated in the warehouse
- Update Exchange SDK to 2.0.9

## 1.1.0 - 03/10/2024

- Removed future exit dates from enrollment dashboard withdraw counts
- Added subheaders to district charts in Attendance and Chronic Absenteeism dashboards
- Enhancements to dashboard descriptions

## 1.0.0 - 01/31/2024

This version introduced a Profile dashboard that allows district administrators and school leaders to explore summary metrics related to domains covered in the platform such as enrollment, attendance, behavior, and grades. 

##  Initial Release - 09/06/2023 

Leadership Analytics is an application that enables school and district leadership to explore their data and more easily answer questions about their students. This initial release contains six dashboards.

1. Average Daily Attendance
2. Chronic Absenteeism
3. Enrollment
4. Behavior
5. Course Grades: Ds and Fs
6. Assessment

Detailed information about the metrics and business rules for each of those dashboards can be found in the "About this Dashboard" modal to the right of the selected dashboard title.

Users can navigate to any of these dashboards from a left-side navigation bar that can be expanded to see dashboard names and minimized when exploring selected dashboards.

Within each dashboard, users have multiple ways to interact with visualizations.
* Filters: Each dashboard has a filter panel where users can select data by school(s), student groups, and other data. Filters are applied by clicking "Apply Filters" at the bottom of the filter panel. The filter panel can also be minimized while viewing the dashboard.
* Cross-Filters Users can also cross-filter the dashboard by clicking within visuals and selecting a group of interest. Multiple cross-filters can be applied within each dashboard.
* Hover-Over: Users can hover over any visual to see additional information.
* Visual Menu: If they choose, users can also download the underlying data of each visual by clicking on the three-dot menu in the top right of a chart and selecting download and the format of their choice. The three-dot menu also allows users to view specific visuals in full screen or see descriptions of charts.

Each dashboard contains the most recent date of data for the metric displayed and a table displaying which filters have been selected at the top of the page. A "key metrics" section that contains district aggregates and high-level information of interest for that metric is located at the top of each dashboard. In the middle of each dashboard, there is a student table allowing users to quickly identify students of interest. Finally, at the bottom of each dashboard, the key metric is displayed by various student groups.
