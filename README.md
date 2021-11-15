# RequestPipeline_Webapi
Implementation of request pipeline using MediatR Pipeline behaviour

# What is pipeline behaviour

When user send request to an application it returns with response, these requests and response travel forth and back through Pipelines in ASP.NET Core. So, when you send a request, the request message passes from the user through a pipeline towards the application, where you perform the requested operation with the request message. Once done, the application sends back the message as a response through the pipeline towards the user-end.

# Validate the incoming requests even before it hits any of the application logics

A better approach would be to somehow wire up your validation logics within the pipeline, so that the flow becomes like user sends request through pipeline ( validation logics), if request is valid, hit the application logics, else throws a validation exception.

This is not only applicable for validations , but for various other operations like logging, performace tracking etc.

# What is MediateR

MediatR is an open source project and an implementation of the mediator design pattern.

The mediator pattern is a behavioral design pattern that helps to reduce chaotic dependencies between objects. The main goal is to disallow direct communication between the objects and instead force them to communicate only via the mediator

  # Neget used 
  
  - MediateR
  - Fluent Validations

