# 12-factor-cookie-factory
A repository for a [12-factor](https://12factor.net/) app workshop with incremental steps through the 12-factor principles.

The repository follows a cookie factory that would like to scale their production while maintaining a decoupled and maintainable code base for all of their cookie production. 

They heard of magic tricks from Heroku known as the "12-factor app" principles that they would like to implement super-boost their new transition.

This repository is takes on the journey where the developer is able to see snapshots of the cookie factory's implementation journey where the milestones of a 12-factor migration would be implemented. 



The different snapshots are shown as directories:
1. Fantastic cookie recipes, and where to find them. 
2. One cookie recipe to rule them all!
3. Separating chocolate chips from cookie logic 
4. R&D cookie room to the cookie factory
5. The batter-bake-bite process.
6. Yuck, sticky dough!
7. The s'mores'n'gingerbread menace
8. Beating around the batter
9. Disposing the raisin cookie by-product
10. Cream-lining the sabayon-cookie
11. Customer cookie-faction pipeline
12. CCC: Cookie Cleaning Chaos!. 



In less fun but more informational terms:
1. Combine a dev and prod into one repo to ensure high cohesion, low incentive for drift, and easier CI integrations
2. Build an explicit configuration of all dependencies to ensure consitent versioning between developers.
3. Create a configuration that is separate from the codebase to ensure security for passwords, and avoid version cluttering when configuration changes.
4. Create a docker compose file to allow for local testing instead of relying solely on CI for feedback
5. Avoid cluttering the versioning with failed builds and deploying broken software by transforming a single-phase CI/CD pipeline to a multi-phased CI/CD pipeline 
6. Discovering the downsides of sticky sessions and how to avoid them by separating state from logic. 
7. increasing separation of concerns by utilizing port bindings instead of paths for a deployment of  a metrics server and a business app.
8. Scale co-routines increase performance of entire applications when waiting for IO-operations
9. Dispose unnecessary file dumps that are used for debugging and fills space on volumes after disposing of an app.
10. Heighten confidence that code acts similarly between dev and prod environment through identical OS between dev/prod.
11. Apply log aggregation analytics on said aggregation to leverage logs and avoid losing them when app dies. 
12. Create a docker image that spins up, cleans up database and then exits.


TODO: 
- make apps
- Separate into an org with several repos