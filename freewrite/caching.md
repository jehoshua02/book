# Caching

They say that the two hardest problems in programming are caching and naming
things. I tend to believe that neither are really that hard if you can think
clearly about them.

First, to explain what caching is for those not familiar, it is to store a
retrieved or calculated value that is frequently accessed or expensive to obtain
in a non-permanent location so that it can be retrieved more speedily in
subsequent requests. You might see caching in many forms and many places.
Function memoization is a form of caching. Lazy loaded class variables is
another form of caching. A general, specialized cache, that does nothing but
caching is the most easily recognized form. What makes caching hard is
invalidating and discarding cached values.

Invalidation, in my opinion, is the easy part. Invalidation is ejecting values
from the cache when they become stale. Time based invalidation is a common
method. But this is not the most robust method since the passing of time does
not necessarily mean the value has become stale. So what is it then that makes a
cached value stale? A retrieved value is really just a copy of the original
values stored in a more permanent place. So this kind of value becomes stale
when the original value is modified or deleted. That is when we should
invalidate a retrieved value. A calculated value is derived from one or more
original values. So when the original values, which are inputs to the calculated
value, are modified, that is when this kind of value should be invalidated. I
call this event-based cache invalidation. Care must be taken to do this kind of
invalidation correctly. The caching library should not be aware of what the
application is doing but instead provide a public interface that makes it easy
for the application to invalidate the right cache values when appropriate.

Theoretically, every value in the database could be accessed and placed in the
cache. This brings us to the second hard part of caching, the hardest part:
discarding. For any real application, loading the entire database into memory is
impossible and will probably crash the application. So we must impose limits on
how much will be cached, and when we are nearing the limit, and want to cache a
new value, we must choose one or more other values and discard from the cache to
make room.

Sounds easy right? Wrong. Even determining what the cache limit is is harder
than you'd think because it depends on the device. And today there are hundreds
of different devices all with different amounts of memory. Ideally, these
devices would provide an api to query the memory limit for the application and
we'd have a way to measure the amount of memory our application is consuming and
detect when we are getting close to the limit and discard as needed.

https://en.wikipedia.org/wiki/Cache_algorithms
https://en.wikipedia.org/wiki/Cache-oblivious_algorithm

TODO avoiding cache
