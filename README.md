# README


I'm doing some engineering work around email (sending email from a Rails app, receiving email in a Rails app) and more.

## Shapeup Iteration 1

I like the [ShapeUp](https://basecamp.com/shapeup) product design philosophy. To that end, here's the v1 spec of this app:

1. A user can sign up for "bragger" (via Google and/or GitHub), and in doing so, they will receive a weekly email asking "what did you accomplish this week?"
1. When they reply to the email, the contents will be saved to the current week of work
1. They can then log into their account and view all past answers
1. This service will charge a recurring fee or a one-time fee via Stripe
1. This service will enable one-click unsubscribes

I'm going to include detailed notes as I go, and I'll be using Chris Oliver's [GoRails](https://gorails.com/) quite a bit.

So far, I've run `gem update rails` and then `rails new bragger`.

### [How to use Action Mailbox in Rails 6](https://gorails.com/episodes/action-mailbox-rails-6?autoplay=1)

```
rails new bragger
cd bragger
rails action_mailbox:install
```