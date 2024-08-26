## Project MarketPlaceLab

An experimental marketplace platform designed to explore innovative concepts and practice advanced design patterns, pushing the boundaries of modern e-commerce solutions.

### Goals, Objectives and Ideas

* To experiment with various concepts, plugins and libraries.
  * API:
    * [ ] Scribe vs Scramble as tool for auto generating api documentation
    * [ ] Compare various tools to display api documentation 
    * [ ] Experiment with lomkit/laravel-rest-api package to explore api concepts
    * [ ] Best practices when designing REST API
  * Auth:
    * [ ] explore different auth options 
    * [ ] explore how to implement RBAC in Laravel
  * DDD
    * [ ] Experiment with DDD concept. Take inspiration from platforms such as Sylius and Magento.
  * Testing:
    * [ ] Unit
    * [ ] Feature
    * [ ] Api
    * [ ] Integration
  * Conventional Commits https://www.conventionalcommits.org/en/v1.0.0/
* Practice Design Patterns
* To have fun!

### Core Concepts and Definitions

#### Vendor
Vendor is a business or individual that offers products. Vendors create, manage, and list their offerings as well as offerings from other vendors.

Main features:
* Channel - Resource to hold all configuration  related to selling products
  * Each vendor can have only one channel (consider option to allow vendors  to have multiple channels)
  * Channel to have toggable features like website, api 
  * Dynamic validation rules builder based  on toggled features

#### Product
Managed by vendor. 
*  Can be sold on any channel once 

Main features:
* different product types that can be configured including extra fields

#### Coupon 
* Managed by vendor
* Can be created for channel or product or group of products
* Can be scoped to channel or multiple channels
* Rules can be built like in Magento
