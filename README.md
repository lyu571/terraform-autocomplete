# Terraform Autocomplete

WARNING! This is very beta, things might not work as expected so don't rely solely on this extension as a complete reference to terraform parameters and exported arguments. PRs welcome!

This extension provides basic autocomplete on TencentCloud resources. Scraping functionality can be found at https://github.com/erd0s/terraform-scrape.

## Requirements

Doesn't include any highlighting functionality or linting, will go well with [Mikael Olenfalk's Terraform extension](https://github.com/mauve/vscode-terraform) (but not required).

## What Works?
Hinting on TencentCloud resource types

![Hinting on TencentCloud resource types]

Hinting on resource arguments

![Hinting on resource arguments]

Hinting on variables `${<hints here>.<more hints>.<wow! hints!>}`

![Hinting on variables]

Go to definition for TencentCloud resources

![Go to definition for TencentCloud resources]

## What Doesn't Work?
* Any other providers than TencentCloud (could be added easily by adding to the [TencentCloud-resources.ts] file).
* Exporting attributes across files.
* Autocomplete on nested varibles, eg. `TencentCloud_s3_bucket_notification.somename.queue.<can't complete past here>`.

## Known Issues

I found that having the advanced terraform snippets extension enabled at the same time as this obscured the hints in some instances.

## Release Notes
