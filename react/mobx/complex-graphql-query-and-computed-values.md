# TIL: Complex graphql queries and computed values

I was using computed values to extract the view models from a single observable that contained a complex query result.
Bad idea.

It is better to save several parts of the query result as separate observable properties.
Then each computed value and mappers only act upon the small observable property.

*Protip*: Use fragments to define the model of those small parts!
