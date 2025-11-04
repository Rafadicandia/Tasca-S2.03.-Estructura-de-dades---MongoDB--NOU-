# Data structure - MongoDB


### Level 1
#### Optician Shop
An optician shop, called "Cul d'Ampolla", wants to computerize the management of customer data and glasses sales.

First, the optician wants to know the supplier for each pair of glasses. Specifically, they want to know the following information for each **supplier**: The name, address (street, number, floor, door, city, zip code, and country), telephone, fax, and NIF (Tax Identification Number).

For the **glasses**, the desired information is: The brand, the prescription for each lens, the frame type (rimless, plastic, or metallic), the frame color, the color of each lens, and the price.

For the **customers**, the shop wishes to store: The name, postal address, telephone, email, and registration date.
When a new customer arrives, store the customer who recommended the establishment (provided someone did recommend them).
Our system must indicate which employee sold each pair of glasses. Define the date/time when the sale is made.

**- Exercise 1**
Imagine we have the following graphical interface, from the point of view of a customer of the Optician Shop. How would you design the database to facilitate the information?

**- Exercise 2**
What if the point of view of the interface were the glasses?

### Level 2
**- Exercise 1**
You have been hired to design a website that allows customers to place food delivery orders online.
Take into account the following specifications to model the project's database:

For each **customer**, we store a unique identifier: Name, last names, address, zip code, town/city, province, and telephone number.

A person can place many **orders**, but a single order can only be placed by a single person. For each order, a unique identifier is stored: Date/time of placement, whether the order is for home delivery or for store pick-up, the quantity of products selected of each type, the total price, plus a note with additional information.

An order can consist of one or more **products**.

The products can be pizzas, burgers, and drinks. For each product, a unique identifier is stored: Name, description, image, price. In the case of **pizzas**, there are various categories that may change name throughout the year.

An order is managed by a single **store**, and a store can handle many orders. For each store, a unique identifier is stored: Address, zip code, town/city, and province.

Many **employees** can work in a store, and an employee can only work in one store. For each employee, a unique identifier is stored: Name, last names, NIF, telephone, and whether they work as a cook or a delivery person. For home delivery orders, it is important to store who the delivery person is that makes the delivery of the order and the date/time of the delivery moment.

### Level 3
**- Exercise 1**
We will try to create a simple model for a database for a reduced version of YouTube.

For each **user**, we store a unique identifier: Email, password, username, date of birth, gender, country, and zip code.

A user publishes **videos**. For each video, we store a unique identifier: A title, a description, a size, the video file name, video duration, a thumbnail, the number of views, the number of likes, and the number of dislikes.

A video can have three different **states**: public, hidden, and private. A video can have many **tags**. It is important to store which user publishes the video and at what date/time they do so.

A user can create a **channel**. A channel has a unique identifier: A name, a description, and a creation date.

A user can **subscribe** to other users' channels. A user can give a **like or a dislike** to a video only once. A record must be kept of the users who have given a like or a dislike to a specific video and at what date/time they did so.

A user can create **playlists** with the videos they like. Each playlist has a unique identifier: A name, a creation date, and a state indicating whether it is public or private.

A user can write **comments** on a specific video. Each comment is identified by a unique identifier: The comment text and the date/time when it was made.

---

## 💾 Database Models Structure
In every folder, you'll find a .png with the data structure for each exercise. 