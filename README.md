# apiary-test

a repo for testing of apiary and tools around ...

# local mock server

just run the install routine

    npm install

after this start the mock server

    # we have two variants of mock server
    npm run api-mock
    # we have two variants of mock server
    npm run drakov

## Validation

you can use the blueprint to validate against any URL ... 
Just run against the local mock server to verify the functionality ... in this case it is impossible to run into any
errors ;)

    # start local mock server
    npm run drakov
    
    # and the run dredd
    node_modules/.bin/dredd apiary.apib http://localhost:3000
    
if you want to run against the real backend implementation just replace the endpoint

    # example
    node_modules/.bin/dredd apiary.apib https://api.endpoint.com:12345

This tool (dredd) can be very helpful for continous integration with jenkins and co. ...

### ATTENTION

under mac osx there will be problems when using node.js higher than `v0.10.*` ... if it was installed via 
brew, then just switch back to an older version ...

* check installed and cached versions of node with `brew info node`
* switch back to an older version with `brew switch node 0.10.35`