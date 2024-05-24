---
outline: 2
---

<!--
For each release create a new section at the top with heading including the version that clients would see in the app (i.e., 1.18.0) and release date, followed by subsections (if applicable) for:
- New Features
  New capabilities that we want clients to be able to use. Include screenshots or links to docs on how to use the new features.
- Improvements
  Any general improvements or fixes that are significant enough to make clients aware of.
- Deployments
  Updates or notes specific to self-hosted deployments. Include any new config changes, etc.
- Security
  Let clients know when security improvements are made, including severity as applicable (e.g., minor changes that are beneficial, major improvements that are recommended).

Once the release notes are approved and merged then notification should be sent to clients (TBD, via releases@paramify email list?).
-->

# Release Notes

> Notable changes and improvements to Paramify Cloud and self-hosted deployments.

<!-- >Subscribe to release notifications (TBD) -->

![paramify](/assets/hero-rocket.png)


## 1.31.0 (May 23, 2024)

### Improvements

- Elements: Added initial global import and export for Inventory
- Issues: Added ability to filter by Deviation status
- Issues: Added ability to specify impacted assets
- Issues: Added support for multiple originations
- Issues: Improved Links editing and shows favicon for known domains
- Issues: Link valid CVE IDs to NIST summary page
- Fixed Collections to also include Software as a filter option
- Fixed Documents for POAM to include CSP, System Name, and other metadata
- Fixed Documents for POAM to include more fields for Deviations
- Fixed Documents to correctly identify Inherited originations
- Fixed Documents to improve Inventory workbook for FedRAMP Rev 5
- Fixed Documents to show open and closed POAMs on proper sheets
- Fixed Imports of Elements to not warn when missing unnecessary fields
- Fixed Issues to report "changes saved" on updates
- Fixed Projects from reporting a 500 error after deletion
- Fixed Projects security impact level from extending off small windows
- Fixed Projects to delete diagram images on project deletion
- Fixed Projects to import proper catalog for StateRAMP
- Fixed Projects to include Alternative Implementation in CMMC SPRS score
- Fixed UI dropdowns to select when clicking anywhere in row
- Fixed UI to include page titles on all pages

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.30.0 (May 13, 2024)

### Improvements

- Controls Implementation: Adds full text search to Link Risk Solutions view
- Documents: Added KEV (Known Exploited Vulnerabilites) to generated POAM document
- Documents: Updated POAM generation to include more details of Deviations
- Issues: Added ability to show/hide Due Date column in list view
- Issues: Added more data including Point of Contact, Impacted Requirements, and Links
- Issues: Added option for Admins to delete all Issues (with warning)
- Issues: Added Status Date to detail view and generated POAM document
- Issues: Improved overall layout of detail view
- Issues: Included Activity log of changes to list and detail views
- Fixed Documents to properly set Inherited originations checkbox
- Fixed Issues to show consistent UTC-based milestone dates
- Fixed Projects to preview result when changing impact level to Default


## 1.29.0 (May 7, 2024)

### Improvements

- Documents: Initial generation of FedRAMP POAMs documents from Issues
- Issues: Added ability to show/hide CVE in list view
- Issues: Added limited rich text descriptions where supported
- Issues: Allows manually setting or autogenerating unique POAM ID
- Issues: Made POAM ID and CVE visible and searchable in list view
- Issues: Supports importing from POAM template CSV
- Fixed Attachments download link for FedRAMP Appendix O template
- Fixed Attachments for TX-RAMP workbook to include parameters
- Fixed Attachments for TX-RAMP to better name workbook file
- Fixed Attachments to include both Acronyms and Glossary terms
- Fixed Attachments to properly identify Shared and Hybrid originations
- Fixed CMMC projects by removing unnecessary Data types selection
- Fixed Element imports to not warn about missing FedRAMP systems
- Fixed Images being deleted to also be removed from storage
- Fixed Issue detail to always show adjusted risk level
- Fixed OSCAL export compliance against NIST schema
- Fixed OSCAL export from mishandling non-string parameters
- Fixed Risk Solutions filters to sort Responsible role options
- Fixed Documents to prevent overflow of table cells
- Fixed Import dialogs to not remember previous filenames

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.28.0 (April 19, 2024)

### Improvements

- Issues: Improved detail view of Observations, Deviations, and Recommendations
- Issues: Initial version of OSCAL generation of POAMs
- Issues: Added initial ability to attach Evidence
- Issues: Added support for deleting Issues
- Projects: Added ability to create base project when creating new DoD project
- Projects: SPRS score included on CMMC dashboard
- Fixed Attachments to highlight and show newly created Custom Attachment
- Fixed Attachments for Li-SaaS projects to reduce list of required
- Fixed Attachments to prevent changing filename extension of generated files
- Fixed Documents to correct CSP inheritance in CRM and leverage Risk Solutions to explain customer responsibilities
- Fixed Imports to improve warning messages and identify missing fields in source file
- Fixed Key Contacts by removing FedRAMP contacts from CMMC projects
- Fixed Mentions to allow dragging the scrollbar when selecting Elements
- Fixed User management to better support multiple workspaces
- Fixed Warnings in browser on several pages related to library deprecations and improvements

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.27.0 (March 27, 2024)

