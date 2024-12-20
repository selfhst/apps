<h1 align="center">Change Log</h1>

### 2024-12-20

* Added tag option to filter directory by software with built-in support for selfh.st/icons

### 2024-12-02

* Fixed dynamic filter (alternative, software, platform) not loading when URL parameter is present

### 2024-09-17

* Added support for tagging favorites and caching via local browser storage (per suggestion from reader Mukesh G.)
* New 'Favorites' option in tag list to quickly filter by starred tiles

### 2024-09-15

* Rebuilt JavaScript logic to streamline directory load and accommodate source data structure changes
* Directory no longer includes sort in URL parameters when changed
* Transitioned icon soures to selfh.st/icons
* Icons for mobile apps remain in 'icons' directory, consolidated to root folder

### 2024-08-13

* Added subdirectory for ActivityPub platforms, clients, and tools
* Fixed project name indentation when no icon is displayed
* Fixed 'Software' filter not working correctly when switching subdirectories

### 2024-08-11

* Added 'Icon Type' to project details to identify square vs native icons
* Added 'project-icon-square' CSS class to add a border radius to square icons

### 2024-07-31

* New tile indicator for select applications that can self-hosted by third-party services
* Include third-party service names in search functionality

### 2024-07-23

* New sort option for randomly sorting projects
* Fixed order of alternatives in dropdown to be alphabetical

### 2024-07-19

* New default sort option (<i>Default</i>) to bring sponsors to the top of the directory (all other sort options deprioritize sponsors)
* Fixed default sort value not appearing on intiial page load

### 2024-07-16

* Changed the dark theme directory switch color for improved readability

### 2024-07-09

* <b>selfh.st/apps</b> and <b>selfh.st/companions</b> have been consolidated onto a single page. Users can easily switch between the two using the Software/Companion switch.
* Tags and source details are now hidden by default. Users can hide/unhide them in bulk using the <b>Details</b> toggle at the top of the page.
* Details for individual tiles can be expanded and collapsed by clicking a tile when the <b>Details</b> toggle is disabled
* Closed source projects can now be filtered when browsing the directory using the <b>Closed Source</b> toggle at the top of the page
* Project icons not found in the [dashboard-icons](https://github.com/walkxcode/dashboard-icons) repository are now being maintained and stored in the project's repository. The work has been started to transition all icons to independent maintenance to eventually be loaded as sprites for optimization purposes.
* Readability of project details has been improved by justifying values to the right and adding a dotted line separator between identifiers and values (inspired by the [OpenAlternative.co](https://github.com/piotrkulpinski/openalternative?ref=selfh.st) open-source project)
* Open-source companion project tiles now include license, latest version, and last activity details
* URL properties for some attributes have been updated to improve the readability of shared links
* The <b>Platform</b> filter for companion apps has been replaced with a <b>Tags</b> filter. Users should utilize search to filter by platform.
* Lazy loading has been implemented to improve page load speeds by only generating 100 tiles at a time

### 2024-06-25

* Changelog start