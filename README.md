#Cengage Answer Key Generator

This utility solved a problem I once had where a teacher would assign tedious crossword puzzles from cengagebrain.com.

Luckily, however, the answer key could be easily found, in XML format, from the URL!

This utility takes that input, grabs the key, and outputs the answers in an easily readable format. 

To set it up, you'll need [NodeJS](https://nodejs.org/) (if you require a CORS proxy), and a reverse proxy from your webserver. You may also want to look into [PM2](https://www.digitalocean.com/community/tutorials/how-to-use-pm2-to-setup-a-node-js-production-environment-on-an-ubuntu-vps) to have the 
proxy process always run in the background. The server js file is located in mkreq/xmlproxy.js.

The webserver configuration is written for lighttpd but can easily be adapted for other web servers, you can view it in xword.conf. It will use the URL <root>/xword/mkreq/ for the reverse proxy.

A live version can be seen at https://www.charltontrezevant.com/xword/

Enjoy!
