
# Applied Data Science Capstone Project - Final Report

## Introduction

London, UK, is arguably one of the greatest cities in the world.  It is a tourist hotspot.  Those especially interested in “gastronomic tourism” have a plethora of restaurants to choose from, boasting cuisines from all over the world.  Choosing which areas of London to visit for the purpose of sampling great food could be challenging.

**Scenario**:  A budget-minded tourist has put 3 days of their trip aside for self-created foodie walking tours.  Each day will be devoted to one area of London.  Each day, a self-created tour will highlight the restaurants with very good ratings within that area.  On average, these restaurants together should have a medium or lower price range (so there could potentially be a higher priced restaurant in the mix as long as the other restaurants balance out the overall price).   

To summarize, the **question** we want answered is:  What areas of London offer the best foodie experience without breaking the budget?

**Audience**:  anyone interested in a sampling food from well-rated restaurants in London without spending too much money.  Additionally, the results will appeal to those interested in walking as a mode of transportation between restaurants.

In terms of area, our project will focus on a 15 km radius limit from London’s city centre.  The hope is to find clusters of restaurants in three different areas which meet our criteria.

## Data

Four datasets will be used to solve this problem.  The first 3 datasets will gather best rated restaurants from three different websites.  Further details on these restaurants will be gathered with the Foursquare Places API.  The Foursquare API will also be used to query restaurants within 15 km of London's city center, including prices and ratings from it’s users.  So, in total, we will have restaurant recommendations gathered from 4 different sources.  By using opinions/ratings from a range of sources we can be more confident of our final recommendations.


**1. TripAdvisor London Restaurant Ratings**  
The [Restaurants in London TripAdvisor page](https://www.tripadvisor.ca/Restaurants-g186338-London_England.html) lists    restaurants by user rating.  

  Data of interest:  Restaurant name, user rating.
  

**2. The London Eater website**  
The [38 Essential London Restaurants, Winter 2019](https://london.eater.com/maps/best-london-restaurants-eater-38) article gives us the names and addresses of it’s recommended restaurants.

  Data of interest: Restaurant name, address.


**3. Conde Nast Traveler website**  
This article lists the [30 best restaurants in London](https://www.cntraveler.com/gallery/best-restaurants-in-london) with prices.

  Data of interest: Restaurant name, price.

**4. Foursquare location data**  
The Foursquare Places API will be used to find restaurants within 15 km of London’s city center.  

  Data of interest:  Restaurant name, address, rating, price, category.
	

