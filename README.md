<p align="left">
  <img src="xhockware.jpg">
</p>

## Coding Challenge

> ### ⚠️ Read it first!
> The purpose of this challenge is to give us an idea about your coding skills.
> At XHOCKWARE we value well structured and tested code. Semantic HTML, modern and responsive CSS, a consistent coding style and a structured code base are important to us.
> I know... you probably love to code (we also love it!). But please, read this file until the end and make sure you understand the requirements before you start coding! If you have any questions, just let us know!
> ### ⚠ Please do not share this challenge ! ⚠


### Challenge
Build a Javascript application that contains a list and a detail view of news articles.
The application should be built with two columns and behave like this:

- The left side with the list of news articles.
   * When you click on one of the articles in the list, the content is shown in the other section and that article is marked as read.
- The right side with a detailed view of the current active article, or an empty view if none is selected.

The final app should look somewhat similar to the mockup below, but as long as you meet the criteria described above, you can build it in whichever way you find appropriate.

<p align="center">
  <img src="fe_hiring_challenge.png">
</p>

# Tech Requirements
## Frontend

### For Everyone
- Use Vue.JS/React/NextJS to build this application (MANDATORY).
  * If you think it makes it easier for you, you can start with some 

  Vue boilerplate (https://vue-community.org/guide/ecosystem/boilerplates.html).
  React boilerplates (https://dev.to/buildwebcrumbs/19-react-boilerplates-to-quickstart-your-project-56ge)
  NextJS boilerplate (https://vercel.com/templates/next.js/nextjs-boilerplate)


  * (FALLBACK) If you don't know Vue.JS or React at this time (don't worry about it... we all keep learning new stuff every day), you can use some other JS framework to build this application. 

- Please do the layout and styling with your own CSS (pre-processors are allowed). Don't use any component libraries like bootstrap or material-ui.

- Please try to implement a layout that shows emphasizes the relevant data points of each article(Title, picture, publish date, source, etc)

- Testing your code is important, we'd like to see some tests (full coverage not required).

- Use this README to document what you've built. Make sure that the person that reviews this code understands your choices and challenges:
  * **Use this readme to explicitly list and comment the features you decided to implement - we don't want to miss ou on anything...** - you can find the more advanced requirments identified as (Rn) bellow, to help you reference them in the readme
  * Outline your reasoning behind technical choices (architecture, third party libs, etc.)
  * Explain technical trade-offs
  * Anything you skipped due to time constraint?
  * What would you add if you had additional time for this project?
  
### Not challenging enough?

- (R1) Add a search functionality for the list view so we can reach certain articles easier. Search should filter the articles on the left side, and clear the panel on the right.

- (R2) We're showing too many articles on a single page. Implement pagination using client-side routing, so we only see 10 articles at a time.

- (R3) We like tidy code! Configure linting for your JavaScript and CSS files (you can use style guides like [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)).

- (R4) Let's say we need our application to support IE11. To a reasonable extent, ensure we can support modern Javascript in not-so-modern browsers.

- (R5) We all know designers love animations, so try adding some CSS animations.

- Anything else you'd like to show us? :)

### Advanced Level
Do you feel this is too easy, and that you are way better than this?
We allways prefer people with advanced knowledge and that can provide value in broader range of compentences.

**Things we would like to see from an advanced developer**

- (R6) Use VueX to store your data - All requests should then be directed to VueX Store So that a data set is stored locally
- (R7) Change the "search" and "paging" feature to operate over the VueX stored data rather than over the API
- We use Framework7 ([framework7.io](https://framework7.io)) for many of our ongoing and legacy projects. Instead of doing your own Vanilla implementation, we would like to see you use framework 7 to implement this project.
 * (R8) at first you can use framework7 standard features to implement your project
 * (R9) but afterwards you should customize the look and feel of the list to better enhance the looks of the article list column to highlight the key data points
- (R10) You should use media queries or other style sheet features to assure correct rendering on both mobile and desktop


## Backend 


We ask you to develop a simple API to serve content to the frontend environment

We use PHP as one of the main backend technologies, together with slim to implement the framework supporting routers and the full API description.
If you are not familiar with Slim, you can implement the backend using any other framework you want, like laravel or Symphony.



We provide you with a working API, that you can use to develop the frontend, and use to validate the requirements and overall objectives.

Main Goal : replicate exactly in PHP the same API provided as example.


### (Basic Tooling & API)
To get you started in the right direction, we give you with a working API and a couple of yarn scripts. But feel free to improve and extend it as you go through the assignment.

```sh
> cd api
> yarn install
> yarn api       # run API on 0.0.0.0:8000
```

The API serves the endpoint you'll need:

```sh
/v1/news?q=      # get the list of articles
```

Or if you want to use GraphQL

```sh
query GetNewsArticles($title: String){
  articles(title: $title) {
    author
    title
    description
    url
    urlToImage
    publishedAt
    content
  }
}
```

You can Run this server or to use this API, but we highly recommend it. If you really want to use another API, please give a good reason in the [Development Journal](#development-journal) section. If you feel the need to change the API or add something, feel free to do so.

> The data was obtained through newsapi.org


### Advanced Level
Do you feel up to it you can add a database to this. 
You can use PostgresSQL, MySQL, MariaDB or SQLite.

We allways prefer people with advanced knowledge and that can provide value in broader range of compentences.

Please provide the SQL to create the database (structure and data) replicating the above supplied API.

A Data abstraction layer is incouraged to concentrate all SQL/Database sintax specifics





### Submiting your code

To submit this challenge please do as instructed

1. Start by clonning this project your own GitHub account - **this is important because it establishes when you started working on this...**
2. Submit your final code as the lattest commit to the Master Branch.
3. Add 'joaopasrodrigues' as a colaborator on the project and set it as private
3. Let us know about it by sending us an e-mail with the URL to [tech@xhockware.com](mailto:tech@xhockware.com)

> ** ⚠️ PLEASE MAKE SURE THIS PROJECT ON GITHUB IS NOT PUBLICLY VISIBLE. **



Feel free to use different branches if you want to show different version - but make sure you let us know which ones you want us to look at...


### Notes

- The total working time should be around 6 hours. Focus on completing the [Frontend Tech Requirements](#tech-requirements) first and only then move to the Backend and then to the [Not challenging enough?](#not-challenging-enough) and [ Advanced Level](#advanced-Level) sections. This lasts sections is not mandatory, but with that done we can get more information on your coding skills.

- We'd like to see how familiar you're with Vue.JS and its features, but if you think you'll need another framework please explain shortly in the documentation section.

- In general, we'd rather see something simple you understand than something fancy you can't explain.

- Please don't use something you already developed.

- if you have any questions feel free to get in touch to [tech@xhockware.com](mailto:tech@xhockware.com) - we will try our best to get reply quickly

Happy coding & good luck! 🚀

---
## Development Journal

- Here you can pour all your thoughs and comment on your decisions throughout the project
- Feel free to leave sugestions 

