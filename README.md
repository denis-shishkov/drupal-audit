#Audit of drupal applications

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
    
  

## Maintainability
## Development workflow
## Deployment workflow
## Security audit
  * Security review module
  * Security update
  * Hacked
  * Permissions
  * Config.php and files permissions
  * PHP module
  * Check_plain or format for user input
  * Update.php access
  * Readme, version, etc. files

## Monitoring

## Code quality
  * Custom modules
  * Custom theme
  * JS and CSS analysis
## Longevity of deployed modules
## Core integrity
## General architecture and contrib modules selection
  * Justified functionality
  * Only neccessary modules enabled
  * Search (solr/search engines, core, search_api, custom)
## Content and data modelling
  * Content types
  * Terms
  * Entities
  * Users
  * Fields and relations
## SEO
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
