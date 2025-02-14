# Test Plan for the Registration BB

Non-functional tests: 

1. All `examples` must be runnable via `docker compose up`.

2. Tests in `/test` will include the expected HTTP status codes for the current endpoints.

3. Via a basic SSH script we will recurse through the `examples` directory, run `docker compose up` for
   each example, wait until we get a running set of containers, and then execute
   the api endpoint tests for _that_ example.

Functional tests: 

1. ensure that application can be launched via docker with a adaptor and a security server (Information Mediator integration).
2. check that all defined API endpoints in the openAPI-spec.json return proper response codes.
3. check UI functionality for new registration service creation, User Interface and Flow Builder, rule engine configuration. Two different domain e-services will be created. 
4. check UI for new integrated service, where one e-service contains two or more registration applications integrated into one service. 
4. check UI for service publish. 
5. check UI for published Online Registration services.
6. check UI for processing screens in Online Registration services. 
7. process test applications sent via Registration BB from end to end.
8. integration test with Digital Registries BB: send data to a registry via Information Mediator after processing; 
pull data to the form from Digital Registries BB (or any BB); Evaluate user information from Rest API via Information Mediator.  




The output will be a ✅ or ❌ for _each_ example, for each of the tests.

## Comments

**Next Step:** 
