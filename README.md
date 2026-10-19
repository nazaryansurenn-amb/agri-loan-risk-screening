# Agricultural Loan Risk Screening

**Geospatial AI for agricultural lending: assess a farm from space before the field visit.**

Agricultural loans are hard to assess. Farms are remote, records are thin, and a
season's outcome depends on vegetation health, water and weather that a loan
officer cannot see from a desk. Field visits are slow and costly, and they rarely
show more than one moment in time.

Agricultural Loan Risk Screening gives a lender a first, evidence-based view of a
farm in minutes, using years of satellite and climate history.

## What the product does

- **Starts from the parcel:** the loan officer draws the farm boundary on a
  satellite map; no data is needed from the borrower.
- **Reads five seasons of satellite history:** Sentinel-2 vegetation and moisture
  signals per growing season, with multi-year trends.
- **Recognizes the crop system:** distinguishes orchards and vineyards (perennial)
  from annual field crops, because their risks differ.
- **Measures climate exposure:** hail-prone conditions and early-spring frost from
  ERA5-Land climate data around the farm; frost counts toward the score only where
  it actually threatens the crop.
- **Produces a lending view:** a 0–100 screening score, yield, water, hail and frost
  risk levels, a suggested decision, a suggested loan-size factor, and the
  conditions that would reduce the risk (irrigation evidence, crop insurance, field
  visit).

## Who it is for

Banks, microfinance institutions, credit unions and agricultural insurers that
lend to or insure small and mid-sized farms, starting with Armenia.

## Product principles

**Human accountability.** The system screens and explains; it does not approve
loans. The credit decision stays with the lender.

**Explainable results.** Every result is broken down into the risks that drove it
and the conditions that would reduce them.

**Honest uncertainty.** Cloud cover, small parcels and missing seasons limit what
satellites can show; those limits must be visible, not hidden in a score.

**Local first.** The interface is built in Armenian for local lending teams.

## Current stage

Working local prototype: a map-based web interface and a scoring service on Google
Earth Engine, calibrated for Armenian conditions. The current scoring engine uses
transparent, rule-based indicators; trained ML risk models, validation against
historical loan outcomes, batch portfolio screening and bank-system integration are
on the roadmap. Not yet validated for production credit decisions.

## Related work

- [geospatial-ml-decision-support](https://github.com/nazaryansurenn-amb/geospatial-ml-decision-support)
- [geospatial-ai-assistant-platform](https://github.com/nazaryansurenn-amb/geospatial-ai-assistant-platform)

## Built with

Python · FastAPI · Google Earth Engine · Sentinel-2 · ERA5-Land · React · Leaflet

## About this repository

This repository contains a **product overview only**. It does not contain source
code, screenshots, scoring rules, credentials or deployable application files.

The implementation is proprietary and intended for future commercial development.
No open-source licence or rights to the implementation are granted here.
