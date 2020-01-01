# localserver1
import http.server
import socketserver

PORT = 8080
Handler = http.server.SimpleHTTPRequestHandler

with socketserver.TCPServer(("", PORT), Handler) as httpd:
    print("serving at port", PORT)
    httpd.serve_forever()

html code
<html>
     <head>
         <title>Fyellow loves contributing to ScoreLab.</title>
     </head>
       <body>
        <h1>Fyellow loves contributing to ScoreLab.</h1>
        <p>Fyellow loves contributing to ScoreLab.</p>
       </body>
</html>
