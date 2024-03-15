Hard
We will create a Shopping Scroll App. We will implement a load-on-scroll functionality. We don't have to change anything inside App. js
API: https://content.newtonschool.co/v1/pr/63b6c911af4f30335b4b3b89/products?page=${page}&limit=5

Use page = 1 for first 5 items, page = 2 for next 5, and so on..
[
{
id: 2,

title: "Mens Casual Premium Slim Fit T-Shirts ",

price: 22.3,

description: "Slim- fitting style. some long description",

category: "men's clothing",

image: "https://fakestoreapi. com/img/71-3HjGNDUL. _AC_SY879. \_SX. \_UX. \_SY. \_UY_. jpg"

rating: {

rate: 4.1,

count: 259

}
}
]

For shop. js
We have an input element with className = shop- input which will help us search items by the value we enter in it.
A div with className = shop- articles.
Inside this div, we will render 5 divs initially with className = article which will represent the articles.
Each article will have following data in given order:
h2 element with className = article- title which will contain the article's title from JSON
Three p elements will contain the article's price, category, and description respectively. As it is from the JSON.
An img element which displays the article image using the article's image URL from JSON.
At last in the p element we will display the article's current rating and the total number of ratings as "rate, count" from JSON.
Initially, 5 articles should be rendered by default.
After we scroll to the bottom, 5 more should be rendered keeping the previous 5.
Scrolling to the bottom should add 5 more articles as divs.
Typing anything in the shop- input should show only those articles which contain that text typed in the input as the article title or description.
Note: We have to render new articles only at the bottom of our page. Not even 100px above the absolute bottom.

Demo Video - This is how the website should work after solving
Test Cases

1.  loads the shop app and displays the title
2.  displays the search label and input
3.  displays shop articles with title, link, price, category, description, image, and rating
4.  loads more articles when scrolled to bottom
5.  doest no load more articles when scrolled to bottom
6.  filters articles based on search input
