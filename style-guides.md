# Ruby

TBD

# Rails

We will adopt the following mental model when working with Rails:

## Controllers

The purpose of the controller is to get the request, pass it to an object to process it according with our business logic and then return the response in a specific format.
The controller can use callbacks or filters without abusing them.

## Models

The models can be either Active Record or simple POROs. 
They will as much as possible be namespaced.
They can use callbacks within a limited ammount. Do not abuse callbacks

## POROs

Try to reach for composition over inheritance. 


# Testing

Tests should never contain smart code (metaprogramming, one liners, extra fancy code, smart algorithms to execute testing).
Tests should be simple, linear and procedural. 
Tests should not have conditionals inside. 

