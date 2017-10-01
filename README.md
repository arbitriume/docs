# Arbitriume

## Tech
* Backend: 
  * Database: MongoDB
  * API: GraphQL
  * Server: Koa
* Frontend:
  * DOM: React
  * State Management: Flux(pattern) - Redux
* D3 (for admin stats)

### Third Party
* [Beer Advocate](https://www.npmjs.com/package/beeradvocate-api)
  * [Source code](https://github.com/billism1/beeradvocate-api/blob/master/index.js)
* [Rate Beer](https://www.npmjs.com/package/ratebeer-api)

## Functionality
### Admin
#### Analytics (per timestep)
* Active Users
* All Users
* Users by Location
* New Subscriptions

#### Management
* Subscription
* Authorization 
* User Management
  * [AWS User Service](https://aws.amazon.com/cognito/)

### Public Consumer
1. User logs in
2. Dropped on some user summary page/feed
  * What's going on today?
  * What's trending?
  * What's popular?
3. Search for and select 
  * Brewery
4. Dropped onto Brewery summary page
  * Brewery Name
  * Follow/Save
  * Location/MetaData
  * Brewery Description
  * Recent Releases
  * Beer Roster 
    * Rating
    * Name
    * Description
5. Subscribe to separate beers
  * unfollow/unsave/save at this level
  * Push Notifications
  * Text/SMS
  * Email
6. Update option when beer data has changed since last crawl 
  
## Other Things
* How to verify brewers

## Things we need to build
* Script/Crawler to grab data from these websites
  * Pass data to graphQL API
* Authorization/privileges for different types of accounts
  * Libraries for this out there
* Ops job to archived information
  * Inactive/non-subscribed users after a threshold
* Payment Processing
  * How do we get it?
  * Where does it go?
  * File for LLC
  
### Frontend
* Home Page
* Profile landing page
* Brewery Landing Page
* Admin
  * Separate S.P.A
* Contact Us
  * Verify simple form
* Features
  * [Ulysses](https://ulyssesapp.com/features/)
  * Cards by category
  
### Crawler
* Ops job every day @ time
* Adhoc crawls per timestep per brewery view