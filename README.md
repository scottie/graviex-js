# graviex-js
A libary for graviex API written in JS
# graviex-js

A libary for graviex API written in JS

Here is a full implimentation of the graviex exchange API in a nodejs NPM package.


> accessKey secretKey listMarkets allMarketsTicker ticker account
> allDeposits deposits deposit depositAddress orders ordersAll
> createOrder order cancelOrder clearAllOrdersSide clearAllOrders
> orderBook depth trades myTrades kLine timestamp

    //listMarkets
    //Get all available markets
    /*
    listMarkets(function(res){
    	if(!res.error){
    		//console.log(res);
    		for (var key in res) {
    			if (res.hasOwnProperty(key)) {
    				console.log(res[key]);
    			}
    			}
    	}else{
    		console.log(res)
    	}
    });
    */  

    //createOrder    
    //Create a Sell/Buy order    
    /*    
    createOrder("onzbtc", "buy", "5.0", "0.000000200", function(res){    
        if(!res.error){    
            console.log(res);    
        }else{    
           console.log("ERROR: " + res)    
        }    
    });
    
    */

# Example
Install:

    npm install graviex
	
Example:

        //Import module
        var  graviex  =  require("./graviex.js"); 
	    //Settings / Config  
        graviex.accessKey  =  "";    
        graviex.secretKey  =  ""
        
        graviex.allMarketsTicker(function(res){
	        if(!res.error){        
	            console.log(res)
	        }else{        
	            console.log(res)
	        }        
        });

For a more detailed example, please see "mm.js" in the git directory.

