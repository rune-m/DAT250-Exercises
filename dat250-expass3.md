# Exercise report (3)

### Technical problems
After installing MongoDB 4.4 I couldn't run the mongo-shell with "mongosh" on my Mac. Had to install version 6.0 to make it work.

### Validation of installation package
<img width="749" alt="image" src="https://user-images.githubusercontent.com/54098894/189683911-7e06f18b-0a91-4ae4-b9c4-3cee4c1bf8c8.png">


### Experiment 1 screenshots

Find after insertMany (insert):

<img width="429" alt="Skjermbilde 2022-09-12 kl  15 35 22" src="https://user-images.githubusercontent.com/54098894/189681863-e4a58f33-8e42-4715-8836-40c01804f363.png">

Find query (query):

<img width="686" alt="Skjermbilde 2022-09-12 kl  15 34 13" src="https://user-images.githubusercontent.com/54098894/189681781-a90c848a-4172-4f7d-a531-ec12bb2d4b43.png">

Bulk write (bulk):

<img width="849" alt="Skjermbilde 2022-09-12 kl  15 41 51" src="https://user-images.githubusercontent.com/54098894/189681887-44af2e17-be6c-4ae6-8e7f-dfa1c13bc963.png">

### Experiment 2 screenshots

The first map-reduce shows how much each person has spent on orders. This is useful information to know, both from and customer and a seller aspect.

This map-reduce gives back an array with objects with customer id/name and total value of all their orders.

<img width="485" alt="Skjermbilde 2022-09-12 kl  16 28 50" src="https://user-images.githubusercontent.com/54098894/189682806-da03993c-8d7d-4421-9c9b-75c3498e7753.png">

The next map-reduce gives us information about how many orders containing each of the items, as well as total quantity for the orders. Count tells us in how many orders the item occurs in. One order can have more than one of an unique item, e.g. 3 apples in one order. Therefore qty (quantity) shows the total amount of ordered items. Avg (average) is (count / qty) and is the average number of items sold per order instance of the item.

<img width="564" alt="Skjermbilde 2022-09-12 kl  16 32 37" src="https://user-images.githubusercontent.com/54098894/189682821-584cda2a-d663-46c2-a501-425e036fa2d7.png">
