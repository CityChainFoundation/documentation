# City Chain - API Documentation #

The City Chain daemon has both a full RPC implementation from the Bitcoin-protocol, and it has it's own REST API. Both of these APIs are accessible locally from the machine that runs the City Chain daemon.

It is possible, through configuration file (city.conf) or launch arguments, to expose these endspoint to other IPs addresses, like another computer on the same LAN network, or even publicly.

WARNING: Do not expose your City Chain daemon to public traffic. It is very easy for anyone to shut down your daemon, or do other harm. There are no additional authentication on the API.

## Links

When running the City Chain daemon, you can access the documentation UI here: [http://localhost:4335/swagger/](http://localhost:4335/swagger/)

On the top right, there is an option to select version. Whenever major changes to the API is released, a new version will be made available. The previous versions is kept for compatibility. All features will not be available in all versions, new functionality is added on the new versions.

## API definition files

The API definitions is available in swagger file format:

[API Version 1.0](API-v1.json) (Contains most APIs, including RPC forward)

[API Version 2.0](API-v2.json)

## Endpoints

Ports can be configured through startup arguments, and they are standard:

- P2P: TCP PORT 4333 (Can be opened to public access to make the daemon a public fullnode)
- RPC: TCP PORT 4334 (Should be kept internal)
- API: TCP PORT 4335 (Should be kept internal)
- WS: TCP PORT 4336 (Web Socket endpoint, should be kept internal)

