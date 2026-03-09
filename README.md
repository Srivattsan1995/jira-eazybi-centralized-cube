# jira-eazybi-centralized-cube
This project introduces a centralized eazyBI cube designed to simplify and standardize reporting across Jira teams.

Centralized eazyBI Cube for Jira Reporting

**Overview**

This project introduces a centralized eazyBI cube designed to simplify and standardize reporting across Jira teams. Instead of creating independent cubes or rebuilding reports repeatedly, this centralized cube allows Jira engineers and analysts to:

* Import customized reports from eazyBI centralized cube
* Reuse standardized metrics and dimensions
* Build custom and complex reports without recreating data models
* Maintain consistency in reporting across projects and teams

The centralized cube acts as a single source of truth for analytics while still allowing flexibility for customized reporting.

**Objectives**

The main goals of creating this centralized cube are:

1. Standardization: Provide consistent reporting metrics across all Jira projects.
2. Reusability: Enable engineers to reuse existing report structures and calculated measures.
3. Flexibility: Allow teams to build advanced reports for complex use cases without modifying the base data model.
4. Efficiency: Reduce duplicated effort in creating cubes or rebuilding reports.
5. Scalability: Support reporting requirements across multiple teams and projects.

**Architecture**

The centralized eazyBI cube aggregates complex Jira requirements from multiple data sources and build it for reporting needs on case-to-case basis.

Data Sources:

- Jira Issues
- Jira Projects
- Custom Fields
- Existing eazyBI Reports
- Issue History / Status transitions

Core Components:

1. Centralized Cube:
- Aggregated dataset containing key Jira reporting dimensions
- Optimized for multi-project reporting

2. Standard Dimensions: Examples include:
- Project
- Issue Type
- Status
- Assignee
- Priority
- Sprint
- Time
- Custom Fields

3. Predefined Measures: Commonly used metrics such as:
- Issues Created
- Issues Resolved
- Average Resolution Time
- Story Points Completed
- Cycle Time
- Lead Time

4. Calculated Members: Reusable formulas created to support complex reporting logic.

**Workflow for Jira Engineers**

1. Import Existing Reports:

Engineers can import data and logic from previously created reports.

Steps:
* Navigate to eazyBI → Reports
* Select the centralized cube
* Import or reference an existing report
* Reuse existing dimensions and measures

2. Customize Reports for Complex Use Cases

Engineers can extend the centralized cube to create new reports by:

1. Adding MDX calculated measures
2. Creating custom dimensions
3. Filtering using project-specific attributes
4. Combining multiple metrics

Example use cases:

- SLA compliance tracking
- Cross-team sprint performance
- Incident resolution analytics
- Release readiness dashboards

**Benefits**

For Engineers

1. Faster report creation
2. Access to reusable metrics
3. Reduced duplication of work

For Teams

1. Consistent reporting definitions
2. Shared dashboards
3. Easier collaboration

For Organization

1. Centralized analytics layer
2. Improved governance of Jira reporting
3. Scalable reporting infrastructure

**Best Practices**

To maintain performance and consistency:

- Avoid creating duplicate calculated measures.
- Reuse existing dimensions and metrics whenever possible.
- Validate complex MDX queries before publishing reports.
- Keep cube refresh schedules optimized to prevent data latency.

**Cube Maintenance**

Maintenance tasks include:

* Scheduled cube refresh
* Updating custom fields when Jira schema changes
* Monitoring cube performance
* Removing unused calculated measures
* Versioning report templates

**Example Reporting Use Cases**

Some sample reports supported by this cube include:

- Sprint velocity tracking
- Team workload distribution
- Issue aging reports
- Resolution SLA compliance
- Bug trend analysis
- Cross-project delivery performance

**Future Enhancements**

Planned improvements include:

- Additional calculated measures
- Automated report templates
- Integration with external analytics tools
- Advanced performance optimization

**Centralized EazyBI Cube MVP - Solution.pdf** - This PDF document in Git repo is classified as MVP aligning towards the solution & engineering efforts behind the Centralized EazyBI cube design.

**YouTube Demo Link** - This video demonstrates the core development work in setting up the EazyBI centralized cube for Jira engineers to clone the predefined reports from the EazyBI console and use for creating complex reports based on the requirements.
Link: https://www.youtube.com/watch?v=oAsZbMJqDXw
