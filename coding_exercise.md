Coding exercise
===============

1. Look at this URL: [https://offersvc.expedia.com/offers/v2/getOffers?scenario=deal-finder&page=foo&uid=foo&productType=Hotel](https://offersvc.expedia.com/offers/v2/getOffers?scenario=deal-finder&page=foo&uid=foo&productType=Hotel)
    * It is a JSON API that presents a bunch of Hotel deals.
2. Note that there are certain query parameters that can be passed in, that will filter the results.  For example:
    * [`destinationName`](https://offersvc.expedia.com/offers/v2/getOffers?scenario=deal-finder&page=foo&uid=foo&productType=Hotel&destinationName=New%20Orleans)
      - alternatively, `destinationCity` or [`regionIds`](https://offersvc.expedia.com/offers/v2/getOffers?scenario=deal-finder&page=foo&uid=foo&productType=Hotel&regionIds=6126616,6057480) (for example [6126616](https://www.expedia.com/Wadi-Rum-Hotels.d6126616.Travel-Guide-Hotels))
    * [`minTripStartDate`](https://offersvc.expedia.com/offers/v2/getOffers?scenario=deal-finder&page=foo&uid=foo&productType=Hotel&destinationCity=New%20Orleans&minTripStartDate=:2017-05-03) (format: `:2017-05-03`)
    * also `maxTripStartDate`
    * `lengthOfStay`
    * `min`/`maxStarRating`
    * `min`/`maxTotalRate`
    * `min`/`maxGuestRating`
    * (maybe you can find more?)
3. Create a very simple site hosted for free on [Heroku](https://www.heroku.com/) that consumes this API as a server-side call and displays deals in an appealing manner. A few requirements:
    * The call should be server-side and not done as an AJAX call
    * The call should be dynamic (on each request) and not from a saved/cached file
    * Feel free to do it in a language of your choosing. For example, Java, Scala, Ruby, Python, PHP, NodeJS, Elixir. Please indicate in your `ABOUT.md` file why you picked the language you did  
4. Push your code to GitHub
5. Document the instructions for setting the site up in a local sandbox in your `README.md` file. Also document any assumptions you've made about the API or the runtime environment. And document any known issues with your example, etc.
6. In a file called `ABOUT.md`, document what you wanted to accomplish with your application. Include your thought process as you built the application. Also include what you learned in the process. Mention how much (or little) experience you have with the particular language and framework you chose.
7. Extra credit if your project builds and tests in Travis-CI: https://travis-ci.org/

Then share the links for the GitHub code and the site in Heroku.  These are what we will look for in the solution:

* **Readability**: Coding style, method/variable/class/etc. names, encapsulation
* **Structure**: Object design and code architecture. Try not to overarchitect your solution
* **Documentation**: Clarity of communication in your documentation. Also, the quality of your commit messages
* **Testing**: Approach to testing
* **Creativity** in choosing how to present the deals

**Additional notes:**
* Page design/layout, fit and finish, etc., are not that important.
* The sandbox setup instructions don't have to be foolproof (e.g., no need to make sure it works on every OS).  But they should be fairly easy to follow
* Keep the exercise simple.  This is not something that should take more than four to eight hours of effort for someone familiar with the technologies, and maybe twice as long for someone who's never used git and heroku before.