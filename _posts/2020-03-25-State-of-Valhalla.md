
I highly recommend the latest ["State of
Valhalla"](http://cr.openjdk.java.net/~briangoetz/valhalla/sov/01-background.html)
document by Brian Goetz if you're interested in the Java language (or just
language runtimes in general). It gives an accessible overview of
this huge shakeup of the JVM, made possible by the breakthrough observation
that inline classes and object references can simply re-use the JVM's
"L-carrier type".
