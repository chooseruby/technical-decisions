# General

Making technical decisions is a mix of:
- Having a good argument for choosing something
- A bit of flair to think about the future
- Some bias in what we like

Here I will add the first decisions that I took when thinking about this project. 

# Web framework: Rails

We will use Rails as the main web framework as this will help most people contribute. 

Also most people that learn Ruby will do it through Rails so we can be a place where they contribute.

## Vanilla Rails with a twist

1. We will use mostly vanilla Rails => we will use Hotwire and not any other library. 
2. We will write our views in ERB with the exception of components that will be in Phlex. 
3. We will pick Propshafts, Importmaps and SQLite as defaults.

# Testing

We will use Minitest and try to use fixtures where it makes sense.

The code in test should be:
- simple, not smart
- each test should include the preconditions (setup), assertions and post-conditions inside
- do not dry tests, except for cases when we really really use something is so many tests

# Gems

Here is a list of gems that I decided from the beginning to use: 

## Avo for Administrative Dashboard

We will use [Avo](https://avohq.io) as Admin dashboard. 
Avo is a new admin dashboard and it is built by [Adrian](https://github.com/adrianthedev) who contributes a lot in the community. He is also a very good friend. 

## Sitepress for managing static pages

We will use [Sitepress](https://sitepress.cc) to manage static pages. It is build by [Brad](https://github.com/bradgessler)
It is a nice way to manage static pages in either .erb or .markdown. It will help us with publishing content easy. 

## Phlex

For building components we will use [Phlex.fun](https://phlex.fun). It is build by [Joel](https://github.com/joeldrapper)
Phlex is Ruby and thus it will be a learning experience to use it.
We will use Phlex as a component system that will be composed in .ERBs
