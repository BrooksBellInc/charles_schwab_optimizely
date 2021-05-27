# charles_schwab_optimizely
Optimizely Training for Charles Schwab


Imagine that returning users with the cookie "expedited" with the value "true" are able to open an account more quickly than other users.
You want to create an A/B tests to see if highlighting the speed of creating an account leads to more brokerage account sign ups.
Use the following test information to create an experiment in Optimizely.

### Open An Account in 5 Minutes Test
Set up targeting and audiences
1. The test will run only on this URL: https://www.schwab.com/public/schwab/investing/accounts_products/accounts/open_an_account.html
2. Test will target all devices & browsers, but to qualify for the audience users must be returning visitors to the site and must have a browser cookie with the value "expedited" = "true"

Set up variations
- Test will have a control and one variation (Variation A)

For Variation A
1. Change headline from "Open an account in about 10 minutes" to "Open an account in about 5 minutes"
2. Change the font weight of the headline to bold

<img width="1641" alt="Screen Shot 2021-05-27 at 10 52 59 AM" src="https://user-images.githubusercontent.com/15365569/119848391-c78cb480-bed9-11eb-9452-f427b7647007.png">

Then, add metrics to your experiment:
1. Add click tracking on the 'select brokerage' radio button.
2. Primary metric should be clicks on the 'select brokerage' button
3. Secondary metric should be overall revenue per visitor

Finally, set traffic allocation & schedule:
1. Update traffic allocation to only include 25% of site visitors
2. Set experiment to begin on June 1st at 12:01 am EST and end on June 20th at 12:01 EST.

### Notes
- For this exercise you can use Optimizely's visual editor or the code editor. If you use the code editor, you'll need to use polling for any JavaScript changes. Refer to the documentation here: https://docs.developers.optimizely.com/web/docs/utilities for how to use Optimizely's waitForElement function.
- Optimizely recommends adding click tracking by saving the URL as a Page within Optimizely, then going to the implementation tab on the left, clicking "events" in the top nav, and creating the click event from that screen. For the purposes of this exercise, you can create the click event using this method OR within the visual editor for variation A of your experiment.
