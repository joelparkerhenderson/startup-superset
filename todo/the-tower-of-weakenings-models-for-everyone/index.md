# The Tower of Weakenings: Models For Everyone

By Aria Beingessner

https://gankra.github.io/blah/tower-of-weakenings/



The Tower Of Weakenings is simply the idea that having One True Model is a frustrating and futile endeavour that leaves no one satisfied. 

Instead, we should have a tower of models. The top model emphasizes “what users should think about”. As you descend the tower, the models become increasingly complex, but critically always more permissive than the ones above it. At the bottom of the tower is “whatever the machine actually does”.

Here is a sketch of what a tower looks like for a computer program:

  * The “Nice” Model: a simple friendly model that you can teach.

  * The “Real” Model: a messier model that allows for useful deviations.

  * The "Base" Model: whatever the machines actually do.

Here is a sketch of what a tower looks like for a service business:

  * The "Nice" Model: The customer is always right.

  * The "Real" Model: The customer is sometimes wrong, and here are some of the circumstances, why they happen, and how to handle them.

  * The "Base" Model: The customer-employee practices are specified in the employee handbook, maintained by our human resources department and audited by our legal department.

As you descend the Tower Of Weakenings, you have to deal with the reality of everything getting fuzzier, or more complex, or more technical.

The Tower Of Weakenings rejects the possibility of serving all the above concerns with just one model. Instead, the Tower provides each person with a Really Great Lie that we can all agree to pretend is true in order to make everyone’s job easier. 

The lies are part of The Tower Of Weakenings: if someone follow the model at one level, then whatever the other models might be won't actually matter. 

  * A new front-line employee can use the "Nice Model" starting on day one. Everyone accepts that the new employee will err on the side of the customer being right.

  * A long-time mid-level manager can use the "Real Model". Some customers will have exceptional circumstances, or unusual needs, or special orders. Everyone accepts that the manager's can field escalations and exert special powers, to bring together customer needs and company needs.

  * A legal-expert VP can use the "Base Model". Some practices have legal risks and repercussions, such as published product warranties and service guarantees, and these need close examination and specific research. Everyone accepts that this Model needs complex language, beyond most people's ability to use day-to-day.

As far as I am concerned, The Tower of Weakenings is horrifyingly effective. Like really it’s actually fucked up that I can hand out wins like this by just saying “but what if we just all agree to pretend things are simpler most of the time?”.

This whole mess is why Strict Provenance is such a nice simplification to a memory model: it just puts it foot down and says No Absolutely Not You Do Not Get To Get Lucky.

But of course, Strict Provenance is “a lie”, so you still can get lucky, so what’s the point? The point is that if everyone agrees to just pretend that you’re not allowed to do int-to-ptr casts, then having our sanitizers default to the strict semantics is actually useful and effective! Programmers that opt into this game also don’t have to worry about “are we doing PNVI-ae-udi” or something else, because… it doesn’t matter! Tower Of Weakenings Baby! Allowing any kind of int-to-ptr shenanigans is definitely weaker than forbidding them completely!

But ok we have all this code that does pointer crimes, this is useless! It 

Strict Provenance does a lot of weird little things for a lot of people, but going into all the weird side-benefits would take forever and I want to just focus this post on memory-models. TL;DR It’s Kind Of A Big Deal, For Many Reasons.

It's best to make it more explicit as to whether you’re actually playing this game or not. 

Having an actual semantic distinction allows people to operate in a “mixed” mode where code that is playing along with strict provenance isn’t exposing addresses and will generally be more strictly checked, but code which isn’t playing along gets more leeway and we still let you Get Lucky sometimes.