### Improvements

- Attachments: Icons now indicate which are automatically generated or can download templates
- Documents: Added User Summary as Appendix S to FedRAMP Rev 5
- Documents: Policies and Procedures attachment added to CMMC (pre-beta)
- Implementations/Risk Solutions: Remarks now support mentions and rich text formatting
- Implementations/Risk Solutions: Tables in rich text can now set a header row
- Issues: Added summary dashboard, filters, sorting, and detail views for POAMs (alpha)
- Projects: Revision History can now be uploaded
- Fixed Advanced Parameters using "Show DoD" flag to be more persistent
- Fixed Attachments to show "Not Applicable" status as complete only with remarks
- Fixed Attachments view to properly refresh remarks when navigating
- Fixed Collections import to properly link applicable products
- Fixed Dashboard charts to include User/Role filters when clicking to detail view
- Fixed Implementations to remove unused parameters
- Fixed Imports to prevent submitting without selected file and improve various warnings
- Fixed Imports with images in rich text content with some storage providers
- Fixed Key Contacts to select the Person/Org created with "+ Create" button
- Fixed Paramify Cloud application "502" errors caused by large headers
- Fixed Project Dashboard "Select Control Set" link when no controls are selected
- Fixed Revision History to better sort version numbers
- Fixed Risk Solutions and custom responses mishandling images in text in some cases
- Fixed Risk Solutions to prevent deleting narrative when removing extra responsible role

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.26.0 (March 7, 2024)

### Improvements

- Implementations/Risk Solutions: Added support for images in rich text fields
- Documents: Initial CMMC document generation completed (pre-beta)
- Projects: Improved progress bars to animate progress and reduce shifting during load
- Projects: Adjusted dashboard progress to more heavily weight by count of controls
- Issues: Initial structure for POAMs support (alpha)
- Fixed Custom Response review status to be saved in project export
- Fixed Risk Solutions view to avoid shifting during page load
- Fixed Key Contacts to fit odd-sized images properly into avatar
- Fixed Project side navigation to properly highlight active Controls section


## 1.25.0 (March 1, 2024)

### Improvements

- Key Contacts: Made view more compact, including proper party icon and image, if set
- Controls Implementation: Show family/subfamily and sort by name in Link Risk Solutions view
- Elements: Always sort view by name
- UI: More consistent Previous/Next buttons and tooltips
- Fixed Key Contacts to always default by project type


## 1.24.0 (February 23, 2024)

### Improvements

- Projects: Initial NIST 800-171/172 catalogs and foundation for CMMC (coming soon)
- Advanced Parameters: Added "fast forward" navigation buttons to skip to previous/next incomplete
- Advanced Parameters: Shows current, total, and incomplete counts
- Project Dashboard: No longer shows sections which have no data
- Key Contacts: Removed unnecessary entries for FedRAMP projects
- Fixed Project Dashboard to report proper count of Custom Responses, if any
- Fixed Advanced Parameters UI bug that could cause the window to not open or to close unexpectedly
- Fixed Elements minor UI issue when navigating after adding an image

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.23.0 (February 16, 2024)

### Improvements

- Show Element type icon and tooltip in list when selecting mentions
- Use substring search on short and long names for mentions
- Allow merging cells (horizontally) in tables within text
- Re-add Advanced Parameters and Project Settings to Actions menu on Control Implementations
- Quick "view" link to see control text when adjusting mappings on Risk Solutions
- Fixed error when clicking on certain parts of the Risk Solutions chart to see filtered views
- Added new "demo mode" to allow limited functionality in specified workspaces
- Rename attachments to new standard when migrating from FedRAMP Rev4 to Rev5
- Prevent deleting locked Organization object from workspace
- No longer generates empty Policies and Procedures doc when no controls are selected
- Corrected rare OSCAL generation error due to broken mentions
- Fixed error when navigating between Advanced Parameter Settings
- Updated certain controls to properly show as "withdrawn"

### Deployments

