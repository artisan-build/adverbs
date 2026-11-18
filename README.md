# Adverbs

Tools and utilities to make us more productive when using Verbs

> [!WARNING]  
> This package is currently under active development, and we have not yet released a major version. Once a 0.* version
> has been tagged, we strongly recommend locking your application to a specific working version because we might make
> breaking changes even in patch releases until we've tagged 1.0.

## Installation

`composer require artisan-build/adverbs`

## Configuration

## Usage

## Memberware

This package is part of our internal toolkit and is optimized for our own purposes. We do not accept issues or PRs
in this repository. 


## Archived 2026-11-18

This repository is archived and read-only. Abandoned, and the dependency fix is not enough on its own: 4 larastan errors and a failing `pint --test` sit on top of it.

Its open "Drop PHP 8.4 from CI" pull request (#1) was closed unmerged at the same time. That PR was
not what broke CI here: `orchestra/testbench ^9.x` accepts only `laravel/framework` 11.x, and every
11.x release is now withheld by Composer's security-advisory policy, so `composer install` fails
before a test runs. The full diagnosis of all twenty repos in that sweep is in brain at
`projects/brain/reports/drop-php84-prs-2026-11-10.md`.
