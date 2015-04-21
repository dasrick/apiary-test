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
    
### ATTENTION

under mac osx there will be problems when using node.js higher than `v0.10.*` ... if it was installed via 
brew, then just switch back to an older version ...

* check installed and cached versions of node with `brew info node`
* switch back to an older version with `brew switch node 0.10.35`