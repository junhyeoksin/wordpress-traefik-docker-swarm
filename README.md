# wordpress-traefik-docker-swarm
#### Wordpress with Let's Encrypt in a Dokcer Swarm


#### Create a secret for storing the password for MySQL root using the command:

#### <pre><code> printf "YourPassword" | docker secret create wordpress-mysql-root-password -</code></pre>

#### Create a secret for storing the password for WordPress database using the command:

#### <pre><code> printf "YourPassword" | docker secret create wordpress-database-password - </code></pre>

#### Clear passwords from bash history using the command:

#### <pre><code> history -c && history -w </code></pre>

#### Deploy WordPress in a Docker Swarm using the command:

#### <pre><code> docker stack deploy -c wordpress.yml wordpress</code></pre> 