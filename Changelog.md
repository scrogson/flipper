## 0.6.1

* Added statsd support for instrumentation.

## 0.4.0

* No longer use #id for detecting actors. You must now define #flipper_id on
  anything that you would like to behave as an actor.
* Strings are now used instead of Integers for Actor identifiers. More flexible
  and the only reason I used Integers was to do modulo for percentage of actors.
  Since percentage of actors now uses hashing, integer is no longer needed.
* Easy integration of instrumentation with AS::Notifications or anything similar.
* A bunch of stuff around inspecting and getting names/descriptions out of
  things to more easily figure out what is going on.
* Percentage of actors hash is now also seeded with feature name so the same
  actors don't get all features instantly.
