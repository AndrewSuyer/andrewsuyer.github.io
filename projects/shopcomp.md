---
layout: without-toc
title: ShopComp 
---

# ShopComp

**ShopComp** is an online shopping-list maker and receipt sharing platform that helps you find the
best place to do your shopping. 


## Business pitch

Do you want to take your shopping to the next level? Sign up for a free account at 
[ShopComp.online](http://shop-comp-s3-bucket.s3-website-us-east-1.amazonaws.com/){:target="_blank"}
to start finding the best deals for your everyday items.

Once you sign up for ShopComp, you can start creating shopping lists for various different everyday
items, like groceries, household supplies, and toiletries.

After a shopping trip, you can upload your receipt by simply scanning them with your 
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

My main contributions had to do with user authentication. I set up an AWS Cognito User Pool to store
user credentials and validate user credentials. I constructed an authorizer for the user pool and 
attached it to the API Gateway endpoints, ensuring our API was inaccessible to unauthorized users.
Additionally, I build a login page where new users can create an account and existing users can log 
in with their username and password.

## Pictures

### Login page

![login-page](/assets/images/shopcomp/shopcomp-login-page.png)

### Shopper dashboard

The dashboard page shows some highlight statistics and allows the shopper to review their activity 
over certain time periods.

![dashboard-page](/assets/images/shopcomp/shopcomp-dashboard-page.png)

### Stores page

From the stores page, shoppers can view all stores that ShopComp knows about and create stores that
are not yet in the system.

![stores-page](/assets/images/shopcomp/shopcomp-stores-page.png)

### Receipts page

From the receipts page, shoppers can upload their receipts using an AI analyzer or manually with
a tabular interface.

![receipts-page](/assets/images/shopcomp/shopcomp-edit-receipt.png)

### Admin dashboard

The admin dashboard is a special dashboard where admins can review system information and recorded 
sales at all stores.

![admin-page](/assets/images/shopcomp/shopcomp-admin-page.png)

## See for yourself

Check out the website [here](http://shop-comp-s3-bucket.s3-website-us-east-1.amazonaws.com){:target="_blank"}! 
*Note: if the link doesn't work, it's likely we took the site down for cost reasons. You can 
checkout the frontend repository to see the website locally.*

Our code is publicly viewable in the following GitHub repositories: 
- [Frontend](https://github.com/Software-Engineering-Kappa/shopcomp-frontend)
- [Backend](https://github.com/Software-Engineering-Kappa/shopcomp-backend)

