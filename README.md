# TIP App!






Today you'll be building an app for calculating your your tips & keeping track of the money you spend when eating out! You will be using a local API and building out the frontend for our app, Tipit.

<!-- ## Demo
Use this gif as an example of how the app should work.

![Demo](assets/demo.gif) -->

## Setup

- Fork and clone this repository
- Run `json-server --watch db.json` to get the backend started
- Open the `index.html` file on your browser

## Endpoints

Your base URL for your API will be: http://localhost:3000

The endpoints you will need are:

- GET `/meals`
- GET `/meals/:id`
- PATCH `/meals/:id`
- POST `/meals`

## Core Deliverables

As a user, I can:

1. See all the meal data in a `div` with the id of `"all-meal-data"`. When the page loads, **request** data from the server to get all of the meal objects. When you have this information, you'll need to add (create) a div with some HTML with the information about each meal. Each meal div should look like:

```html
    <div class="item card">
        <header>
            <h3>{meal restaurant } |<span> {meal experience rating} / 10.0</span></h3>
        </header>
        <p>Subtotal: <span>{meal subtotal}</span></p>
        <p>Tip Amount: <span>{meal tip amount}</span> <span>({meal tip percentage}%)</span></p>
        <p>Total + Tip: <span>{meal tip amount + meal subtotal + meal tax percentage}</span></p>
    </div>
```


2. Select a meal from the `"div#all-meal-data"` side panel and see the selected meal's info inside the `#detailed-info` div. 

3. Clicks on "Update" button to update the img and/or rating of the meal. Persist rating & image values to the server and update the DOM.

4. Click on the "Create" button to calculate the tip amount and subtotal and create a new meal card inside the `"div#all-meal-data"` side panel. The new meal should render on the DOM without refreshing the page and it should persist.

## Advanced Deliverables

> Note: If you are going to attempt these advanced deliverables, please remember to have a working commit with all the Core Deliverables first!

As a user, I can:
- Click on a `Delete` button to delete a meal. Persist the deletion to the server and update the DOM.
- Sort the meals displayed in the `"div#all-meal-data"` side panel by rating, subtotal (meal cost without tax or tip), total + tip, tip percentage, and/or tip amount

