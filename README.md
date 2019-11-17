# Airbnb Exploratory Analysis

## Problem Statement

I completed this short technical exercise as part of a job application. I was given the data set 'AB_NYC_2019.csv' and asked to conduct exploratory data analysis and produce a 10 minute presentation of my findings. I was required to demonstrate:

- a general understanding of what the data is, including an assessment of its quality 
- some analysis I have carried out to show findings of interest in the data
- suggestions for data science techniques I would apply if I had more time

## Files

This depository contains the raw data set as a csv file, the Jupyter notebook I used to conduct analysis (I mainly used Pandas and Matplotlib), the presentation slides in pdf format, and a folder of graphics that I used in the presentation slides.

## The Data Set

The data set consists of Airbnb listings in New York City (NYC). There are 48895 data points with the following columns:

- id: Unique identification code for the listing
- name: Descriptive name of the listing
- host_id: Unique identification code for the host
- host_name: First name of the host
- neighbourhood_group: Neighbourhoods are grouped into NYC boroughs
- neighbourhood: The name of neighbourhood of the listing
- latitude: A numeric variable that combining the longitude to represent the location of the listing
- longtitude: A numeric variable that combining the latitude to represent the location of the listing
- room_type: A categorical variable including Shared Room, Private Room or Entire Room/Apt
- price: The price of the listing
- minimum_nights: The minimum number of nights the host requires to book their property
- number_of_reviews: Number of customer reviews regarding the listing
- last_review: Date of the last review
- reviews_per_month: Number of customer reviews per month
- calculated_host_listings_count: Number of listings each host has simultaneously
- availability_365: The number of days that the listing is available in a 365 days, which is pre-defined by the host

A cursory internet search showed that the data comes from Inside Airbnb (http://insideairbnb.com/) - an activist project that provides data and analysis about Airbnb. It consists of publicly available data that was compiled from Airbnb.com, cleaned, and processed on 6 Aug 2019. This means that the data is clean and consistent (e.g. hosts have unique host_id and neighbourhoods are consistently labelled and match with city definitions), but it is limited in scope. That is, it is limited to the publicly available information on the Airbnb website. So we lack, for example, a detailed rental history for each listing.

## My Analysis

At first I spent some time just exploring the data and getting a feel for its scope and limitations. I became interested in the question of how hosts were using Airbnb: casually - the way it was 'intended' to be used - or more like a full time business. I identified availability_365 and minimum_nights as good indicators for this and so conducted short analyses of these variables on their own before examining their covariance. Since this was only intended to be an exploratory analysis I concentrated on getting a feel for the data through graphics and didn't apply any rigourous data science/statistical techniques.
