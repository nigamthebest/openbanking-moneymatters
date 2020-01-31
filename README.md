# openbanking-moneymatters
Client App for Nordea Open Banking APIs
# Sample TPP Client Application
This is the Java centric "Sample TPP" application that will thrive with ["Dogfooding"](https://en.wikipedia.org/wiki/Eating_your_own_dog_food)

### Building local:

```mvn clean install``` 

## Running local, Github build:
```mvn spring-boot:run -Drun.profiles=github -fpom-github.xml```


#### Proxies
If you are running WebWallet from inside a secured network and you are using the developer portal/sandbox that is in the public network. 
Then you need to set the Company proxy for the jvm, otherwise the connection to external network does not work. 

```-Dhttp.useProxy=true -Dhttp.proxyHost=proxy.domain.net -Dhttps.proxyHost=proxy.domain.net -Dhttp.proxyPort=8080 -Dhttps.proxyPort=8080```

#### Browser 
Go to: [http://localhost:7000](http://localhost:7000)
