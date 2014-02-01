# httpServer

## About

`httpServer` is a library which provides a basic, yet flexible HTTP server, ready to be wrapped in server libraries. You can control response, and header requests. In the future, a primitive static server will be included in the future, to serve as a little helper. See `httpServer.static`, already included.

## Functions

### Handler

    func server(req,res){
        name = req.get["name"];
        res.body(name);
        return(res);
    };
    
    httpServer.create(server,port);
    
- `req` - The data sent at request.
 - `req.path` - String containing requested path.
 - `req.post` - Array of post request data, where available.
 - `req.get` - Array of get request data, where available.
 - `req.put` - Array of put request data, where available.
 - `req.head` - Array of all request headers.

### Static

See:

    httpServer.static(port,fileLoc,servLoc);

- `port` - The port for server to use.
- `fileLoc` - _(optional)_ Where the files to be served are, assumed to be the directory the app is operating in.
- `servLoc` - _(optional)_ Where the files will be served from, at the given port, assumed to be the root directory.