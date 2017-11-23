# iota-peer-manager
IOTA IRI Peer Manager


    docker run --rm goestin/iota-peer-manager [--iri=iri_api_url] [--port=IP:your_local_port] [--refresh=interval]
      -i --iri       = The API endpoint for IOTA IRI implementation (Full Node). 
      -p --port      = Local server IP and port where the dashboard web server should be running
      -r --refresh   = Refresh interval in seconds for IRI statistics gathering (default 10s)
      -h --help      = print this message
                
    Example.
    docker run --rm goestin/iota-peer-manager -i http://127.0.0.1:14800 -p 127.0.0.1:8888
    IPM will connect to IOTA endpoint and produce the status at localhost port 8888
    To view the dashboard, simply open a browser and point to http://127.0.0.1:8888


