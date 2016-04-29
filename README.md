#Audit of drupal applications

##Audit types:
* **Acquisition audit.** Acquisition audit generally done before the decision to buy a business. A part of the ‘due diligence’ process. Usually done to smaller startups who base their business to a web site / web service. Typically more in-depth. Focuses on whatever business plans there are for the system.
* **Implementation verification audit.** A customer want to validate their vendor’s work on their Drupal system. Usually pretty brief, done in collaboration with the implementing vendor. Shouldn’t ever be done for a system that’s not finished, unless it’s a strict architecture audit. Usually the client isn’t expecting major problems to be found.
* **Vendor management audit.** Vendor management audit is usually done to either switch vendors or due to problems with the current vendor. Usually done without the knowledge of the current vendor, thus done usually with limited documentation and/or information. Might be either very brief or very profound audit. Client expects to ﬁnd problems in the implementation.
* **Support audit.**  A very brief audit done to move the system to be supported by the auditing partner. These are done with minimal resources, but must be done well, because the vendor carries all the risks. The only type of audit where the auditing consultant can learn from the experience, as all the details will be revealed in the longer run.

## Steps:
* Read the NDA
* Get code and DB-dump (obfuscated)
* Get all access, (production if possible)
* Install the site 
* Get other configs (varnish, db, apache etc...)
* Look at the architecture
* Read the code (focus on cutom only). Beginers mistakes, security holes, performance problems.
* Social engeneering (talk to original site developers if possible)
* Test performance
* Use monitoring tools

## Performance and scalability audit
  * Site audit module
  * Watchdog (analyze and where is it)
  * Front
    - Google PageSpeed Insights
    - CDN
    - Image optimization
    - JS and CSS minification and gzip
    - Expiration headers
    
  * Back
    - Cache (general, panels, views, blocks, entity, render)
    - Master-slave DB
    - Missing module
    - Speed and amount of the queries
    - Fast 404
    - Performance module
    - Profiling slow pages
    - Separatly for anonymous and logined user
    - UI modules (views_ui, field_ui)
    - DB:
      * Analysis table size
      * Analysis big tables
      * Flat
      * Joins
      * Slow queries
      * Indexies
      
  * Envieroment ( performance + security)
    - Web server
    - Reverse proxies
    - DB settings
    - Search engines
    - Cache servers
    - Network settings
    - File system
    - PHP config
    - Backups
  

## Maintainability
* Where is code
* Where is logs

## Development workflow
* Git strategy
* Defects strategy

## Deployment workflow
* CI/CD
* Content staging
* Features, update scripts
* Post install hooks (clear cache, features revert, updates, etc...)

## Tests
* Unit tests
* Automation

## Security audit
  * Security review module
  * Security update
  * Hacked
  * User rorles and permissions
  * Config.php and files permissions
  * PHP module
  * Check_plain or format for user input
  * DB abstaction queries
  * JS XSS
  * Update.php access
  * Readme, version, etc. files
  * Private data without HTTPS
  * SSL

## Monitoring

## Code quality
* Static, mem and persistent caching
* Init hooks
* Slow backend API or 3rd parties
* Custom modules
* Custom theme
* JS and CSS analysis
* Coder module, code sniffers (use them only for custom modules)

## Longevity of deployed modules

## Core integrity

## General architecture and contrib modules selection
  * Justified functionality
  * Misusage contribs
  * Contrib modules settings
  * Only neccessary modules enabled
  * Search (solr/search engines, core, search_api, custom)
  * Integration with 3rd parties
  * Multisite configuration
  * Language configuration

## Content and data modelling
  * Content types
  * Terms
  * Entities
  * Users
  * Fields and relations

## SEO
* Seo audit module

## Accessibility

## Custom modules code review

## Features and code encapsulation

## Site configuration

## A basic site audit does not include:
  * full security audit for code vulnerabilities
  * cross browser checks for client site functionality
  * business logic checks for functionality
  
## Final Report
  * List of defects (architecture, content types modeling, modules, custom implementations)
  * Way to improve defects.
  * State of the application.
  * How to improve performance.
  * How to improve security.
  * How to improve code quality.

## Improve
Improve performance to improve overal user satisfaction, this results in more visits, more interaction, more leads, more conversion, more sales.
Improve security to steer clear from trouble and avoid painful loss of face.
Improve code quality to reduce maintenance costs and make future integration faster and more cost effectif.


## Who can do an audit?
The person doing the audit needs to be a real expert In Drupal audits, Drupal skills are not enough: the person needs to have rock-solid programming skills, especially in PHP. Also, experience in integrations, high-performance and security is hugely beneﬁcial.
