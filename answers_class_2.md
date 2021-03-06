# answers_class_2
Working from DAT-DC-10/data directory

## Question 1
#### Command: 
  * `head chipotle.tsv`
  * `tail chipotle.tsv`

#### Answer: 
  * Each column describes an aspect of a Chipotle menu item, each row is an order or instance of a Chipotle menu item.

## Question 2
#### Command: 
  * `tail chipotle.tsv`

#### Answer: 
  * According to the order_id, there are 1834 orders.


## Question 3
#### Command: 
  * `wc -l chipotle.tsv` 

#### Answer: 
  * There are 4623 lines in this file.

## Question 4
#### Command:
  * `cat chipotle.tsv | grep "Steak Burrito" | wc -l`
  * `cat chipotle.tsv | grep “Chicken Burrito" | wc -l`

#### Answer: 
  * 368 orders of Steak Burritos, 553 orders of Chicken Burritos. Chicken is more popular than steak.

## Question 5
#### Command:
  * `cat chipotle.tsv | grep "Chicken Burrito" | grep "Pinto Beans" | wc -l`
  * `cat chipotle.tsv | grep "Chicken Burrito" | grep “Black Beans" | wc -l`

#### Answer: 
  * 105 orders of chicken burritos with pinto beans; 282 orders of chicken burritos with black beans. Chicken burritos more often have black beans than pinto beans.

## Question 6
#### Command:
  * `find .. -name "*.csv" && find .. -name "*.tsv"`

#### Answer:  

  * ../data/airlines.csv
  * ../data/bank-additional.csv
  * ../data/bikeshare.csv
  * ../data/drinks.csv
  * ../data/hitters.csv
  * ../data/imdb_1000.csv
  * ../data/titanic.csv
  * ../data/ufo.csv
  * ../data/vehicles_test.csv
  * ../data/vehicles_train.csv
  * ../data/yelp.csv
  * ../data/chipotle.tsv
  * ../data/sms.tsv

## Question 7
#### Command: 
  * `grep -r -i "dictionary" .. | wc -w`

#### Answer: 
  * 1522 case-insensitive instances of “dictionary”

## Question 8
  * 44% of orders of chips also had guac

  * number of orders of chips (1084)
    * `cat chipotle.tsv | grep Chips | wc -l`
	
  * number of order with chips and guac (479)
    * `cat chipotle.tsv | grep "Chips and Guacamole" | wc -l`
	
  * 479/1084 = 44% of orders including chips also included guacamole.

