# auxledger-web3js
Web3js library for aux

Steps to follow for using the library -

In your program, set the path of web3js folder for using web3js library directly.

Refer below sample node program for the same -

var http = require('http');
var Web3 = require('/home/auxesis/web3.js');
var Eth = require('/home/auxesis/web3.js/lib/web3/methods/aux.js');
var Promise = require('promise');

http.createServer(function (req, res) {
    res.writeHead(200, {'Content-Type': 'text/plain'});
    res.end('Hello All!');

var aux = new Eth('http://localhost:8545');
var web3 = new Web3(new Web3.providers.HttpProvider('http://localhost:8545'));

console.log("##### web3.aux ##### ", web3.aux);

}).listen(9000);
