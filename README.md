# blog-proxy-error
Text proxy error message fix with Docker

This is a project related with a blog post I wrote on how to understand and fix a misconfigured reverse proxy when using it with Jenkins

You can find the blog post [here](https://www.sergiosanchez.com/posts/broken-reverse-proxy/)

# How to use it

To run this demo you will need docker and docker-compose installed on your system and follow these steps:

1. Clone the repo
2. Update _parameters.conf_ file setting the FQDN you want to use in the variable **$PUBLIC_HOST**
3. Create a folder named _certs_ in the root folder
4. Generate a self-signed certificate for the FQDN configured in point 2 and copy the generated files inside _certs_ folder 
with the names **nginx-selfsigned.crt** and **nginx-selfsigned.key**
5. Run command _docker-compose up_
6. Enter FQDN defined in point 2 in the browser


