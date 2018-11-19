# social-networking-kata
Social networks.  Get you one!

This kata replicates how the delivery discipline within Pillar represents business value.  At Pillar, we begin solution and product development with value stories.  Here's what is defined as a value story:

> A value story is a statement of a particular chunk of business value expected to be realized by this project.  A value story is a one sentence expression of how value is achieved by a business case objective.  One project can have multiple value stories but one value story should not be spread across multiple projects.  Value stories may originate in a business case or return-on-investment document produced to justify this project.

From value stories we create user stories.  Here's the definition of a user story:

> A user story is a fine grained artifact that defines work within an agile cadence.  User stories should be the smallest piece of work that the business is willing to sign off on.

User stories relate directly back to a value story, and several user stories may be needed to satisfy a value story.  One value story has many user stories.

### Social Networking Value Stories

For this kata, we will focus on two value stories.

```
Reading My Friends Posts.

    As a social network user
    I want to be able to read my friends posts 
    So that I can stay updated on their happenings.
```

And...

```
Creating My Own Posts.

    As a social network user
    I want to be able to post a message
    So that my friends can stay updated on my happenings.
```

### The User Stories

These are the user stories.

#### Stories for "Read My Friends Posts"
```
Given I am in the application
  And Bob is another person on the social network
 When I enter "Bob's wall" at the prompt
 Then I should see Bob's ten most recent messages
```
```
Given I am in the application
  And Bob is another person on the social network
 When I enter "<My name> follows Bob" at the prompt
 Then I should be subscribed to Bob's wall feed.
```
```
Given I am in the application
  And I am subscribed to Bob and Sonya
  And Bob has posted several messages
  And Sonya has posted several messages
 When I enter "Latest wall posts"
 Then I should see a list of the last five messages from each of the wall feeds that I am subscribed to.
```
#### Stories for "Creating My Own Posts"
```
Given I am in the application
 When I enter "<My name> -> The clouds in the sky are amazing!" at the prompt
 Then I should see "The clouds in the sky are amazing!" posted to my wall feed.
```