## Elixir in the Medical Cannabis space -- ElixirConf2017

### Who we are...
* Chris Steinmeyer
* Mike Groseclose
* Alex Weidmann
* Justin Weidmann
* Eric Robetaille


### Weedmaps introduction
* Largest tech company in the medical marijuana space
  * Stats
    * 	traffic
    * 420 traffic

### Weedmaps timeline
* Insane growth over the last 3 years
   *  Pushing out new feature after feature
   *  Supported by 4 FTEs Development
   *  Rapidly changing market
     *  New competitors

 All lead to....

### 4/20 downtime
For those of you who don't know 4/20 is the marijuana's Black Friday. Not the day you want to be down and we had... catastrophic downtime. 🙀

* 100% 502 responses from 9:30am until 3:30pm
* Caused by
  * Bad/missing indexes
  * Select *s on massive geodata columns
  * Switch in user behavior
  * Nefarious scripting by "integration partners" 

### 4/20 mitigation in the Rails world
* Top to bottom analysis of all DB indexes, queries
* Split high traffic views into CloudFront
* New Rails 5 API backed by ES
* Tons of hardware thrown at the problem 👉💰

### What was Weedmaps technology in mid-2016?
* We needed to continue to support the Rails application for the foreseeable future.
* We needed to add new features to stay competitive in the market.
* We needed to compartmentalize our growth.

### WE NEEDED MICROSERVICES!!!

### WE NEEDED _NODE_ MICROSERVICES!!!!1!!!1!1!1
Much of the team knew Node and let's be honest can't everyone write in JavaScript? So, we started down the path of architecting a NodeJS Microservices and immediately started to notice problems. Monitoring and logging become vastly more difficult than they are in a monolith. Debugging can be a wild goose chase across services. Separation of concerns comes with a large OPS cost. Source of truth can become blurred and on and on and on.

### There was an epiphany
Alex and Justin had been playing with Elixir for a few months at this point but only on their side projects (FamlyRack), Mike had been spiking on Haskell and functional programming in general and took quickly to Elixir. And then there was me...

### GET OFF MY GODDAMN LAWN!
Me being the "elder statesman" of the team (read: anti-fanboi curmudgeon) was much slower to rush to the Elixir fountain. I had been burned over the last almost 20 years by all of the promises that the new technology on the block was going to solve my problems. I could smell snakeoil from a mile away.

### Cognitive Dissonance
So this is where a good case of cognitive dissonance set in. I really trust and respect these guys, maybe I should give this a chance. So, I did the next logical thing...

### I went on vacation
I PDF'd the getting started section from the elixir website, bought Dave Thomas' excellent book and went to Sedona. And here is where the power of Erlang, the elegance of Elixir and the scalability of Phoenix all clicked at once. I was sitting amongst the red rocks of Sedona thinking about this quagmire of microservices, message busses, replays, concurrency, debugging, OPS orchestration and then I thought about what an Elixir architecture would look like. 

### I knew enough to be dangerous

### The approach of how we introduced Elixir/Phoenix into our architecture

To be continued....


### Thanks much.
* @chrisfishwood
* @mikrofusion
* @effectz
* @nitsuj
* @eric

### We're hiring
(you don't need to smoke to work at Weedmaps. You just need to be cool.)

