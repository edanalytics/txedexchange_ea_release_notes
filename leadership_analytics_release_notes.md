
# Leadership Analytics Release Notes

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
