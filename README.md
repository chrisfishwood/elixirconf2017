### First Name:
Chris

### Last Name:
Steinmeyer

### Company:
Weedmaps

### Phone number:

### Email address:

### Github:
https://github.com/chrisfishwood

### Twitter:
https://twitter.com/chrisfishwood

### Country or State of Origin:
United States

### Talk title:
Elixir in the Medical Cannabis industry

### Talk abstract:
Weedmaps is the largest technology company in the Marijuana industry. We currently have 10,000 clients, across 28 states in 4 countries and handle 8.5m page views a month.
We experienced explosive growth from 2013 through now as more states legalized the medicinal use of cannabis. On 4/20 2016 - the "Black Friday of Weed" - that growth reached
a critical mass and we suffered a catastrophic outage. This outage, the resulting loss of revenue and the projected growth of cannabis legalization in the US led us to reconsider
how long the Rails monolith could support our growth.

This talk chronicles the architectural journey over the last year as our application architecture evolved from a Rails monolith to a NodeJS microservice architecture and finally to a platform of services
written in Elixir. It covers the architectural decisions that were made in the short, medium and long term and how 5 architects all came to the same conclusion through very different paths.  If we wanted to continue to support
our extreme growth in user base, while adding new features and expanding into new markets we needed an architecture that gives us flexibility, low latency, redundancy, scalability without the limits
of a monolith and the technical complexity of microservices. We needed Elixir.

### Talk TLDR:
This talk covers the decisions that led the architecture team at Weedmaps to select Elixir as the language to use as we continue to grow with the exploding Cannabis industry. When not at work, Chris spends his time with his family, writing elixir, camping, riding bikes, hiking and rock climbing.

### Target audience:
Software architecture teams that are facing the same operational challenges and architectural decisions presented by monolithic application as they try to expand or are interested in introducing Elixir to their software architecture.

### A link to your photo:
https://github.com/chrisfishwood/elixirconf2017/blob/master/csteinmeyer_profile.png

### Your Bio:
Chris Steinmeyer is a Vice President of Engineering at Weedmaps.com. Chris lives in Tucson Arizona and spends his days working with some of the best software engineers in the world solving the technical problems of a rapidly growing industry.

### Your Tagline:
Chris is an Aquarian who likes hack nights, riding bikes, half pipes, beer flights and craggy heights.

___

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
    * 	Not traffic stats because it's embarrassing how little traffic brought us down

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

