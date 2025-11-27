---
layout: without-toc
title: ShopComp 
---

# ShopComp

**ShopComp** is an online shopping-list maker and receipt sharing platform that helps you find the
best place to do your shopping. 

#todo (After css styling) Add pictures!


## Business pitch

Do you want to take your shopping to the next level? Sign up for a free account at 
[ShopComp.online](http://shop-comp-s3-bucket.s3-website-us-east-1.amazonaws.com/)
to start finding the best deals for your everyday items.

Once you sign up for ShopComp, you can start creating shopping lists for various different everyday
items, like groceries, household supplies, and toiletries.

After a shopping trip, you can upload your receipt by simply scanning them with your phone
camera and letting our AI image analyzer create a tabular list. ShopComp uses the prices
on your receipts to predict the prices of items on other peoples shopping list. It can even determine
the ideal store to go to where you can get the best deals. All your receipts are kept digitally,
allowing you to effortlessly search through your shopping history (no more paper receipts!).

ShopComp is a place for shoppers to come together to try and find the best deals when shopping.
The more people that contribute their receipts, the better ShopComp can be at predicting prices and
finding the best deals. Sign up for ShopComp today!


## Technical details

ShopComp was a collaborate effort between myself and three of my friends in a Software Engineering
course at WPI. The project idea was developed by [George Heineman](https://www.wpi.edu/people/faculty/heineman){:target="_blank"},
the professor of the course.

ShopComp is a full stack web application that uses **React/NextJS** on the frontend and various AWS
services on the backend, namely:
- **API Gateway** + **Lambda** proxy integrations for the RESTful API
- **S3** for static website hosting
- **Cognito** for user identity and access management
- **Aurora and RDS** to host the MySQL database

My main contributions where 


## See for yourself

Check out the website [here](http://shop-comp-s3-bucket.s3-website-us-east-1.amazonaws.com){:target="_blank"}! 
*Note: if the link doesn't work, it's likely we took the site down for cost reasons).*

Our code is publicly viewable in the following GitHub repositories: 
- [Frontend](https://github.com/Software-Engineering-Kappa/shopcomp-frontend)
- [Backend](https://github.com/Software-Engineering-Kappa/shopcomp-backend)


