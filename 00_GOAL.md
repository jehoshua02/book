# The Goal

The goal of this book is __to search for and propose the ideal in all aspects of
web application architecture.__

To satisfy the goal of this book we need to establish what we mean by "ideal"
pertaining to application architecture. I don't think we can adequately do this
without empathizing with the developer, the employer, and the users of their
applications.

First, "ideal" for me boils down to this: __simple__. And simple equals easy.
Easy to teach, easy to learn, easy to build, easy to test, easy to maintain.
This is huge. But simple does not mean stupid. Ideal application architecture
will not neglect any legitimate need of the application. So ideal to me also
means __robust__.

Because it's easy to teach and learn we don't need to rely on slow, expensive,
formal education systems to get developers up to speed. This saves developers
both time and money and lowers the bar for developers to start doing good work.

Because it's easy to build, test, and maintain, developers will not get buried
in technical debt that will slow them down. Their employer will continue to
enjoy a steady rate of delivery.

Because it's robust, we no longer will need to patch the application in strange
ad-hoc ways that won't be easy to maintain (*or teach, learn, build, test*),
thus upholding the first principle of ideal application architecture:
simplicity.

Users will ultimately benefit from this too since the application will always be
stable, regression-free, and developers who were once fighting technical debt
and application architecture will now be freed up to put more energy into
features to improve user experience.

We also need to identify all aspects of web application architecture. As has
already been mentioned, ideal application architecture will be robust,
providing for every legitimate need of the web application. The reason I say
"legitimate need" is because some needs are artificial, springing up out of
suboptimal application architecture. Looking at web application architecture
from a different perspective may eliminate these needs, especially as we
simplify things as much as possible.

So what are the legitimate needs of the application? To make sure we have only
the legitimate needs, let's focus on what the application actually does. I
suspect that the needs of the web application are quite finite and predictable.
While I believe that every application is unique, I also believe that most of
what every web application does is not. How it does what it does also does not
need to be unique. By identifying these things every web application does we can
then standardize the way they are done and do away with arbitrary variation,
which will tend to make things simpler, and thus, more ideal. In fact, I would
prefer that we not stop there, but also standardize how we do some of the more uncommon and esoteric things a web application might do. This actually has great
benefit because those things that are uncommon and esoteric we tend to forget.
This leaves us prone to reinvent the wheel or spend too much time rediscovering
or reaquanting ourselves with it. We can save ourselves time and headache by
standardizing especially

Here is a short list of needs

+ Authenticating user
+ Checking user permissions
+ Loading configuration
+ Fetching data
+ Caching data
+ Displaying data
+ Filter and sort data
+ Handling user actions
+ Saving data
+ Handling real time updates
+ Sending notifications
