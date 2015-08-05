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

We also cannot satisfy the goal of this book without identifying every aspect
of application architecture that we want to explore.

TODO expound a little

+ Loading configuration
+ Fetching data
+ Caching data
+ Displaying data
+ Filter and sort data
+ Handling user actions
+ Saving data
+ Handling real time updates
+ Sending notifications
+ Code reuse

Having established what "ideal" means for application architecture, and
identified every aspect of application architecture, we are ready to explore
each of them to find out the simple and robust way to implement them.
