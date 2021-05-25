# Islandora COAR Access Rights

## Introduction

A Drupal 8 module that creates a Confederation of Open Access Respositories (COAR) Access Rights vocabulary and terms for open access, embargoed access, etc. that can be referenced by repository items.

## Overview

This modules creates a `coar_access_rights` vocabulary and offers a migration definition to create taxonomy terms. You will need to add a field to a content type to refer to the terms, otherwise incorporate them into your repository (e.g. mapping to these terms in OAI-PMH).

## Requirements

* [Islandora 8](https://github.com/Islandora/islandora)

## Installation

1. Clone this repository into your Islandora's `drupal/web/modules/contrib` directory.
1. Enable the module either under the "Admin > Extend" menu or by running `drush en -y islandora_coar_access_rights`.
1. Import terms:
   `drush migrate:import coar_access_rights_term --userid=1 --uri=https://{your-site-domain-port}` .
   

## Configuration

None.

## Current maintainer

* [Catalyst IT](https://github.com/catalyst)

## License

[GPLv2](http://www.gnu.org/licenses/gpl-2.0.txt)
