# README

Sample application to setup Solidus ecommerce platform and configure Braintree payment gateway

### Steps followed to setup application

- Created new rails application with below command
```
  rails new solidus_demo --database=postgresql
```
- Setup Solidus into application by adding 'Solidus' gem in Gemfile and bundle install
```
  gem 'solidus'
```
- Setup basic configuration and migration by running below command
```
  bin/rails g solidus:install
```
- Run application
```
  bin/rails server
```
- Setup Braintree payment gateway into the application by adding below gem in file
```
  gem 'solidus_paypal_braintree', github: 'solidusio/solidus_paypal_braintree', branch: :master
```
- Setup new payment gateway configuration as mentioned in this link
[https://github.com/solidusio/solidus_paypal_braintree#create-a-new-payment-method](https://github.com/solidusio/solidus_paypal_braintree#create-a-new-payment-method)



### References

- [https://github.com/solidusio/solidus](https://github.com/solidusio/solidus)
- [https://github.com/solidusio/solidus_paypal_braintree](https://github.com/solidusio/solidus_paypal_braintree)

