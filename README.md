# venom
Tool designed for fast crawl and extract endpoints



# Features

    Fast web crawler for endpoint or unlike other tools you can crawl big list of endpoints


    Extract allowed and disallowed endpoints from robots.txt for big list of endpoints that you can use disallowed endpoints with other tools to bypass 403 Status_Code to get quick money easily

    Fast extracting endpoints from sitemap.xml for list of endpoints 
 
    So if you faced any problem with tool or your machine have connection problem with internet or you closed tool you don't need to crawl all endpoints again but you can go to file that contain failed threads and complete your crawl where tool stopped from failed threads file

    Any failed or lack threads you will find it in failed threads file so you can crawl it again

    randomize User-Agent 

    Extract subdomains from crt.sh and certspotter.com and crawl it

    Extract endpoints from Wayback Machine for subdomain or list of subdomain

    if you used a lot of threads and WAF detect it you can bypass it by taking control of threads and time to delay between threads

    Crawl enpoints authenticated or unauthenticated




# Installation

#### 1- Install python3 
#### 2- Run this commands

    git clone https://github.com/omarhashem123/venom.git

    pip install -r requirements.txt

# Usage

    $ python3 venom.py

    usage: 

    to extract endpoints from crawl:

    python3 venom.py -f <file> -t <threads> -o <output file> -l <depth level> -s <scope> -time <delay> -spider

    OR

    python3 venom.py -f <file> -t <threads> -o <output file> -l <depth level> -s <scope> -time <delay> -cookie <cookie> -spider

    to extract disallowed endpoinds and allowed endpoints from robots.txt:

    python3 venom.py -f <file> -t <threads> -o <output file> -time <delay> -robots

    to extract endpoints from sitemap.xml:

    python3 venom.py -f <file> -t <threads> -o <output file> -time <delay> -sitemap

    to extract endpoints from wayback machine:

    python3 venom.py -d <domain> -o <output file> -archive

    OR

    python3 venom.py -f <file> -t <threads> -o <output file> -archive

    to extract subdomains from crt.sh:

    python3 venom.py -d <domain> -o <output file> -crtsh

    to extract subdomains from certspotter:

    python3 venom.py -d <domain> -o <output file> -certspotter


    description:Tool that spider subdomains and extract endpoints


    optional arguments:
  
    -h, --help            show this help message and exit
  
    -f F                  <file contain subdomains>
  
    -d D                  <domain or subdomain>
  
    -s S                  <only domains in scope>
  
    -time [TIME]          <time to sleep between threads>
  
    -t [T]                <threads>
  
    -l L                  <levels of crawl>
  
    -o [O]                <folder that contain results>
  
    -spider [SPIDER]      <extract endpoints from spider websites>
  
    -cookie COOKIE        <crawl with Cookie>
  
    -robots [ROBOTS]      <extract allowed endpoints and extract disallowed endpoints>
  
    -sitemap [SITEMAP]    <extract endpoints from sitemap.xml>
  
    -archive [ARCHIVE]    <extract endpoints from Wayback Machine>
  
    -crtsh [CRTSH]        <extract subdomains from crt.sh>
  
    -certspotter [CERTSPOTTER]
                        <extract subdomains from certspotter.com>
