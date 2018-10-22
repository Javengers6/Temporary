**Introduction and purpose**

  --Definitions, system overview and references--

  -> Web application name, logo and motto:
    -> What do we offer: Reliable, accurate, up-to-date, easy and fast to access information, secure transactions system and a chance to be a part of an interactive crowdsourcing community.

  -> What makes as different from existing services?

  -> Main purpose: Develop a web application that presents several information about different products, based on the input from the users, and allow the user to complete secure transactions.

  -> What types of products should we focus on?
    i. General approach, include every possible product that is registered by the users.
    ii. Focus on a certain type of products, for example:
      a. Technology
      b. Fashion
      c. Art
      d. Home and kitchen
      e. Automotive

  -> Should we focus on a certain group of people?



**Overall description**

**Product function**

  --System interfaces, user interfaces, software interfaces, communication interfaces--

  -> Software description: register and examine the value of several products found on nearby stores through our web service. The application is based on the method of crowdsourcing, where a group of people combine information to achieve a common goal, usually via the internet. In our case, the common goal is to keep track of the quality and the value of different products and optimize the customers choice.

  -> Can a user communicate with other users and the administrator?

  -> Each registered user will have a profile page
    -> What should we include in it?
      a. Personal information: full name, email, a sort bio and description, a profile image.
      b. Registration history, the amount of registered and bought products. Each user should also possess a bonus card which will keep track of his activity.  
  -     -> In order to present reliable information, each registration will have a review, so if it drops below a certain amount it will be automatically removed. In that way, we remove the biased and the info that is not up-to-date. In that sense, our page will have an autocorrection mechanism, based entirely on our users activity and feedback.  

**User characteristics**

  -> Types of users
    a. Registered user: update information via the user interface and the RESTful API
    b. Administrator: (Special type of password required) manage the accounts, i.e. he can delete or block a user
    c. Visitor: query our database with several criteria, such as location, time stamp and type of products

  -> Users actions
    a. Registered user
      i. Create an account
      ii. Connect using a username and an Password
      iii. Visit his profile page where he can manage his profile and delete his account
      iv. Register products, with a time stamp, a location, a value and possibly some general comments
      v. Communicate with the administrator and send feedback
      vi. Perform visitor's actions
    b. Administrator
      i. Verify administrator privileges through the use of a private key
        -> Should the administrator sign in from the users form or from a completely different one?
      ii. Access users information and track their history
      iii. Delete, modify or restore user accounts after their request
      iv. Perform visitor's actions
    c. Visitor
      i. Become a registered user
      ii. Query our database based on several criteria
        -> The search should be based on:
          i. His location: Sort the results, in order to present the entries that are close to him
          ii. Key words: We need some sort of search engine
          iii. Categories
          iv. Time stamp

    -> UML Diagram: Define the entities, their dependencies and their relationship in general.

    For example:
      -> Entities: User, Administrator, Products, Card...
      -> Relationships: user_is_registered, user_bought_product, user_registered_product, user_has_card...


**Constraints, assumptions and dependencies**

  -> Time, budget and human resources constraints: The development is taking place under a strict time limit of 3 months, with zero economical resources and by a group of 6. Therefore, we should prioritize our tasks and focus on the functionality of the application, which is the essential part.

  ->  How do we make profit from the application?
    a. Keep a percentage (5-10%) from the sales
    b. Use advertises, possibly with a dynamic approach based on the user preferences  
  -> The problem of parallel transactions, two or more people attempting to buy the same product.

**Specific requirements**

  --External interface requirements, Functional requirements, Software system attributes--
    -> Reliability: Present reliable information.
    -> Availability: The application has to be constantly available.
    -> Security: Use the secure version of http, which is https and it means that all communications between the website and the browser are encrypted. In that way, customers information like credit card numbers cannot be intercepted and potential customers are more likely to trust use. To achieve that, security certificate (SSL) that can be verified by the certificate authorities must be installed.
    -> Maintainability: After the completion of the project, a regular functional control of the application to detect any abnormalities.
    -> Portability: Mobile/tablet app or web service?
