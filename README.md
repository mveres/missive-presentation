# About Missive

![](https://lh3.googleusercontent.com/baBiSLGrkp81hBo8t7rQainAO8pGSI0AIKnK8D5jgHaOKHZBPa_UGRcfjNRRyz1mVA=s360-rw)

### Content

- the team
- app features demo
- the numbers
- tech side
- tracking
- testing
- deployment
- marketing
- interesting challenges

## The Team



## App Features Demo

> "Missive wishlists bring creativity and fun - and a bit of thoughtfulness - to the birthday gift experience. When the party settles, we’ll help you craft digital thank-you notes right in the app."

https://wishlists.getmissive.com/

- homepage with wishlists, recommendations, collections, age selector, thank-yuu todo's
- holidays' features
- account creation (OAuth)
- creating wishlists (categories, gender), adding items, sharing wishlists
- webapp to view the wishlist - claim a gift
- notifications (claimed, add items wishlist, upcoming event, new recommendations, new collections )
- record and send thanks
- view thanks
- ideas tab (consumes blog https://getmissive.com )
- deep linking

## The numbers

#### Metrics from production:
- users 618	
- wishlists 359
- wishes 1,285 (123 claimed)
- thankyous 14
_(some of these are tests)_

mixpanel.com for insights

## Tech side (architecture, components, tools)

### Mobile app
- react native app with EXPO
(camera, contacts, oauth, cloudinary, tracking, logging)

https://play.google.com/store/apps/details?id=com.getmissive.missive
https://apps.apple.com/us/app/missive-app/id1472427708#?platform=iphone

### API server
- node js, mongo, serp api, oauth, send-grid

### Web App
- node js, react, scss
https://wishlists.getmissive.com/

### Catalog Api
- node js, mongo, python

### Ideas Blog
- wordpress, mediabox plugin
https://getmissive.com/


## Tracking
segment.com
![SEGMENT](https://images.ctfassets.net/9u2t3ap6pctb/TqPBykc0TkvqnU2xsDkoi/84c6af769d793e86a6351b94bed0efc5/connections-hero-spot-2-02.svg "SEGMENT")


firebase analytics + facebook analytics + mixpanel

Events tracked:
   - sign in
   - create account
   - sign out
   - delete account
   - wishlist created
   - wish added
   - wishlist shared
   - thankyou shared
   - search
   - next recommended item viewed
   - collection viewed
   - empty wishlist notification clicked
   - wish claimed notification clicked
   - upcoming event wishlist notification clicked
   - new recommended items notification clicked
   - new collection notification clicked
   - app link clicked
  
sentry.io for logging

## Testing

Automated testing:
* jest snapshot testing (app)
* unit tests (app, api server)
* integration test (api server, catalog api)
* lint (everywhere)
* github workflows (catalog api), Circle CI (everywhere else)

### _Thank you to QA team!_

## Deployment

Mobile app:
- inside EXPO for staging and development
- app bundles for production: iOS and Android
- EXPO for buids and OVER-THE-AIR updates
- (EXPO CLI mini demo)
- drawbacks (firebase analytics, video recording, android group notifications)

Everything else:
- heroku for staging
- heroku for production
- (mini demo)

## Marketing 
* google
* facebook
* contests

## Interesting challenges
- webp image conversions (sharp)
- emails html (clodinary for image framing and resize)
- app synchronous updates
- mongo migration
- video recording and sharing
- catalog notifications

# Questions?
