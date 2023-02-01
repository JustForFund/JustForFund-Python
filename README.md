# JustForFund-Python

Python library for interacting with the JustForFund API.

Install:


          pip install justforfund

First off. Define the following environment variables if you are interacting with:

  - Algorithms:

          JUSTFORFUND_ALGORITHM_API_KEY
          JUSTFORFUND_ALGORITHM_SECRET_KEY

  - Resources:

          JUSTFORFUND_RESOURCE_API_KEY
          JUSTFORFUND_RESOURCE_SECRET_KEY

      
    

Interact with:
  - Algorithms:

          from justforfund import algorithms_api
          
          algorithms_api.authenticate(JUSTFORFUND_ALGORITHM_API_KEY, JUSTFORFUND_ALGORITHM_SECRET_KEY)
          algorithms_api.upload_signal(algorithm_id, ...)
 
 - Resources:

          from justforfund import resources_api
          
          resources_api.authenticate(JUSTFORFUND_RESOURCE_API_KEY, JUSTFORFUND_RESOURCE_SECRET_KEY)
          resource_id = 5
          resource_dict = {....}
          resources_api.upload_signal(resource_id, resource_dict)
