# Stock

This software tracks stocks and uses data from Yahoo! Finance. It will be able to retrieve the most recent stock values, add or remove stocks from a list, and change the visual presentation to reflect gains or losses for the most recent day.

First, there is a normal REST API that loads the most recent stock price information from Yahoo! Finance; this API doesn't require authentication. To help us access and load data from the API, we'll build a service.

The dashboard screen with a list of cards is displayed when the programme first launches. Each card lists a single stock, its current price, and the day's price change (in both dollars and percentages). The cards will have a red backdrop for a negative change, a green background for a positive change, or a grey background for no change. Each of these cards is an instance of a component that chooses how to render the card based on the stock data.

/image s1

Last but not least, two links to the dashboard and manage views in the top navbar enable for easy switching between views. To set up these routes and control how the browser chooses which to display, we'll utilise the Angular Router.
The manage page with a list of the stocks will appear when you click the Manage link in the navbar. By selecting the Remove option, you can delete any of the stocks listed here. By entering the stock symbol in the text box and pressing the Enter key, you can easily add additional stocks.

/ image s2

Adding a new stock symbol to the input field and pressing Enter will add it to the list. Pressing the Remove button will remove it from the list. In both situations, the list of symbols is updated right away, and if you go back to the dashboard, the new list will be there.

