---
layout: master
title: Groovy Fast Track
---

# Groovy Fast Track

Using the Groovy Fast Track you will start experimenting with GPars in about 3
minutes. We assume you have Groovy installed on your system.

## Step 1 -- Start up the Groovy Console

Start fresh Groovy Console or open up an empty groovy script source in your
favorite IDE

## Step 2 -- Add dependencies

_Note: GPars comes bundled with Groovy distributions so this step should
normally be not required._

We'll use Groovy's Grape functionaity to grab all the requited dependencies
for us. You may check ot the [GPars Integration page](Integration) for
alternative ways to integrate GPars with your project.

Add the following line to the groovy script:

## Step 3 -- Experiment with parallel collection processing

Believe it or not, now, we're ready to experiment. Try the following script,
which will concurrently query a collection of strings with regular
expressions:

Run the script and you should get the following output:

Now feel free to experiment changing the regular expressions, using different
collections or different methods, like eachParallel(), collectParallel(),
maxParallel(), sumParallel() and others. You get the idea, right?

To find out more about parallel collection processing, visit the [Parallel
Collections section](http://www.gpars.org/guide/guide/dataParallelism.html#dat
aParallelism_parallelCollections) of the [User
Guide](http://www.gpars.org/guide/).

## Step 4 -- Actors

Now we could try to build an actor and send it a couple of messages to see it
acting.

Our actor maintains a private counter and accepts different types of messages,
which result in updating the counter. Sending a null value will make the actor
reply the current counter value back to us. Notice the _send()_ method name is
optional and can be replaced by the _<<_ operator or ommited altogether.

The [Actor section](http://www.gpars.org/guide/guide/actors.html) of the [User
Guide](http://www.gpars.org/guide/) will help you dive deeper into GPars
actors.

## Further steps

Now when you have GPars runing on your system, the time is up you opened up
the [User Guide](http://www.gpars.org/guide/), browsed the [GPars code example
s](http://git.codehaus.org/gitweb.cgi?p=gpars.git;a=tree;f=src/test/groovy/gro
ovyx/gpars/samples;h=6e25c7ecb409197aced73a76719795976ee461ec;hb=HEAD) and
continued experimenting. You may also consider checking out the [Java Fast
Track](Java+Fast+Track), in case you need to use GPars high-level concurency
abstractions from Java code. Good luck!
