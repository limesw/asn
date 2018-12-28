# ADR 001: Create new site from scratch

## Status
accepted

## ADRs Superceeded
none

## Context
There is an existing site coded in Drupal 6. Problem is that tgis is very old Drupal version and new functionality is not created for it. We need to comply with GDPR requirements, as website is processing some personal identifiable data. The required modules exist for Drupal 8 only.

Three posibilities exist. Either do D6 -> D8 migration, create new site D8 site, or build a new site on differentplatform/CMS. 

There is a lot of existing data, mostly photos, forum data, articles, pages and comments. There are currently two Drupal themes used (winter and summer one).

Site is hosted at WebSupport and so far there is not much of limitation regareding DB type/version and PHP version supported.

## Decision
We had decided to build completly new site. New site will be built on latest release Drupal 8. There reasons are mostly that we want to take advantage of users already knowing their wau around the site, existing admins used to Drupal and finaly, Drupal is the only CMS I have previous experience as sitebuilder. 

We will not upgrade as there is no upgrade path for all modules used, while multiple new modules needs to be introduced. Also, we decidid not to migrate all content from old site, as it is not relevant any more. The exact scope of content migrated is to be decided. Starting from scratch also allows us to change the structure of site to better fit the way site is used now.

Creating custom CSM or using different one (for example Wordpress) would require a lot of investing for coding, training and support with no significant benefits.

We will move content in multiple stages, first moving ASN organization data, list of FKK sites in Slovakia, GDPR/EU Cookie compliance and support to create events/display calendar.

In stage 2, we will move galleries, forum, foreign nudist site section.

We may decide to create some social networks accounts for ASN and integrate them with website, but it was not discussed at the moment.

## Consequences

### Positive
List of sites was shared between Naturista and ASN, but we have no way to edit the map. It was already unavailable in the past, so we would like to keep it under our control. It is nice idea to share single DB of nudist sites betwen SR and CR, but a more appropriate way would be just to link site for particular country, so the most up to date is kept on one place.

There was a lot of outdated content that needs to be removed, so we can keep the old site as an archive while having lean new site with relevant data only.

There was ongoing problem with SPAM bots registering or posting to site and D6 modules to combat it are getting long in a tooth.

### Negative

Content needs to be moved between old and new site manually, that would require significant effort.

There will be some effort required for users/admins to get to know new site and its structure.

Some of the data will be migrated only once the stage 2 is completed, which could take several months to do as time I can invest here is very limited.