- Now supports Azure Blob storage in Azure Government (see [new config](https://github.com/paramify/support/blob/main/azure/values-local.yaml.example#L40-L48))
- Fixed use of persistent volume in embedded DB (may require backup/restore of DB)

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.22.0 (February 6, 2024)

### Improvements

- Optimized filters on Control Implementations to improve overall performance
- Able to filter Control Implementations by unassigned, leveraged system, review status, and response type
- Clicking Project dashboard donut chart now links to filtered view of relevant Control Implementations
- Fix some mentions becoming invalid during Risk Solution imports
- Fixed searching when selecting Main Component in Risk Solutions
- Ability to filter Risk Solutions by unassigned
- Added option to delete all Risk Solutions
- Fixed saving an empty Custom Response as a Risk Solution
- Added link from Project dashboard to see Custom Responses that are not reviewed
- Clarified difference between Users (accounts) and People (elements)
- Added reminder that MS Word is recommended for proper document viewing
- Fixed ordering in Project Overview when adding custom sections
- New option to easily deselect all Control Selections
- Prevent deleting the project-associated Plan element
- Updated Activity to always show latest User name
- Minor fixes to control requirements for FedRAMP Li-SaaS
- Added missing DoD Rev5 parameters

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.21.0 (January 19, 2024)

### New Features

#### Collaborators Approval Workflow

Collaborators have an optional new worklow to support approving Risk Solutions assigned to their Role. They can flag their Risk Solutions as "Approved" or "Change Requested" to assist Editors and Admins in their review process. If the Collaborator approves a Risk Solution the overall status will show as "Ready for Review", at which point an Editor or Admin can mark it reviewed. Note that this "Approval by Responsible Role" option will only be available when there is a Collaborator that is assigned a Role matching the Risk Solution.

![collaborator-approve](/assets/1.21-collaborator-approve.png)

Alternatively, if the Collaborator is unsatisfied with their Risk Solution and can't make the desired change (such as to Implementation Status or Responsible Owner) they could indicate "Change Requested" which will bubble up to those responsible for overall review. The Editor or Admin could then communicate with the Collaborator to address the feedback. Once satisfied they would click to "Resolve Change Request" and reset the Role approval status, after which they could wait for the Collaborator to approve or just mark it reviewed.

![collaborator-changes](/assets/1.21-collaborator-changes.png)

This Collaborator workflow is completely optional, and it is not required for Admins and Editors as they review Risk Solutions. It's intended to enable them to delegate part of the review process to Collaborators as subject matter experts to (optionally) edit and approve based on their responsible Role. See the related Collaborator Access options in Workspace Settings.

### Improvements

- Fixed performance issue waiting for document generation
- Options in Workspace Settings to restrict Collaborators to only see Elements and/or Risk Solutions assigned to their role
- When applying suggested Risk Solutions the default option is now to skip Control Implementations with existing responses
- Able to filter for linked Risk Solutions in Control Implementations
- Now able to review Custom Responses (similar to Risk Solutions)
- Added loading indicator while importing files
- Added ability to delete your own comments (or Admin can delete any)
- Improved Risk Solutions view for lower resolution screens
- Minor improvements to FedRAMP and DoD documents
- Better naming convention for document attachments

### Deployments

Added option for automated backups of embedded database.


## 1.20.0 (January 11, 2024)

### Improvements

- Search filters persist on Elements, Control Implementations, and Risk Solutions
- Limit next/previous navigation of Elements and Control Implementations within search results
- Click diagram thumbnails to show full-sized image
- Allow multiple Leveraged Authorizations in Custom Responses
- Ability to filter search of Control Implementations by Leveraged System
- Option to show only suggested Risk Solutions when manually linking to Control Implementation
- Option to hide titles on Custom Responses now under Project Settings
- More detailed error notifications on Element and Risk Solution imports
- Document generation errors now show as tooltip to facilitate troubleshooting
- Option to expand/collapse all response details in Control Implementation
- Searching Acronyms and Glossary now include definitions
- Various formatting improvements on FedRAMP Rev5 and DoD SSP documents

### Security

This release includes security-related dependency updates. Updating is recommended.


## 1.19.0 (December 21, 2023)

### Improvements

- Add section in Project Overview to allow automatic or manual listing of Leveraged Authorizations
- Deleting all Elements will replace mentions with text name in Risk Solutions and Custom Responses
- Option to delete all existing Custom Responses when importing Solution Responses in Project Settings
- Retain references to applied Risk Solutions in Project export
- Fix failure to import Parameters under certain conditions
- Improve sorting list of Project names and when selecting items from dropdowns

### Deployments

Allow connecting to SMTP servers with self-signed certificates by default.


## 1.18.1 (December 14, 2023)

### Deployments

Minor improvement to include some missing app logs in support bundles.


## 1.18.0 (December 7, 2023)

### Improvements

- Floating formatting toolbar will stay visible when editing long text in Risk Solutions and Custom Responses
- Able to filter Control Implementation by Origination and Status
- Notifications and warning messages will stay until closed
- Able to globally toggle titles on Responses in Project Settings
- Ensure high resolution images in documents

### Deployments

Allow sending SMTP mails without authentication by leaving either SMTP user or password blank.

### Security

This release includes security-related dependency updates. Updating is recommended.
