
# Usage

The expectation is that this command will be run inside your FOLIO development directory. For example, 

    some/path/                           -- Maybe your home dir or dev area
        folio/                           -- A folder for folio work
            posgres-config.json          -- Config file needed by mod-users et al
            folio_globals.yaml           -- A config file where we can share global 
                                         -- config for spring-boot based apps.
                                         -- we decided to go for something more general 
                                         -- than just postgres-config.yaml .
            folio-grails-module-demo/    -- Folder containing new module and descriptors
                folio-demo-module/       -- the grails app itself
            folio-sample-modules/        -- The defacto folio demo module
            mod-users/                   -- the users module
            okapi/                       -- okapi core
            raml-module-builder/         -- the raml module builder, in case you want to play

This structure is taken from https://github.com/k-int/folio-grails-module-demo. The expectation is that you will run the command

     grails create-app new-module-name --profile=com.k-int.grails.profiles:folio-service-module:1.0.0

Under the folio directory.


# Background

Initially created with grails create-profile folio-service-module

Grails documentation on profiles can be found here: http://docs.grails.org/latest/guide/profiles.html
